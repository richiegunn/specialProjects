# specialProjects

import matplotlib.pyplot as plt

def generate_y_coordinates(x_values, line):
    y_values = []
    for x in x_values:
        y = line[0] * x + line[1]
        y_values.append(y)
    return y_values

# Example line: y = 2x + 1
line = (2, 1)

# Define the range of x-axis values
x_values = range(-10, 11)

# Generate y-coordinates
y_values = generate_y_coordinates(x_values, line)

# Plot the line
plt.plot(x_values, y_values)
plt.xlabel('x')
plt.ylabel('y')
plt.title('Line: y = 2x + 1')
plt.grid(True)
plt.show()
