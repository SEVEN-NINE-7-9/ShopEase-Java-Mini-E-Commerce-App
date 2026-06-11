# ShopEase — Java Mini E-Commerce App

## 📦 Features
- Browse a 10-product catalog with stock counts
- Add products to cart with quantity selection
- Real-time stock tracking (stock decreases on add, restores on remove)
- **Bulk discounts**: 5% off (qty ≥ 3) | 10% off (qty ≥ 5)
- **GST** at 18% applied on checkout
- Formatted **Tax Invoice** with invoice number & timestamp
- Remove items from cart
- Multi-class OOP design

## 🗂️ Classes
| Class | Responsibility |
|-------|----------------|
| `Product` | Stores product data + stock |
| `CartItem` | Product + quantity, computes discount |
| `Cart` | Manages cart items & totals |
| `ProductCatalog` | Holds inventory, handles stock changes |
| `BillGenerator` | Generates formatted tax invoice |
| `ShopEase` | Main class, menu & app flow |

## ▶️ How to Run

### Compile
```bash
cd src
javac *.java
```

### Run
```bash
java ShopEase
```

## 🧾 Sample Discount Logic
| Quantity | Discount |
|----------|----------|
| 1–2      | 0%       |
| 3–4      | 5%       |
| 5+       | 10%      |

GST (18%) is added on the discounted subtotal at checkout.
