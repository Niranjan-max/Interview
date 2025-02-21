# Interview
interview for frontend support

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=2.0">
    <title>BOGO Offer</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #f8f9fa;
            margin: 0;
            padding: 20px;
        }
        .container {
            width: 341px;
            height: auto;
            position: absolute;
            top: 82px;
            left: 59px;
            padding: 20px;
            background: white;
            border-radius: 0px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }
        .offer-box {
            border: 2px solid #f3f3f3;
            padding: 15px;
            border-radius: 0px;
            margin-bottom: 10px;
            text-align: left;
            background: #fff;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        .most-popular {
            border: 2px solid #ff5eaa;
            position: relative;
            background: #fff4f7;
        }
        .most-popular::after {
            content: "MOST POPULAR";
            position: absolute;
            top: -12px;
            left: 10px;
            background: #ff5eaa;
            color: white;
            padding: 5px 10px;
            border-radius: 0px;
            font-size: 12px;
        }
        .price-container {
            text-align: right;
        }
        .price {
            font-weight: bold;
            color: black;
            display: block;
        }
        .strike-price {
            font-size: 12px;
            text-decoration: line-through;
            color: grey;
            display: block; /* Forces it to appear below the price */
        }
        .inline-strike {
            display: inline-block; /* Keeps Total section's strike price inline */
            margin-left: 5px;
        }
        .discount {
            background: #ff5eaa;
            color: white;
            padding: 2px 5px;
            border-radius: 0px;
            font-size: 12px;
            margin-left: 5px;
        }
        .add-to-cart {
            background: #ff5eaa;
            color: white;
            border: none;
            padding: 12px;
            width: 100%;
            border-radius: 0px;
            font-size: 18px;
            cursor: pointer;
            transition: 0.3s;
        }
        .add-to-cart:hover {
            background: #e05499;
        }
        select {
            padding: 5px;
            border-radius: 0px;
            border: 1px solid #ccc;
        }
        .free-delivery-total {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-top: 10px;
        }
        .total-price-container {
            display: flex;
            align-items: center;
            gap: 5px;
        }
    </style>
</head>
<body>
    <div class="container">
        <h2 style="color: #ff5eaa;">YAY! It's BOGO</h2>
        
        <div class="offer-box">
            <div>
                <input type="radio" name="offer" value="1" checked>
                <label>1 Unit <span class="discount">10% Off</span></label><br>
                <span style="color: black; font-size: 14px;">Standard Price</span>
            </div>
            <div class="price-container">
                <span class="price">$10.00 USD</span>
                <span class="strike-price">$24.00 USD</span> 
            </div>
        </div>
        
        <div class="offer-box most-popular">
            <div>
                <input type="radio" name="offer" value="2">
                <label>2 Unit <span class="discount">20% Off</span></label><br>
                Size: <select><option>S</option><option>M</option><option>L</option></select>
                Color: <select><option>Black</option><option>White</option><option>Red</option></select>
                <br>
                Size: <select><option>S</option><option>M</option><option>L</option></select>
                Color: <select><option>Black</option><option>White</option><option>Red</option></select>
            </div>
            <div class="price-container">
                <span class="price">$18.00 USD</span>
                <span class="strike-price">$24.00 USD</span> 
            </div>
        </div>
        
        <div class="offer-box">
            <div>
                <input type="radio" name="offer" value="3">
                <label>3 Unit <span class="discount">30% Off</span></label>
            </div>
            <div class="price-container">
                <span class="price">$24.00 USD</span>
                <span class="strike-price">$24.00 USD</span> 
            </div>
        </div>

        <div class="free-delivery-total">
            <strong style="color: #FF6B82;">Free Delivery</strong>
            <div class="total-price-container">
                <span style="color: black; font-size: 18px; font-weight: bold;">Total:</span>
                <span class="price">$18.00 USD</span>
            </div>
        </div>

        <button class="add-to-cart">+ Add to Cart</button>
    </div>
</body>
</html>
