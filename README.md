# Zephyr Project

This is a Zephyr RTOS project initialized using `west init`. Zephyr is a scalable real-time operating system (RTOS) supporting multiple hardware architectures.

## Project Structure

- **zephyr/**: Main Zephyr RTOS source code
- **modules/**: Hardware abstraction layers (HALs) and libraries
- **bootloader/mcuboot/**: MCUboot secure bootloader
- **tools/**: Development and testing tools

## Getting Started

### Prerequisites

- Zephyr SDK installed
- West tool installed
- Python 3.8 or later

### Building a Sample

To build a sample application:

```bash
# Navigate to a sample directory
cd zephyr/samples/hello_world

# Build for your target board
west build -b <your_board>

# Flash to device
west flash
```

### Common Commands

```bash
# List available boards
west boards

# List available samples
west list-samples

# Update west workspace
west update

# Build a project
west build

# Flash to device
west flash
```

## Development

This project uses git submodules to manage the various Zephyr components. When cloning this repository, use:

```bash
git clone --recursive git@github.com:rgrinnovatellc/zephyrproject.git
```

Or if already cloned:

```bash
git submodule update --init --recursive
```

## License

This project follows the Zephyr project licensing. See individual component directories for specific license information.