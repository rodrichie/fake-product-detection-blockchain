---

<p align="center">A blockchain-based Management System for anti-counterfeits by QR codes.</p>

# Fake Product Detection using QR Codes and Blockchain

A comprehensive system for authenticating products and eliminating counterfeits using blockchain technology and QR code verification.

## About
+ In today's world, how do you know if you are buying a genuine product?
+ For more than a decade now, RFID (Radio Frequency IDentification) technology has been quite effective in providing anti-counterfeits measures in the supply chain.
+ We leverage the idea of Bitcoin's blockchain that anyone can check the proof of possession of balance. Along with this, we plan to use QR codes.
+ We plan to implement a proof-of-concept system employing a blockchain-based decentralized application which gives a customer the entire history of a product (eg - brand info, owner, etc).

### Data Flow
![Data Flow](https://imgur.com/VGIPtDU.png)

### Why blockchain?
+ Unlike a normal database, Blockchain has a non-destructive (immutable) way to track data changes over time. This means that data is not editable rather, whenever updates are made, a new block is added to the "block-chain". This helps track historical data (authenticity and owner data) of a product.
+ Given the amount of data to be dealt with (large amount of products being developed), if you have to keep track of all of them, it is better to have a decentralized and distributed network of nodes so that no entity can tamper with the product data and we also obtain 100% up time.
+ Transparent nature of the Blockchain helps avoid [parallel trade](https://en.wikipedia.org/wiki/Parallel_import).
+ Using Blockchain, authenticity can be checked and ownership of a product can be transferred _decades_ from now; even if the product is discontinued.

## Features

- **Blockchain-based Authentication**: Immutable product records
- **QR Code Integration**: Easy product verification  
- **Admin Panel**: Product registration and management
- **User Interface**: Product verification and tracking
- **GUI Application**: User-friendly desktop interface

## Getting Started

### Prerequisites

+ Python 3.x
+ Required Python packages:
  - tkinter (for GUI)
  - opencv-python (for image processing)
  - pillow (PIL for images)
  - qrcode (for QR code generation)
  - pyzbar (for QR code reading)
  - pymysql (for database operations)

### Installation

**1. Clone the repository**
```bash
git clone git@github.com:rodrichie/fake-product-detection-blockchain.git
cd fake-product-detection-blockchain
```

**2. Install required packages**
```bash
pip install opencv-python pillow qrcode pyzbar pymysql tkinter
```

**3. Set up the database**
+ Make sure you have MySQL installed and running
+ Configure your database connection in the application files

**4. Run the application**
```bash
python Main.py
```

## Usage

1. Launch the application using `Main.py`
2. Choose between Admin or User mode
3. **For Admin**: Register new products and generate QR codes
4. **For User**: Scan QR codes to verify product authenticity

## Built With

**GUI Application:**
+ [Python Tkinter](https://docs.python.org/3/library/tkinter.html) - GUI framework
+ [MySQL](https://pypi.org/project/pymysql/) - Database for login/register
+ [qrcode](https://pypi.org/project/qrcode/) - QR code generation
+ [pyzbar](https://pypi.org/project/pyzbar/) - QR code reading
+ [OpenCV](https://opencv.org/) - Image processing
+ [PIL/Pillow](https://pillow.readthedocs.io/) - Image handling

**Blockchain:**
+ [Python Blockchain Implementation](https://www.activestate.com/blog/how-to-build-a-blockchain-in-python/) - Custom blockchain solution

## Project Structure

```
fake-product-detection-blockchain/
├── Main.py                 # Main application entry point
├── Admin.py               # Admin interface and functionality
├── User.py                # User interface and functionality  
├── blockchain.py          # Blockchain implementation
├── database/              # Database related files
├── images/                # Image assets
├── qr_codes/             # Generated QR codes
└── README.md             # Project documentation
```

## Limitations

+ The user needs to have a QR code scanner in order to check the product information.
+ Products that have already been manufactured prior to implementation cannot be tracked.
+ We currently depend on the company to register with our services, without which, we cannot provide information about a brand to the user.

## Future Scope

+ Making an Android app based on this architecture 
+ To track every genuine product that is to be sold.
+ Implement this idea in other fields.
+ Virtual transactions
+ Using tamper-proof tags
+ Dynamic (read & write NFC tags)
+ QR codes that have secure graphics
+ Implement custom tokens which can be sold to users so that they can purchase ownership of a product using tokens that helps in insurance processing.

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is open source and available under the [MIT License](LICENSE).

## Repository

🔗 **GitHub Repository**: [rodrichie/fake-product-detection-blockchain](https://github.com/rodrichie/fake-product-detection-blockchain)

---

<p align="center">Made with ❤️ for product authentication and anti-counterfeiting</p>
