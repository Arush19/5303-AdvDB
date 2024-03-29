## Homework 1

### Name:
    Gyaneshwar  Malba

### Ip Address
    192.241.140.57

### Phpmyadmin Link
    http://192.241.140.57/phpmyadmin

## Table Create statements

#### gift_options.sql

```sql
CREATE TABLE IF NOT EXISTS `gift_options` (
        `allowGiftWrap` BOOLEAN NOT NULL,
        `allowGiftMessage` BOOLEAN  NOT NULL,
        `allowGiftReceipt` BOOLEAN NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=latin1;
```

#### image_entities.sql

```sql
CREATE TABLE IF NOT EXISTS `image_entities` (
        `thumbnailImage` VARCHAR(149) NOT NULL,
        `mediumImage` VARCHAR(149) NOT NULL,
        `largeImage` VARCHAR(149) NOT NULL,
        `entityType` VARCHAR(9) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=latin1;
```

#### market_place_price.sql

```sql
CREATE TABLE IF NOT EXISTS `market_place_price` (
        `price` DOUBLE(6,2)NOT NULL,
        `sellerInfo` VARCHAR(44) NOT NULL,
        `standardShipRate` DOUBLE(5,2) NOT NULL,
        `twoThreeDayShippingRate` DOUBLE(6,2) NOT NULL,
        `availableOnline` BOOLEAN NOT NULL,
        `clearance` BOOLEAN NOT NULL,
        `offerType` VARCHAR(16) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=latin1;

```

#### products.sql

```sql
CREATE TABLE IF NOT EXISTS `products` (
        `itemId` INTEGER(9) NOT NULL,
        `parentItemId` INTEGER(9) NOT NULL,
        `name` VARCHAR(200) NOT NULL,
        `salePrice` DOUBLE(6,2) NOT NULL,
        `upc` VARCHAR(12) NOT NULL,
        `categoryPath` VARCHAR(123) NOT NULL,
        `shortDescription` VARCHAR(1112) NOT NULL,
        `longDescription` VARCHAR(5540)  NOT NULL,
        `brandName` VARCHAR(36) NOT NULL,
        `thumbnailImage` VARCHAR(149) NOT NULL,
        `mediumImage` VARCHAR(149) NOT NULL,
        `largeImage` VARCHAR(149) NOT NULL,
        `productTrackingUrl` VARCHAR(416) NOT NULL,
        `modelNumber` VARCHAR(53) NOT NULL,
        `productUrl` VARCHAR(345) NOT NULL,
        `categoryNode` VARCHAR(23) NOT NULL,
        `stock` VARCHAR(13) NOT NULL,
        `addToCartUrl` VARCHAR(221) NOT NULL,
        `affiliateAddToCartUrl` VARCHAR(296) NOT NULL,
        `offerType` VARCHAR(16) NOT NULL,
        `msrp` DOUBLE(7,2) NOT NULL,
        `standardShipRate` DOUBLE(5,2) NOT NULL,
        `color` VARCHAR(10) NOT NULL,
        `customerRating` VARCHAR(5) NOT NULL,
        `numReviews` INTEGER(5) NOT NULL,
        `customerRatingImage` VARCHAR(48)  NOT NULL,
        `maxItemsInOrder` INTEGER(6) NOT NULL,
        `size` VARCHAR(49) NOT NULL,
        `sellerInfo` VARCHAR(44) NOT NULL,
        `age` VARCHAR(14) NOT NULL,
        `gender` VARCHAR(6) NOT NULL,
        `isbn` VARCHAR(13) NOT NULL,
        `preOrderShipsOn` VARCHAR(19) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=latin1;
```
