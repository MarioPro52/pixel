# pixelclass Pixel:
    def __init__(self, x, y, color="white"):
        self.x = x          # X-coordinate of the pixel
        self.y = y          # Y-coordinate of the pixel
        self.color = color  # Color of the pixel

    def set_color(self, color):
        self.color = color
        print(f"The pixel at ({self.x}, {self.y}) is now {self.color}.")

    def move(self, new_x, new_y):
        self.x = new_x
        self.y = new_y
        print(f"The pixel has been moved to ({self.x}, {self.y}).")

# Example usage:
pixel = Pixel(5, 10, "red")  # Create a pixel at position (5, 10) with color red
print(f"Initial position: ({pixel.x}, {pixel.y}), color: {pixel.color}")

pixel.set_color("blue")  # Change the pixel's color to blue
pixel.move(8, 12)        # Move the pixel to a new position (8, 12)
