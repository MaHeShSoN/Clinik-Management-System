
<p align="center">
  <img src="https://github.com/user-attachments/assets/c8085d67-513c-4fd5-b76f-8410b26f5774" width="200"/>
  <img src="https://github.com/user-attachments/assets/bfe226e1-2cbb-47c6-b97c-da921a63a15c" width="200"/>
  <img src="https://github.com/user-attachments/assets/5916c5d8-66f9-4943-b327-46bd675e5ee2" width="200"/>
</p>



# Clinic Management System

A comprehensive Android application built with Kotlin and MVVM architecture for managing medical clinic operations, inventory, and sales.

## 🏥 Project Overview

This application streamlines medical clinic operations by providing a complete solution for inventory management, sales processing, and automated reporting. The system is designed to handle various types of medical products with dynamic form generation and real-time data synchronization.

## ✨ Key Features

### 📋 Dynamic Medicine Management
- **5 Medicine Types**: Tablets/Capsules, Syrups/Liquids, Creams/Ointments, Injections, and Other medical devices
- **Dynamic Forms**: Type-specific form generation with appropriate fields and validation
- **Smart Calculations**: Automatic inventory calculations based on product type (strips, bottles, tubes, vials)

### 📦 Inventory Management
- **Real-time Tracking**: Live inventory updates with Firebase Firestore integration
- **Smart Search**: Real-time search functionality across all inventory items
- **Stock Alerts**: Automated low stock, near-expiry, and out-of-stock notifications
- **Batch Management**: Complete batch tracking with expiry date monitoring

### 📱 Invoice Processing
- **Camera Integration**: ML Kit-powered invoice scanning with text recognition
- **Automatic Data Extraction**: Parse invoice data and populate inventory automatically
- **PDF Generation**: Professional invoice generation with clinic branding
- **QR Code Support**: Generate and scan QR codes for quick product identification

### 📊 Sales & Reporting
- **Complete Sales Workflow**: From product selection to invoice generation
- **Multi-format Reports**: PDF and Excel export capabilities
- **Customer Reports**: Detailed medicine and customer reporting
- **Date Range Filtering**: Flexible reporting with custom date ranges

### 🔔 Alert System
- **Low Stock Alerts**: Automatic notifications when inventory falls below threshold
- **Expiry Management**: Near-expiry and expired product tracking
- **Comprehensive Dashboard**: Centralized alert management and monitoring

## 🛠️ Technical Architecture

### **Architecture Pattern**
- **MVVM (Model-View-ViewModel)** with Repository Pattern
- **Dependency Injection** for clean code organization
- **LiveData** for reactive UI updates
- **Coroutines** for asynchronous operations

### **Backend & Database**
- **Firebase Firestore** for real-time data synchronization
- **Firebase Authentication** for user management
- **Firebase Storage** for file management
- **Firebase ML Kit** for text recognition

### **UI/UX Technologies**
- **Material Design** components and guidelines
- **ViewBinding** for type-safe view access
- **Navigation Component** for seamless navigation
- **RecyclerView with Paging** for efficient list management
- **Custom Fonts** and theming

### **Additional Libraries**
- **CameraX** for camera functionality
- **PDFBox** for PDF generation
- **ZXing** for QR code generation and scanning
- **Gson** for JSON serialization
- **Dexter** for runtime permissions

## 📱 Screenshots

*[Add screenshots of key features here]*

## 🏗️ Project Structure

```
app/src/main/java/com/msp/clinicmangement/
├── activities/           # Activity classes
├── fragments/           # Fragment classes
├── viewmodel/           # ViewModel classes
├── repository/          # Repository pattern implementation
├── DataClass/          # Data models and entities
├── ui/                 # UI components and utilities
├── utils/              # Utility classes
├── di/                 # Dependency injection
└── core/               # Core functionality
```

## 🔧 Key Components

### **Data Models**
- `InventoryItem`: Comprehensive inventory item with dynamic fields
- `MedicineFormType`: Enum for different medicine categories
- `Sale`: Sales transaction model
- `ClinicInfo`: Clinic information and settings

### **Repository Layer**
- `InventoryRepository`: Inventory operations interface
- `FirebaseInventoryRepository`: Firebase implementation
- `SalesRepository`: Sales operations interface
- `FirebaseSalesRepository`: Firebase sales implementation

### **ViewModel Layer**
- `InventoryViewModel`: Inventory business logic
- `SalesViewModel`: Sales business logic
- `SalesListViewModel`: Sales list management

### **UI Components**
- `DynamicMedicineFormFragment`: Dynamic form generation
- `InventoryFragment`: Main inventory management
- `SalesFragment`: Sales processing
- `AlertFragment`: Alert management dashboard

## 🚀 Features in Detail

### **Dynamic Form System**
The application features a sophisticated dynamic form system that adapts to different medicine types:

- **Tablets/Capsules**: Tracks strips, units per pack, and individual tablet counts
- **Syrups/Liquids**: Manages bottles with volume specifications
- **Creams/Ointments**: Handles tubes with weight measurements
- **Injections**: Manages vials and injection forms
- **Other**: Flexible system for medical devices and miscellaneous items

### **Smart Inventory Calculations**
- Automatic unit price calculations based on product type
- Intelligent inventory counting (individual units vs. packages)
- Dynamic pricing for different selling units
- Comprehensive stock level monitoring

### **Advanced Search & Filtering**
- Real-time search across all product fields
- Filter by medicine type, stock status, and expiry dates
- Sort by various criteria (name, expiry, stock level)
- Pagination for large datasets

## 📈 Business Logic

### **Inventory Management**
- Multi-level inventory tracking (packages → individual units)
- Automated stock level calculations
- Expiry date monitoring and alerts
- Batch number tracking for traceability

### **Sales Processing**
- Dynamic pricing based on product type
- Quantity validation against available stock
- Automatic inventory deduction
- Professional invoice generation

### **Reporting System**
- Comprehensive sales reports with date filtering
- Inventory status reports
- Customer-specific medicine reports
- Export capabilities in multiple formats

## 🔒 Security & Data Management

- **Firebase Security Rules** for data protection
- **Input Validation** on all forms
- **Error Handling** with user-friendly messages
- **Data Backup** with Firebase integration
- **Offline Support** with local caching

## 🎯 Target Audience

- **Medical Clinics**: Small to medium-sized medical practices
- **Pharmacy Owners**: Independent pharmacy management
- **Healthcare Professionals**: Doctors and medical staff
- **Medical Supply Managers**: Healthcare facility administrators

## 📋 Requirements

- **Android 8.1 (API 27)** or higher
- **Camera** for invoice scanning functionality
- **Internet Connection** for Firebase synchronization
- **Storage Permission** for PDF generation and file management

## 🏆 Project Highlights

- **Clean Architecture**: Well-structured MVVM implementation
- **Scalable Design**: Easy to extend with new features
- **Modern Android**: Latest Android development practices
- **Real-time Sync**: Live data updates across devices
- **User-Friendly**: Intuitive interface for medical professionals
- **Comprehensive**: Complete solution for clinic management

---

*This project demonstrates expertise in Android development, Firebase integration, MVVM architecture, and complex business logic implementation for healthcare management systems.*
