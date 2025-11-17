<div align="center">

# 🛒 Grocery Management System

![C++](https://img.shields.io/badge/C%2B%2B-17-blue?style=for-the-badge&logo=cplusplus&logoColor=white)
![OOP](https://img.shields.io/badge/OOP-Design-green?style=for-the-badge&logo=codeigniter&logoColor=white)
![File System](https://img.shields.io/badge/Binary-Files-orange?style=for-the-badge&logo=files&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)

<p align="center">
  <strong>🏪 A comprehensive Object-Oriented C++ solution for modern grocery store management</strong>
</p>

<p align="center">
  <em>Transforming manual grocery operations into automated, efficient business processes across Pakistan</em>
</p>

</div>

## 📋 Overview

A robust **C++ object-oriented software** designed for large grocery store companies transitioning from manual to automated processes. This system enhances both in-person and virtual shopping experiences with comprehensive inventory management, user authentication, and multi-role access control.

## 🏗️ System Architecture

```
📦 Grocery Management System
├── 👤 User Management (Admin, Manager, Customer)
├── 🏪 Store Management (Multi-location support)
├── 📦 Product Catalog (Food, Hygiene, Household)
├── 📊 Inventory System (Real-time tracking)
├── 🛒 Shopping Cart (Online experience)
└── 💳 Payment Gateway (Multiple options)
```

## ✨ Core Features

### 🔐 **1. User Registration & Authentication**

| Role | Registration | Access Level | Special Features |
|------|-------------|--------------|------------------|
| **👨‍💼 Admin** | Pre-configured | System-wide | Store & user management |
| **🏪 Manager** | Admin-only creation | Store-specific | Inventory control |
| **🛍️ Customer** | Self-registration | Shopping access | CNIC validation |

#### 🔑 **Security Requirements**
- **CNIC Validation**: 13-digit Pakistani CNIC verification
- **Password Policy**: 9 characters, 1 uppercase, 1 numeric
- **Duplicate Prevention**: Unique account enforcement
- **Error Handling**: Comprehensive validation feedback

### 🏪 **2. Multi-Store Management**
- **Nationwide Coverage**: Support for stores across Pakistan
- **Location-Based Assignment**: Managers assigned by geography
- **Cross-Store Visibility**: View inventory across all locations
- **Real-Time Synchronization**: Instant updates across the network

### 📦 **3. Product Catalog System**

<details>
<summary><strong>🍎 Food Categories</strong></summary>

#### **Perishable Goods**
- **🥩 Meat**: Chicken, Beef, Mutton, Fish
- **🥛 Dairy**: Milk, Eggs, Yogurt, Cheese  
- **🍎 Fruits**: Apple, Banana, Mango, Orange, Watermelon
- **🥕 Vegetables**: Tomato, Onion, Cucumber, Potatoes

#### **Non-Perishable Goods**
- **🍿 Snacks**: Chocolates, Chips, Biscuits
- **🌶️ Spices**: Various cooking spices
- **🌾 Grains**: Lentils, Wheat, Flour, Rice
- **🥣 Cereal**: Breakfast cereals

</details>

<details>
<summary><strong>🧴 Personal Hygiene</strong></summary>

- Shampoo, Soap, Hand Sanitizer
- Body care and personal wellness products

</details>

<details>
<summary><strong>🧽 Household Cleaning</strong></summary>

- Detergent, Dish Soap, Washroom Cleaner
- Home maintenance and cleaning supplies

</details>

### 📊 **4. Inventory Management**

| Feature | Description | Access Level |
|---------|-------------|--------------|
| **➕ Add Items** | Stock new products with quantities | Manager Only |
| **✏️ Update Stock** | Modify existing inventory levels | Manager Only |
| **❌ Remove Items** | Delete products from inventory | Manager Only |
| **🔍 Search Products** | Find items across all stores | Manager + View |
| **📋 View Inventory** | Browse store catalogs | Manager + View |

#### 🗄️ **File Structure**
```
Inventory Management/
├── Islamabad_Store.bin
├── Lahore_Store.bin
├── Karachi_Store.bin
└── [City]_Store.bin
```

### 🛒 **5. Online Shopping Experience**

| Step | Feature | Description |
|------|---------|-------------|
| **1** | 🔍 **Browse** | Explore product catalog |
| **2** | ➕ **Add to Cart** | Select items and quantities |
| **3** | ✅ **Checkout** | Review order summary |
| **4** | 💳 **Payment** | Choose payment method |
| **5** | 💬 **Feedback** | Rate shopping experience |

### 💳 **6. Payment Gateway Integration**

#### **Payment Options**
- 🚚 **Cash on Delivery (COD)**
  - Same city: +₨30 charges
  - Different city: +₨50 charges
- 💳 **Debit/Credit Cards**
- 📱 **Digital Wallets**
  - EasyPaisa
  - JazzCash

## 🔧 Technical Implementation

### **Object-Oriented Design**
```cpp
// Class Hierarchy
Product (Base Class)
├── Food
│   ├── Perishable
│   └── Non_Perishable
├── Hygiene
├── Household
├── Cart
└── Inventory

Person (Base Class)
├── Admin
├── Manager
└── Customer

Payment (Base Class)
├── COD
├── Card
├── EasyPaisa
└── JazzCash
```

### **File Management System**
- **Binary File Operations**: Efficient data storage and retrieval
- **Real-Time Updates**: Immediate persistence of changes
- **Categorized Storage**: Separate files for different product types
- **Data Integrity**: Consistent file handling across operations

## 🚀 Getting Started

### **Prerequisites**
- C++ Compiler (GCC 7.0+ or equivalent)
- Standard C++ Library
- File system access for data storage

### **Compilation & Execution**
```bash
# Compile the project
g++ -o grocery_system project.cpp

# Run the application
./grocery_system
```

### **Initial Setup**
1. **Admin Access**: Use predefined admin credentials
2. **Store Creation**: Set up initial store locations
3. **Manager Assignment**: Add store managers
4. **Product Catalog**: Populate initial inventory
5. **System Ready**: Begin operations

## 📁 Project Structure

```
Grocery-Management-System/
├── project.cpp                 # Main application (3,386 lines)
├── README.md                   # Project documentation
├── Data Files/
│   ├── admin.bin              # Admin credentials
│   ├── manager.bin            # Manager accounts
│   ├── customer.bin           # Customer accounts
│   └── ProductCatalog.bin     # Master product list
└── Inventory Management/       # Store-specific inventories
    ├── [Store]_inventory.bin  # Per-store inventory files
    └── ...
```

## 🎯 Business Benefits

| Benefit | Impact | Stakeholder |
|---------|--------|-------------|
| **Automated Operations** | Reduced manual errors | Management |
| **Real-Time Inventory** | Optimized stock levels | Store Managers |
| **Enhanced Experience** | Improved customer satisfaction | Customers |
| **Multi-Store Coordination** | Centralized oversight | Corporate |
| **Data-Driven Insights** | Better business decisions | All Users |

## 🛡️ System Security

- **Role-Based Access Control**: Hierarchical permission system
- **Data Validation**: Input sanitization and verification  
- **Secure Authentication**: Encrypted password storage
- **Audit Trail**: Transaction and modification logging
- **Error Handling**: Graceful failure management

## 📈 Scalability Features

- **Multi-Location Support**: Unlimited store additions
- **Modular Design**: Easy feature extensions
- **Efficient File I/O**: Optimized data operations
- **Memory Management**: Resource-conscious implementation
- **Cross-Platform Compatibility**: Standard C++ compliance

## 🤝 Contributing

We welcome contributions to enhance the grocery management system:

1. **Fork** the repository
2. **Create** a feature branch
3. **Implement** your changes
4. **Test** thoroughly
5. **Submit** a pull request

## 📄 License

This project is licensed under the **MIT License** - see the LICENSE file for details.

## 📞 Contact

<div align="center">

[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Abdul-SubhanCheema)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/abdulsubhan303)

<img src="https://user-images.githubusercontent.com/74038190/213910845-af37a709-8995-40d6-be59-724526e3c3d7.gif" width="100">

### 🛒 *"Bringing grocery management into the modern era, one feature at a time!"* ✨

**⭐ Enjoyed the project? Give it a star!**

</div>


