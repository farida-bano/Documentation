This is a [Next.js](https://nextjs.org) project bootstrapped with [`create-next-app`](https://nextjs.org/docs/app/api-reference/cli/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/app/building-your-application/optimizing/fonts) to automatically optimize and load [Geist](https://vercel.com/font), a new font family for Vercel.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/app/building-your-application/deploying) for more details.

            DAY 2 PLANNING THE TECHNICAL FOUNDATION

                                                          Objective:

The purpose of this code is to define basic data structures for an e-commerce system. These schemas model products, orders, and delivery zones so that:
1.	Product: Details of products (like id, name, price, stock, category, etc.) can be stored and managed.
2.	Order: Customer orders and their details (such as customer info, order items, status, total amount) can be tracked.
3.	Delivery Zone: Delivery zones and their drivers can be managed to ensure smooth delivery operations.
Objective: To organize structured data for an e-commerce system, enabling products to be sold, orders to be tracked, and deliveries to be managed efficiently.


Key Points from the Code (Schemas.ts)
1.	Product Schema:

o	id: Unique identifier for the product.
o	name: Name of the product.
o	price: Price of the product.
o	stock: Number of items available in stock.
o	category: Product category (can be 'women', 'men', or 'kids').
o	size (optional): Available sizes (e.g., 'S', 'M', 'L', 'XL').
o	color (optional): Available colors.
o	description (optional): Product description.
o	imageUrl (optional): URL for the product image.

2.	Order Schema:

o	CustomerInfo: Includes customer details like name, email, phone (optional), and address.
o	OrderItem: Represents a single product in the order, with fields like productId, quantity, and price.


o	Order: 
	orderId: Unique order identifier.
	customerInfo: Customer's details.
	orderDetails: List of items ordered.
	status: Order status (e.g., 'Pending', 'Processing', 'Shipped', 'Delivered', 'Cancelled').
	orderDate: Date when the order was placed.
	totalAmount: Total amount of the order.


3.	Example Order:

o	A customer named John Doe orders 2 units of a product (Floral Summer Dress) and 1 unit of another product, resulting in a total order amount of $129.97.

4.	Delivery Zone Schema:

o	CoverageArea: Specifies a city and a list of postal codes covered by a delivery zone.
o	AssignedDriver: Information about a delivery driver, including driverId, name, and contact.
o	DeliveryZone: 
	zoneName: Name of the delivery zone.
	coverageArea: Area covered by the delivery zone.
	assignedDrivers: List of drivers assigned to this zone.

5.	Example Delivery Zone:

o	A zone called "North City Zone" covers the city of 'North City' and includes postal codes ['12345', '12346', '12347'].
o	Two drivers are assigned: Alice Johnson and Bob Smith.

Exported Entities:
•	Product, Order, and DeliveryZone schemas are exported for use in other parts of the codebase.

 
 


 
I would like to express my heartfelt thanks to Sir Ameen Aalam for giving us students the opportunity to use our potential. We often step forward towards challenges, sometimes in different directions, as the doors of opportunities open before us. My prayers are with all of you for the acceptance of your hard work. May Allah bless your efforts and grant success for our families, our country, and our nation. Ameen.



