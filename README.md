#include <stdio.h>

// Function to calculate travel time
double calculate_travel_time(double distance, double speed) {
    return distance / speed;
}

int main() {
    double distance, speed, travel_time;

    // Getting user input for distance
    printf("Enter the distance to the celestial body (in light years): ");
    scanf("%lf", &distance);

    // Getting user input for speed
    printf("Enter the speed of the spaceship (as a fraction of the speed of light, e.g., 0.5 for half the speed of light): ");
    scanf("%lf", &speed);

    // Calculating travel time
    travel_time = calculate_travel_time(distance, speed);

    // Displaying the result
    printf("At a speed of %.2lf times the speed of light, it will take %.2lf years to reach the destination.\n", speed, travel_time);

    return 0;
}
