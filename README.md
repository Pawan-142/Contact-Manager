# 📇 Contact Manager

A simple and efficient contact management application for storing, organizing, and managing your contacts.

## 📋 Overview

Contact Manager is a web-based application that allows you to create, read, update, and delete contacts with ease. Built with JavaScript, it provides a fast and responsive user experience.

---

## ✨ Features

- ✅ **Add Contacts**: Create new contact entries with name, email, and phone
- ✅ **View Contacts**: Display all contacts in an organized list
- ✅ **Search Contacts**: Quick search functionality
- ✅ **Edit Contacts**: Modify existing contact information
- ✅ **Delete Contacts**: Remove contacts with confirmation
- ✅ **Local Storage**: Persist contacts in browser local storage
- ✅ **Responsive Design**: Works on desktop and mobile devices
- ✅ **Sort Contacts**: Sort by name, email, or date added

---

## 🛠️ Tech Stack

| Component | Technology |
|-----------|-----------|
| **Frontend** | HTML5, CSS3, JavaScript |
| **Storage** | Browser LocalStorage |
| **Framework** | Bootstrap / Tailwind CSS |
| **Icons** | FontAwesome |

---

## 🚀 Getting Started

### Prerequisites
- Modern web browser (Chrome, Firefox, Safari, Edge)
- Text editor (VS Code, Sublime Text, etc.)

### Installation

1. **Clone the repository:**
```bash
git clone https://github.com/Pawan-142/Contact-Manager.git
cd Contact-Manager
```

2. **Open in browser:**
```bash
# Option 1: Direct file opening
open index.html

# Option 2: Using live server
npm install -g live-server
live-server
```

---

## 📁 Project Structure

```
Contact-Manager/
├── index.html          # Main HTML file
├── css/
│   └── style.css       # Stylesheet
├── js/
│   ├── main.js         # Main application logic
│   ├── contact.js      # Contact class/model
│   └── ui.js           # UI manipulation
└── assets/
    └── images/         # Images and icons
```

---

## 🎯 Usage

### Adding a Contact
1. Enter name, email, and phone number
2. Click "Add Contact" button
3. Contact appears in the list

### Searching Contacts
1. Type in the search box
2. Contacts filter in real-time

### Editing a Contact
1. Click "Edit" button on a contact
2. Modify the information
3. Click "Save" to update

### Deleting a Contact
1. Click "Delete" button
2. Confirm deletion
3. Contact is removed

---

## 💻 Code Examples

### Adding a Contact
```javascript
const addContact = (name, email, phone) => {
    const contact = {
        id: Date.now(),
        name: name,
        email: email,
        phone: phone,
        createdAt: new Date()
    };
    
    contacts.push(contact);
    saveToLocalStorage();
    renderContacts();
};
```

### Searching Contacts
```javascript
const searchContacts = (query) => {
    return contacts.filter(contact =>
        contact.name.toLowerCase().includes(query.toLowerCase()) ||
        contact.email.toLowerCase().includes(query.toLowerCase()) ||
        contact.phone.includes(query)
    );
};
```

---

## 💾 Data Structure

```javascript
{
    id: 1234567890,
    name: "John Doe",
    email: "john@example.com",
    phone: "+1-234-567-8900",
    createdAt: "2025-04-20T10:30:00Z"
}
```

---

## 🎨 User Interface

- **Header**: Application title and description
- **Input Form**: Fields for contact information
- **Search Bar**: Quick search functionality
- **Contact List**: All contacts displayed in cards/table format
- **Action Buttons**: Edit and Delete options for each contact

---

## 🔐 Data Privacy

- All contacts are stored **locally** in your browser
- **No data** is sent to external servers
- Clear browser storage to delete all contacts
- No account or login required

---

## 👨‍💻 Author

**Pawan-142**  
- GitHub: [@Pawan-142](https://github.com/Pawan-142)

---

**Last Updated**: 2026-06-14
