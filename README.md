# Avoiding-file-redownload-Chatapp
Avoiding Duplicate File Downloads and Forward Monitoring System Developed an efficient file-sharing platform that prevents redundant downloads using SHA-256 hashing for duplicate detection. Implemented a file-forwarding tracking system that binds sender details to a queue, allowing administrators to trace file propagation.

# Avoiding Duplicate File Downloads and Forward Monitoring System

## 📌 Project Overview
In today's fast-paced digital world, file-sharing platforms face challenges such as redundant file transfers, inefficient tracking, and lack of transparency in file propagation. This project aims to **detect duplicate file downloads and monitor file forwarding** to improve storage efficiency and provide traceability.

## 🚀 Features
- **Duplicate File Detection:** Uses **SHA-256 hashing** to prevent unnecessary downloads.
- **File Forwarding Tracking:** Binds sender details to a queue, enabling **complete propagation tracking**.
- **Real-time User Alerts:** Users are notified if they receive a duplicate file with options to **Cancel or Download Anyway**.
- **Admin Monitoring Dashboard:** Allows admins to **view forwarding history** and analyze file movements.
- **Cloud Integration:** Utilizes **Firebase and Cloudinary** for scalable storage and real-time synchronization.

## 🔍 System Architecture
### High-Level Design
The system consists of four key modules:
1. **Chat-file Transfer Module** - Manages file transfers.
2. **Duplicate Detection Module** - Compares file hashes for redundancy.
3. **Queue Management Module** - Tracks file forwarding paths.
4. **Admin Monitoring Module** - Enables file propagation tracking.

### Process Flow
1. A file is uploaded, and its **SHA-256 hash** is generated.
2. Before downloading, the hash is checked against **local storage** to detect duplicates.
3. If a duplicate exists, the user is given an option to **cancel or proceed**.
4. Forwarding is tracked by storing sender details in a queue, allowing **admins to monitor file movement**.

## 📂 Data Structures
- **Hash Tables:** Store file metadata (name, size, hash) for efficient duplicate detection.
- **Queues:** Maintain file-forwarding history.

## 🛠️ Tech Stack
- **Backend:** Firebase (Real-time Database)
- **Storage:** Cloudinary (File Storage)
- **Framework:** Android SDK
- **Database:** SQLite

## 🔬 Test Cases
1. **Login System:** Verify successful login and error handling.
2. **File Upload:** Ensure correct storage of file metadata.
3. **Duplicate Detection:** Validate hashing mechanism and user alerts.
4. **File Forwarding:** Confirm that forwarding queues update correctly.
5. **Admin Dashboard:** Ensure complete traceability of file propagation.

## 🏆 Conclusion
This project successfully prevents redundant downloads using **hash-based verification**, enhances user experience with **real-time duplicate alerts**, and provides **admin-level monitoring** for file propagation. Future enhancements include **end-to-end encryption**, **multi-device hash synchronization**, and **detailed analytics for admins**.

## 📌 Future Enhancements
- 🔐 **Advanced Encryption** for secure file transfers.
- 🔄 **Multi-device Hash Sync** for better cross-device tracking.
- 📊 **Admin Analytics Dashboard** for monitoring file-sharing trends.
- 🔍 **Graphical Forwarding Visualization** for better traceability.
- 📁 **Support for Large File Sizes** with optimized handling.
