# localBooru
A desktop application that lets users tag and search local image folders (and their sub-folders) like a Booru site.

## Features
- Tag and organize your local image collection
- Fast image searching by tags and ratings
- Automatic thumbnail generation
- Scan folders recursively for images
- SQLite database for storing image metadata and tags

## Requirements
- Python 3.12+
- PySide6
- SQLModel
- Pillow

## Installation

1. Clone this repository:
```bash
git clone https://github.com/yourusername/localbooru.git
cd localbooru
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

## Usage

Run the application:
```bash
python -m localbooru
```

### Basic Workflow

1. Use "Folder → Scan" to add images to your database
2. Select images in the thumbnail grid to add tags
3. Use the filter bar to search for images by tags

### Filter Syntax

The filter bar supports the following syntax:
- `tag:cat` - Search for images with the "cat" tag
- `rating:safe` - Search for images with the "safe" rating
- `cat dog` - Search for images with both "cat" and "dog" tags

## Development

The project is structured as follows:

- `localbooru/db/` - Database models and query functions
- `localbooru/ui/` - User interface components
- `localbooru/utils/` - Utility functions for file operations

## License
Read the License.md for details.
