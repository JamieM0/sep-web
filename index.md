# SEP for Web

![SEP for Web](assets/images/wordmark-inline.png)

**Simple. Private. Portable.**

SEP for Web is a single-file encryption tool that runs entirely in your browser. Encrypt files, create secure containers, and protect your data without uploading anything to servers or requiring internet access.

## What is SEP for Web?

SEP for Web is a complete encryption solution contained in one HTML file. You can download `sep.html`, open it in any modern browser, and start encrypting files immediately. Everything happens locally on your device - no accounts, no servers, no data transmission.

## Key Benefits

- **Complete Privacy**: Your files never leave your device. All encryption happens locally in your browser.
- **Zero Dependencies**: No installation required. Works on any device with a modern web browser.
- **Offline First**: Once downloaded, works without internet connection.
- **Cross Platform**: Runs on Windows, Mac, Linux, phones, and tablets.
- **No Vendor Lock-in**: Open source single file that you control completely.

## Core Features

### File Encryption
- Encrypt any file type with password or keyfile protection
- Uses AES-GCM 256-bit encryption with PBKDF2-SHA-256 key derivation
- Password strength meter with warnings for weak passwords
- Bulk encryption of multiple files at once

### Keyfile System
- Generate cryptographically secure keyfiles
- Use keyfiles as an alternative to passwords for high-entropy security
- Keyfiles can be stored separately from encrypted data

### Secure Lockers
- Bundle multiple files into encrypted containers
- Optional removal of folder structure for privacy
- Password or keyfile protection for lockers
- Single download contains all your files

### Text Encryption
- Encrypt and decrypt text strings directly
- Copy results to clipboard with one click
- Switch between encrypt and decrypt modes easily

### Cross-Platform Compatibility
- Works on any device with a modern web browser
- Consistent experience across Windows, Mac, Linux, and mobile devices
- No installation or setup requirements

### Additional Features
- Built-in progress tracking for all operations
- Keyboard shortcuts for faster workflow
- Responsive design works on mobile devices
- Password strength analysis and recommendations

## Use Cases

### Personal Data Protection
- Encrypt sensitive documents before storing in cloud services
- Protect personal photos and videos
- Secure tax documents and financial records
- Encrypt backup files before external storage

### Professional Applications
- Secure client files and confidential documents
- Encrypt project files for remote work
- Protect intellectual property and research data
- Secure communication of sensitive materials

### Educational and Research
- Demonstrate encryption concepts and security practices
- Protect research data and academic work
- Educational tool for understanding client-side cryptography
- Safe experimentation with encryption workflows

### Travel and Mobile Security
- Encrypt files before traveling with devices
- Secure documents on public or shared computers
- Protect data on USB drives and external storage
- Emergency file encryption when away from trusted systems

## Unique Selling Points

1. **Single File Solution**: Everything you need in one HTML file that runs anywhere
2. **100% Client-Side**: No servers, no accounts, no data transmission
3. **Instant Access**: No downloads, installations, or setup required
4. **Universal Compatibility**: Works on any device with a web browser
5. **Complete Offline Operation**: Full functionality without internet access
6. **Educational Transparency**: Open implementation for learning and verification
7. **Zero Ongoing Costs**: No subscriptions, licenses, or recurring fees
8. **Portable Security**: Take your encryption tool anywhere
9. **No Vendor Dependencies**: You own and control the entire application
10. **Privacy by Design**: Impossible for developers to access your data

## Technical Implementation

- **Encryption**: AES-GCM with 256-bit keys
- **Key Derivation**: PBKDF2-SHA-256 (100,000 iterations for passwords, 10,000 for keyfiles)
- **Random Generation**: Uses Web Crypto API for secure randomness
- **File Formats**: .sep for encrypted files, .locker for containers, .key for keyfiles

## Getting Started

1. Download `sep.html` from this repository
2. Open the file in any modern web browser
3. Start encrypting files immediately
4. Keep the HTML file for future use - it contains everything you need

## Security Notes

- This is a university research project - use appropriate caution for critical data
- No password recovery system - lost passwords mean lost access to files
- No rate limiting on decryption attempts - use strong passwords or keyfiles

## Browser-Based Encryption Limitations

SEP for Web provides strong encryption but operates within browser security constraints:

**Environment Access**: Your browser, installed extensions, and system processes can access application memory and data during processing. This is an inherent limitation of web-based tools.

**Memory Management**: Decrypted data temporarily exists in browser memory and may be written to swap files or included in crash dumps by the operating system.

**Recommended Usage**: Ideal for protecting files from casual access, cloud storage encryption, and educational purposes. For highly sensitive data, consider dedicated desktop encryption tools with OS-level security features.

**Browser Recommendations**: For enhanced privacy, consider browsers that don't collect telemetry by default, such as Firefox with strict privacy settings or privacy-focused alternatives.

## Future Development

- Password Library: Built-in password management for encrypted files
- Password Manager Integration: Explore Bitwarden and other API integrations
- Enhanced locker management and organization features

---

**Status**: Core MVP complete with full feature set

SEP for Web gives you powerful encryption tools without compromising your privacy or requiring complex setup. Download once, use everywhere, trust no one but yourself with your data.
