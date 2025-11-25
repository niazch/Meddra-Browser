# MedDRA Browser

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![GitHub Pages](https://img.shields.io/badge/Hosted%20on-GitHub%20Pages-brightgreen)](https://pages.github.com/)

A client-side web application for browsing MedDRA (Medical Dictionary for Regulatory Activities) terminology hierarchies.

**Developed by Muanda-Lab 2025**

![MedDRA Browser Screenshot](https://img.shields.io/badge/MedDRA-Browser-purple?style=for-the-badge)

---

## 🌟 Features

### 📁 File Upload
- Drag & drop or click to select MedDRA ASCII files
- Supports all standard MedDRA files:
  - `soc.asc` - System Organ Class
  - `hlgt.asc` - High Level Group Term
  - `hlt.asc` - High Level Term
  - `pt.asc` - Preferred Term
  - `llt.asc` - Lowest Level Term
  - `soc_hlgt.asc` - SOC-HLGT relationships
  - `hlgt_hlt.asc` - HLGT-HLT relationships
  - `hlt_pt.asc` - HLT-PT relationships
  - `mdhier.asc` - Full hierarchy data

### 🌳 Hierarchy Browser
- Interactive tree view navigation
- Full hierarchy: **SOC → HLGT → HLT → PT → LLT**
- Color-coded level badges for easy identification
- Expandable/collapsible nodes
- Detailed information panel

### 🔍 Search Function
- Search across all levels or filter by specific level
- Highlighted matching text in results
- Click-to-navigate functionality

### #️⃣ Code Lookup
- Direct lookup by MedDRA code
- Full hierarchy path display
- Support for terms with multiple SOC placements

### 🔒 Security Features
- Password-protected access
- All data processed locally in browser
- No data transmitted to external servers
- Session-based authentication

---

## 🚀 Getting Started

### Prerequisites
- A valid MedDRA subscription from [MedDRA MSSO](https://www.meddra.org/)
- MedDRA ASCII distribution files
- A modern web browser (Chrome, Firefox, Safari, Edge)

### Usage

1. **Access the Tool**: Navigate to the hosted URL
2. **Enter Password**: Input the access password provided by your administrator
3. **Upload Files**: Drag & drop your MedDRA ASCII files or click to select
4. **Browse**: Navigate the hierarchy, search terms, or lookup codes

---


## 📋 File Format Reference

### ASCII File Structure

MedDRA ASCII files use `$` as the field delimiter:

| File | Format |
|------|--------|
| `soc.asc` | `code$name$abbrev$...` |
| `hlgt.asc` | `code$name$...` |
| `hlt.asc` | `code$name$...` |
| `pt.asc` | `code$name$null$soc_code$...` |
| `llt.asc` | `code$name$pt_code$currency$...` |
| `soc_hlgt.asc` | `soc_code$hlgt_code$...` |
| `hlgt_hlt.asc` | `hlgt_code$hlt_code$...` |
| `hlt_pt.asc` | `hlt_code$pt_code$...` |
| `mdhier.asc` | `pt_code$hlt_code$hlgt_code$soc_code$pt_name$hlt_name$hlgt_name$soc_name$...` |

---

## ⚖️ Legal Notice

### MedDRA Licensing

MedDRA is a registered trademark of the International Council for Harmonisation of Technical Requirements for Pharmaceuticals for Human Use (ICH).

- MedDRA data requires a valid subscription
- Data redistribution is prohibited
- This tool does NOT include MedDRA data
- Users must provide their own licensed MedDRA files

For MedDRA subscriptions, visit: [https://www.meddra.org/](https://www.meddra.org/)

### Privacy

- All data is processed locally in your browser
- No MedDRA data is transmitted to any server
- No analytics or tracking implemented
- Session data is stored only in browser sessionStorage

---

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

**Note**: This license applies only to the browser application code, NOT to MedDRA data which is separately licensed.


---

## 🙏 Acknowledgments

- [MedDRA MSSO](https://www.meddra.org/) for the medical terminology standard
- [Tailwind CSS](https://tailwindcss.com/) for the styling framework
- [Font Awesome](https://fontawesome.com/) for the icons

---

<p align="center">
  <strong>Developed with ❤️ by Muanda-Lab 2025</strong>
</p>
