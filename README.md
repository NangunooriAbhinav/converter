# Yoink

**Yoink** is a versatile command-line tool for converting files between different formats. It currently supports converting images to JPEG and PNG formats, as well as converting documents to PDF format.

## Features

- Convert images to JPEG or PNG format.
- Convert documents to PDF format.
- Easy-to-use command-line interface.

## Installation

To install **Yoink**, follow these steps:

### Prerequisites

- **Go** must be installed on your system. You can download and install it from [the official Go website](https://golang.org/dl/).
- **LibreOffice** must be installed on your system for document-to-PDF conversion. You can download and install it from [the official LibreOffice website](https://www.libreoffice.org/download/download/).

### Installation Steps

1. **Clone the Repository (Optional)**

   If your project is hosted in a Git repository, clone it to your local machine:

   ```bash
   git clone https://github.com/yourusername/yoink.git
   cd yoink
   ```

2. **Build and Install**

   Run the provided installation script to compile the Go code and install the `yoink` command globally on your system:

   ```bash
   ./install.sh
   ```

   This script will:

   - Compile the Go program into an executable named `yoink`.
   - Move the executable to `/usr/local/bin` to make it accessible from anywhere in your terminal.
   - Ensure the executable has the correct permissions.

### Manual Installation (Alternative)

If you prefer to manually install the tool without using the installation script:

1. **Build the Go Program**

   ```bash
   go build -o yoink
   ```

2. **Move the Executable to a Directory in Your `PATH`**

   ```bash
   sudo mv yoink /usr/local/bin/
   ```

3. **Ensure Executable Permissions**

   ```bash
   sudo chmod +x /usr/local/bin/yoink
   ```

## Usage

After installation, you can use the `yoink` command to convert images and documents.

### Basic Command Syntax

```bash
yoink [input file path] [output file path] [flag]
```

### Options

- **Image Conversion**:
  - `-ij`: Convert the image to JPEG format.
  - `-ip`: Convert the image to PNG format.
- **Document Conversion**:
  - `-dp`: Convert the document to PDF format.

### Examples

1. **Convert an Image to JPEG**

   ```bash
   yoink /path/to/image.png /path/to/output.jpg -ij
   ```

   This will convert `image.png` to `output.jpg`.

2. **Convert an Image to PNG**

   ```bash
   yoink /path/to/image.jpg /path/to/output.png -ip
   ```

   This will convert `image.jpg` to `output.png`.

3. **Convert a Document to PDF**

   ```bash
   yoink /path/to/document.docx /path/to/output.pdf -dp
   ```

   This will convert `document.docx` to `output.pdf`.

### Help

To display help information:

```bash
yoink -h
```

## Contributing

If you'd like to contribute to **Yoink**, please feel free to submit a pull request or open an issue on the project's GitHub page.

## License

This project is licensed under the MIT License. See the LICENSE file for more details.

---
