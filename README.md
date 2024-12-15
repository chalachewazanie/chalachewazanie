#include <windows.h>
#include <GL/glut.h>
void drawLogo() { // Set up the graphics window
    // Draw the outer oval
    void initgraph(int *graphdriver, int *graphmode, char *pathtodriver)

    setfillstyle(SOLID_FILL, BLUE);
    ellipse(320, 240, 0, 360, 200, 120); // Center (320, 240)
    floodfill(320, 240, BLUE);

    // Draw the inner white oval
    setcolor(WHITE);
    setfillstyle(SOLID_FILL, WHITE);
    ellipse(320, 240, 0, 360, 180, 100);
    floodfill(320, 240, WHITE);

    // Draw the yellow base inside
    setcolor(YELLOW);
    setfillstyle(SOLID_FILL, YELLOW);
    ellipse(320, 240, 0, 360, 150, 70);
    floodfill(320, 240, YELLOW);

    // Draw a basic castle (symbolic)
    setcolor(BLACK);
    rectangle(240, 180, 280, 220); // Left tower
    rectangle(280, 160, 320, 220); // Middle tower
    rectangle(320, 180, 360, 220); // Right tower
    floodfill(250, 190, BLACK);
    floodfill(300, 170, BLACK);
    floodfill(340, 190, BLACK);

    // Add a wheel or gear symbol (simplified)
    setcolor(BLACK);
    circle(320, 260, 20);
    setfillstyle(SOLID_FILL, BLACK);
    floodfill(320, 260, BLACK);

    // Add text
    setcolor(BLUE);
    settextstyle(SANS_SERIF_FONT, HORIZ_DIR, FONT_SIZE 12);
    outtextxy(220, 110, "UNIVERSITY OF GONDAR");

   
}
