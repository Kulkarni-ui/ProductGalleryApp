![image](https://github.com/user-attachments/assets/f88b3440-5c6d-43bd-b4dc-b1935c4e1aca)# 🛍️ React Product Gallery

A simple and interactive **React-based Product Gallery** that allows users to:

- 🔍 Search products by name  
- ➕ Add new products dynamically with image upload  
- 🗑️ Delete existing products  
- 🖼️ Preview uploaded images instantly  
- 🎨 Responsive and clean UI with grid layout

---

## 🚀 Features

- ✅ Real-time search filtering
- ✅ File upload support using `URL.createObjectURL`
- ✅ Dynamic product addition and deletion
- ✅ Responsive grid layout using Flexbox/Grid
- ✅ Component-based structure (`ProductGallery`, `ProductCard`)

---

## 🧱 Components

### `ProductGallery.jsx`
- Manages product state
- Handles image uploads
- Implements search functionality
- Renders `ProductCard` components

### `ProductCard.jsx`
- Displays product details: name, image, description, price
- Supports delete operation

---

## 🖼️ Image Handling

- Static images must be placed in `/public/images`
- Dynamically uploaded images are previewed using `URL.createObjectURL(file)`

---

## 💻 Installation & Run

```bash
npm install
npm start

---
## Folder Structure
src/
├── components/
│   ├── ProductGallery.jsx
│   └── ProductCard.jsx
public/
└── images/
    ├── smart-mirror.jpg
    ├── self-watering-pot.jpg
    └── mini-projector.jpg
---
📄 License
MIT License

