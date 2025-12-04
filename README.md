# PDF Splitter & Image Converter

A sophisticated client-side tool for splitting PDF files into individual pages and converting them to high-quality images. Built with a refined, minimalist interface and hosted as a static site with no server requirements.

## Features

- 📑 **PDF Page Extraction** - Split PDFs into individual PDF files
- 🖼️ **Image Conversion** - Convert PDF pages to PNG or JPG images
- 🎯 **Selective Processing** - Extract specific pages or page ranges
- 📱 **Responsive Design** - Elegant interface that works on all devices
- ⚡ **High Performance** - Client-side processing with optimized rendering
- 🔒 **Privacy First** - All processing happens locally in your browser
- 🎨 **Refined UI** - Minimalist design with subtle animations
- 📊 **Progress Tracking** - Real-time progress updates during processing

## How to Use

### Basic Usage
1. **Upload PDF**: Click "Choose PDF File" or drag and drop a PDF onto the upload area
2. **Select Mode**: Choose between "Split to PDF Pages" or "Convert to Images"
3. **Specify Pages**: Enter page numbers (e.g., `1,3,5` or `1-5` or `all`)
4. **Process**: Click "Process PDF" to start extraction/conversion
5. **Download**: Individual download buttons appear for each processed page

### Page Selection Examples
- `all` - Process all pages
- `1` - Only page 1
- `1,3,5` - Pages 1, 3, and 5
- `1-5` - Pages 1 through 5
- `1-3,7,10-12` - Pages 1-3, page 7, and pages 10-12

### Output Options

**PDF Pages**
- Individual PDF files for each selected page
- Maintains original quality and text selectability
- Perfect for sharing specific pages or creating page-by-page documents

**Image Conversion**
- **PNG Format**: Lossless compression, transparent backgrounds supported, larger file size
- **JPG Format**: Lossy compression, smaller file size, good for photos and complex images
- **High Resolution**: 2x scale factor for crisp, detailed images
- **Web-Ready**: Optimized for presentations, websites, and social media

## GitHub Pages Deployment

### Quick Setup
1. **Create Repository**: Create a new repository on GitHub
2. **Upload Files**: Add these files to your repository:
   - `index.html` (rename `pdf-splitter.html` to `index.html`)
   - `README.md`
3. **Enable Pages**: Go to Settings → Pages → Deploy from main branch
4. **Access**: Your splitter will be live at `https://[username].github.io/[repo-name]`

### File Structure
```
pdf-splitter/
├── index.html          # Complete application
└── README.md          # Documentation
```

## Technical Specifications

### Dependencies
- **PDF.js**: Mozilla's PDF rendering library for page-to-canvas conversion
- **PDF-lib**: JavaScript library for PDF manipulation and page extraction
- **Google Fonts**: Playfair Display (serif) and Source Sans 3 (sans-serif)

### Browser Requirements
- **Modern Browsers**: Chrome 60+, Firefox 55+, Safari 12+, Edge 79+
- **JavaScript Features**: ES6+, Canvas API, File API, ArrayBuffer support
- **Memory**: Sufficient RAM for PDF processing (varies by file size)

### Performance Considerations
- **File Size Limits**: Typically handles files up to 100-200MB (browser dependent)
- **Page Limits**: Efficiently processes PDFs with hundreds of pages
- **Image Quality**: 2x scale factor provides high-resolution output
- **Processing Speed**: ~1-3 seconds per page for typical documents

## Design Philosophy

The PDF Splitter features a **refined minimalist** aesthetic that contrasts beautifully with typical utility apps:

### Visual Identity
- **Typography**: Playfair Display serif for elegance, Source Sans 3 for readability
- **Color Palette**: Earthy greens and browns with cream accents
- **Layout**: Generous whitespace, subtle shadows, gentle animations
- **Interactions**: Smooth hover effects, progressive disclosure of features

### User Experience
- **Progressive Enhancement**: Features reveal as users upload files
- **Visual Feedback**: Clear status indicators and progress tracking
- **Accessible**: High contrast ratios and keyboard navigation support
- **Responsive**: Fluid layouts that adapt to any screen size

## Privacy & Security

### Data Protection
- **100% Client-Side**: No files ever leave your browser
- **No Tracking**: No analytics, cookies, or data collection
- **Local Processing**: All PDF manipulation happens on your device
- **Memory Management**: Processed data is automatically cleaned up

### Security Features
- **File Type Validation**: Only accepts valid PDF files
- **Error Handling**: Graceful failure for corrupted or invalid files
- **Resource Limits**: Browser-based memory management prevents crashes

## Advanced Usage

### Batch Processing Tips
1. **Large Files**: Process in smaller page ranges for better performance
2. **Memory Management**: Close other browser tabs when processing large PDFs
3. **Download Organization**: Files are named systematically (`page-1.pdf`, `page-2.png`, etc.)

### Quality Settings
- **PDF Output**: Maintains original vector quality and text selectability
- **PNG Output**: Lossless compression, perfect for documents with text
- **JPG Output**: 95% quality setting, optimized file size for images

### Browser Optimization
- **Chrome**: Best performance for large files
- **Firefox**: Excellent memory management
- **Safari**: Good performance on macOS/iOS
- **Edge**: Fast processing on Windows

## Troubleshooting

### Common Issues

**"Error loading PDF"**
- Ensure the file is a valid, non-corrupted PDF
- Check that the file isn't password-protected
- Try with a smaller file to test functionality

**"Processing stuck"**
- Large files may take several minutes to process
- Check browser memory usage (close other tabs)
- Try processing fewer pages at once

**"Download not working"**
- Ensure browser allows automatic downloads
- Check that popup blockers aren't interfering
- Try right-clicking download buttons and "Save As"

### Performance Tips
- **Close unused browser tabs** before processing large files
- **Use page ranges** instead of processing entire large documents
- **Choose appropriate format**: PDF for text documents, images for visual content

## Contributing

Contributions are welcome! Areas for enhancement:

### Potential Features
- **Page preview thumbnails** before processing
- **Batch file processing** (multiple PDFs at once)
- **Custom image resolution** settings
- **Password-protected PDF support**
- **Compression options** for output files

### Development Setup
1. Fork the repository
2. Make changes to the HTML file
3. Test thoroughly with various PDF types
4. Submit pull request with detailed description

## License

This project is open source and available under the [MIT License](LICENSE).

## Support

### Getting Help
- **GitHub Issues**: Report bugs and request features
- **Documentation**: Refer to this README for usage guidance
- **Browser Console**: Check for error messages when troubleshooting

### Known Limitations
- **Memory constraints**: Very large files (500MB+) may cause issues
- **Password protection**: Encrypted PDFs are not supported
- **Form fields**: Interactive PDF elements are not preserved in splits
- **Annotations**: Comments and markups may not transfer to split files

---

**Built for Privacy**: This tool processes files entirely in your browser, ensuring your documents never leave your device.
