## Shopee scraper?
Shopee scraper1 will enable you to get more data from https://shopee.**[id|tw|vn|th|ph|my|sg|br|mx|co|cl|pl|es|in|ar]**.

Shopee can scrape:
- Scrape product details - You can scrape attributes like images, seller information, photos, time of listing and many more. You can find details below.
- Scrape search results - You can scrape for a specific search result by keyword.
- Scrape any categories with pagination
- Define maximum number of pages that needs to be scraped - If you only want to scrape first 3 pages, there is an option for that.
 

## How to scrape Shopee
It's easy to scrape site with Shoppe actor. Just follow these few steps and you'll get your data in a few minutes.

1. Click on Try for free.
2. Enter the keyword or enter a URL to start scraping.
3. Click on Run.
4. When Shoppe has finished, preview or download your data from the Dataset tab.

## Input Parameters

The input of this scraper should be JSON containing the list of pages on Realtor that should be visited. Required fields are:

| Field                | Type    | Description                                                                                                                                                                                               |
|----------------------|---------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| country              | Select  | You must specify from which site you want to scrape data.                                                                                                                                                 |
| keyword              | String  | (optional) Specific keyword what you want to scrape.                                                                                                                                                      |
| startUrl             | Array   | (optional) List of Shopee URLs. You should only provide property detail or search URLs                                                                                                                    |
| maxItems             | Integer | (optional) You can limit scraped products. This should be useful when you search through the big subcategories.                                                                                           |
| proxy                | Object  | Proxy configuration                                                                                                                                                                                       |

This solution requires the use of **Proxy servers**, either your own proxy servers or you can use [Apify Proxy](https://www.apify.com/docs/proxy).

### Compute Unit Consumption

The actor optimized to run blazing fast and scrape many as products as possible. Therefore, it forefronts all products detail requests. If actor doesn't block very often it'll scrape 70 products in 2 minutes with ~0.05-0.08 compute units.

## Results
```json
{
  "item": {
    "itemid": 13707866689,
    "brand": null,
    "brand_id": 0,
    "name": "Celana Panjang Jeans Pria / CELANA REGULAR | CELANA STANDAR | CELANA JEANS STANDAR | CELANA JEANS / CELANA JINS SETANDAR PANJANG REGULAR // ARMY DENIM",
    "product_url": "https://shopee.co.id/celana-panjang-jeans-pria-celana-regular-celana-standar-celana-jeans-standar-celana-jeans-celana-jins-setandar-panjang-regular-army-denim--i.354620922.13707866689",
    "description": "[COD] CELANA PANJANG JEANS | CELANA REGULER | CELANA STANDAR | CELANA JEANS STANDAR | CELANA JEANS | CELANA JEANS PANJANG REGULLER\n\nCELANA JEANS STD\nBAHAN :\n• SAKURATEX 13 OZ \n• • TEBAL\n• HALUS \nWARNA :\n• HITAM\n• NAVY\n• BLITZ\n\n\n\nDetail ukuran (ukuran : lingkar pinggang)\nSize 28 : 76-78 cm\nsize 29 : 78-80 cm\nSize 30 : 80-82 cm\nSize 31 : 82-84 cm \nSize 32 : 84-86 cm\nSize 33 : 86-88 cm \n\n[COD] CELANA PANJANG JEANS | CELANA REGULER | CELANA STANDAR | CELANA JEANS STANDAR | CELANA JEANS | CELANA JEANS PANJANG REGULLER\nUntuk stok mohon tanyakan terlebih dahulu karena bisa sewaktu waktu berubah dan untuk kenyamanan anatar pembeli dan penjual⚠️\nKENAPA HARUS BELANJA DI TOKO KAMI ?\n✔COD bayar di tempat\n✔Pengiriman CEPAT\n✔Harga MURAH\n✔Kualitas bahan dijamin BAGUS\n✔Jahitan konveksi RAPI\n✔TIDAK SESUAI barang bisa di kembalikan/tukar, dengan syarat foto/vidio produk yang salah di sertai ss rincian pesanan, lalu diskusikan chat ADMIN\n\nGambar hanya Sebagai referensi kemiripan gambar dengan aslinya hanya 90-95% (perbedaan bisa di sebabkan karena efek cahaya sa'at pemotretan, tinggi rendahnya iso hp yang di pakai pembeli, dan lainnya, harap maklum kalo ada ketidaksesuaian)\n\n#celanalevis505 #celanalevis #celanajeansstandar #celanajeans #celanaleviscowok #celanareguler #celanapanjangstandar #celanajeanspanjang"
  },
  "categories": {
    "category": "Pakaian Pria",
    "Subcategory_1": "Denim",
    "Subcategory_2": "Celana Jeans Panjang",
    "Subcategory_N": "Celana Panjang Jeans Pria / CELANA REGULAR | CELANA STANDAR | CELANA JEANS STANDAR | CELANA JEANS / CELANA JINS SETANDAR PANJANG REGULAR // ARMY DENIM"
  },
  "item_rating": {
    "rating_average": 4.921052631578948,
    "rating_count": [
      38,
      0,
      0,
      1,
      1,
      36
    ]
  },
  "price": {
    "price": 20000,
    "price_before_discount": 0,
    "price_max": 130000,
    "price_max_before_discount": -0.00001,
    "price_min": 20000,
    "price_min_before_discount": -0.00001,
    "raw_discount": 0,
    "discount": null,
    "discount_stock": 0,
    "product_sold": 1221
  },
  "shop": {
    "shop_location": "KAB. PEKALONGAN",
    "shopid": 354620922,
    "item_sold": 29,
    "item_stock": 4669
  },
  "images": [
    "https://cf.shopee.com.my/file/613bec5a4ed65dc8533794bf931d0154",
    "https://cf.shopee.com.my/file/5393cc0d15f840d6cd267fd837bef621",
    "https://cf.shopee.com.my/file/f4d4df22d5da6ef01e529c246408c829",
    "https://cf.shopee.com.my/file/fd216f419b96345bdb3e5f99a61b1119",
    "https://cf.shopee.com.my/file/92beccca5067881e7785fadcd21e9a59",
    "https://cf.shopee.com.my/file/21eaf90b9816c328d23a7711a01a07a4"
  ]
}
```

## Is it legal to scrape Shopee?
Note that personal data is protected by GDPR in the European Union and by other regulations around the world. You should not scrape personal data unless you have a legitimate reason to do so. If you're unsure whether your reason is legitimate, consult your lawyers. We also recommend that you read our blog post: [is web scraping legal?](https://blog.apify.com/is-web-scraping-legal/)
