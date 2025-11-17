CREATE DATABASE manga_store;

USE manga_store;

CREATE TABLE products (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(255) NOT NULL,
    price DECIMAL(10,2) NOT NULL,
    image_url VARCHAR(255) NOT NULL,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

-- ตัวอย่างสินค้า
INSERT INTO products (name, price, image_url) VALUES
('Naruto Vol.1', 250.00, '/images/naruto1.jpg'),
('One Piece Vol.1', 200.00, '/images/onepiece1.jpg'),
('Attack on Titan Vol.1', 300.00, '/images/aot1.jpg'),
('Demon Slayer Vol.1', 280.00, '/images/demonslayer1.jpg');

