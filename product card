import React, { useState } from "react";

const ProductCard = ({ product, index, updateProduct, deleteProduct }) => {
  const [isEditing, setIsEditing] = useState(false);
  const [updatedProduct, setUpdatedProduct] = useState(product);

  const handleSave = () => {
    updateProduct(index, updatedProduct);
    setIsEditing(false);
  };

  return (
    <div style={{ border: "1px solid black", padding: "10px", textAlign: "center" }}>
      {isEditing ? (
        <div>
          <input type="text" value={updatedProduct.name} onChange={(e) => setUpdatedProduct({ ...updatedProduct, name: e.target.value })} />
          <input type="text" value={updatedProduct.description} onChange={(e) => setUpdatedProduct({ ...updatedProduct, description: e.target.value })} />
          <input type="text" value={updatedProduct.price} onChange={(e) => setUpdatedProduct({ ...updatedProduct, price: e.target.value })} />
          <button onClick={handleSave}>Save</button>
        </div>
      ) : (
        <>
          <img src={product.image || "https://via.placeholder.com/150"} alt={product.name} style={{ width: "100px", height: "100px", cursor: "pointer" }} onClick={() => setIsEditing(true)} />
          <h3>{product.name}</h3>
          <p>{product.description}</p>
          <p>${product.price}</p>
          <button onClick={() => deleteProduct(index)}>Delete</button>

        
        </>
      )}
    </div>
  );
};

export default ProductCard;
