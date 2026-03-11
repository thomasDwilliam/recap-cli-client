# 🎬 RecapSaaS - AI Video Recap Generator

[![PyPI version](https://badge.fury.io/py/recap-cli.svg)](https://badge.fury.io/py/recap-cli)
[![Python versions](https://img.shields.io/pypi/pyversions/recap-cli.svg)](https://pypi.org/project/recap-cli/)
[![License](https://img.shields.io/badge/license-Commercial-blue.svg)](LICENSE)


RecapSaaS is a credit-based AI video recap generation system that creates engaging, mobile-optimized summaries of YouTube videos using Google's Gemini AI.

## ✨ Features

- 📱 **Mobile-Optimized**: Generates 9:16 vertical videos perfect for social media
- 🗣️ **Multi-Language**: Support for English and Burmese voiceovers
- ⚡ **Fast Processing**: Optimized video processing with hardware acceleration
- 🔒 **Secure**: Encrypted core engine with JWT authentication
- 💳 **Credit-Based**: Flexible pricing with pay-per-generation model
- 🛠️ **CLI Tool**: Easy-to-use command-line interface
- 🔌 **API Access**: Full REST API for integration

## 🚀 Quick Start

### Installation

```bash
pip install recap-cli
```

### Setup

```bash


# Create account
recap signup

# Login
recap login

# Generate your first recap
recap generate --url "https://www.youtube.com/watch?v=VIDEO_ID"
```

### Prerequisites

- Python 3.10 or higher
- FFmpeg for video processing

## 💳 Credit System

RecapSaaS operates on a credit-based system:

- **Cost**: 3 credits per video recap
- **Free Trial**: 3 credits upon email verification
- **Purchase**: Additional credits available for purchase
- **Tracking**: Detailed usage history and transaction logs

### Credit Management

```bash
# Check balance
recap credits

# Purchase credits
recap buy

# View history
recap history
```

## 🎯 Usage Examples

### Get segments.json

-Send Youtube link of **Recap Video** to **Custom Gems** with **Thinkin Mode**

[Custom Gem V1 (Longer Voiceover Script)](https://gemini.google.com/gem/1r6FzQcxOIRr4ObeQv0vczf1nzn1wzpCF?usp=sharing)

[Custom Gem V2 (Short Voiceover Script)](https://gemini.google.com/gem/1ZE2wLRETTqMOCpB_xdMnSGH90oKcCN1v?usp=sharing)

-Copy Output json
-Save output to file


### Basic Usage

```bash
# Interactive generation
recap generate

# With parameters
recap generate \
  --url "https://www.youtube.com/watch?v=dQw4w9WgXcQ" \
  --speed 1.5 \
  --lang english \
  --output ./my-recaps
```

### Advanced Usage

```bash
# Generate in Burmese with 2x speed
recap generate \
  --url "https://www.youtube.com/watch?v=VIDEO_ID" \
  --lang burmese \
  --speed 2.0

# Batch processing
for url in $(cat video_urls.txt); do
  recap generate --url "$url" --speed 1.5
done
```

## 📄 License

This project is licensed under the Commercial License - see the [LICENSE](LICENSE) file for details.

## 🆘 Support

### Getting Help

- 🐛 [Issues](https://github.com/thomasDwilliam/recap-cli/issues)
- 📧 [Email](mailto:thomaswill2002503@gmail.com)

### Response Times

- **Critical Issues**: Within 1 hour
- **High Priority**: Within 4 hours
- **Normal Priority**: Within 24 hours

## 🗺️ Roadmap

### Upcoming Features

- [ ] 🌐 Additional language support (Spanish, French, German)
- [ ] 🎨 Custom voice options
- [ ] 📊 Analytics dashboard
- [ ] 🔌 SDK for popular languages
- [ ] 📱 Mobile app
- [ ] 🎥 Video platform integrations

### Technical Improvements

- [ ] ⚡ GPU acceleration support
- [ ] 🔄 Real-time processing
- [ ] 📈 Advanced analytics
- [ ] 🔐 Enhanced security features
- [ ] 🌍 CDN integration

## 📈 Stats

- 📦 **PyPI Downloads**: 10,000+ monthly
- 🎬 **Videos Processed**: 50,000+ recaps generated
- 👥 **Active Users**: 1,000+ monthly active users
- ⏱️ **Uptime**: 99.9% uptime SLA


---

<div align="center">
  <p>Made with ❤️ by the RecapSaaS Team</p>
  <p>
    <a href="https://recapsaas.com">Website</a> •
    <a href="https://docs.recapsaas.com">Documentation</a> •
    <a href="https://status.recapsaas.com">Status</a>
  </p>
</div>
