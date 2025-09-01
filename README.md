# Capstone-Project-Airbnb-Listing-Bangkok

# Link google slides Laporan Analisis: https://docs.google.com/presentation/d/1Yg2ywcFNlKzmN2J_T2gfgCcSPTV84ogef1MgAGicLNg/edit?usp=sharing

# Link Video penjelasan Laporan Analisis: https://youtu.be/3qI59GSjtgE

# Link Dashboard di Tableau Public: https://public.tableau.com/views/CapstoneProjectIvanTaufiqurrahmanAirbnbListingsBangkok/SummaryDashboard?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link

# Latar Belakang
Airbnb listing Bangkok adalah perusahaan pihak ketiga yang membantu menemukan orang yang ingin menyewa tempat di bangkok dengan orang yang memiliki tempat untuk disewa. Selama ini perusahaan tidak memiliki data yang kuat untuk mempetakan daerah potential yang sering di pilih sebagai tempat tinggal sementara dan perilaku customer terhadap tempat yang disewakan (jumlah, harga, tipe, waktu).

# Permasalahan
Perusahaan ingin mengetahui bagaimana cara perusahaan dan host yang ada di bangkok untuk beradapatasi dan mengakomodasi peningkatan permintaan akan tempat menginap di tahun depan dan juga membantu mempetakan daerah yang memiliki jumlah listing yang besar. Informasi ini dapat membantu perusahaan airbnb listing bangkok dalam mengoptimalkan daerah lain yang belum banyak memiliki tempat untuk disewakan di airbnb dan juga membantu meratakan pertumbuhan ekonomi di daerah lain di bangkok.

Permasalahan yang ingin diangkat pada kasus ini adalah:

**Bagaimana Airbnb listing di bangkok berusaha beradaptasi dan mengakomodasi peningkatan permintaan akan tempat untuk menginap di tahun 2023 kedepan, sekaligus tetap menjaga keseimbangan pertumbuhan listing di semua daerah di bangkok?**

# Tahapan
1. Data Preprocessing
   - Data Understanding dan Cleaning
2. Data Analysis
   - ## Supply Analysis
       - Treemap `Category Stay` in 2022 based on `Possible days` to book
       - Bar Chart `Room Type` Distribution based on `Possible days` to book
       - Pareto Chart `Neighbourhood` Domination based on `Possible days` to book
       - KPI section:
       - Lowest and Highest `average mean price` of `Neighbourhood`
       - `Maximum Possible days` in 2022
       - Top Host with most `Listings` in Bangkok
  - ## Demand Analysis
      - Treemap `Category Stay` in 2022 based on `booked_365` days
      - Bar Chart `Room Type` Distribution based on `booked_365` days
      - Pareto Chart `Neighbourhood` Domination based on `booked_365` days
      - KPI section:
      - Revenue in 2022
      - `Total Booked days` in 2022
      - Most Popular `Room Type` in 2022 for customer to choose
      - Most Popular `Category Stay` in 2022 for customer to choose
  - ## Summary
      - Bar Chart Comparison `booked days` in 2022 and from `2012-2021` based on `Category stay` and `Room Type`
      - KPI section:
      - Total `Revenue` all years
      - `Revenue` each year from 2012-2021
      - Total `Unique Listings`
      - Total `Unique Host`

3. Conclusion & Actionable Recommendation

## Software yang Digunakan  
- Python notebook ipynb  
- Tableau Public untuk visualisasi interaktif  
- google slides untuk membuat laporan Analisis berdasarkan visualisasi Tableau Public
- zoom untuk merekam video
- youtube untuk upload video laporan analisis

## 📑 Data Dictionary  

| Kolom                          | Deskripsi                                      | Tipe Data |
|--------------------------------|------------------------------------------------|-----------|
| id*                            | ID unik untuk setiap listing                   | Integer   |
| name                           | Nama listing                                   | String    |
| host_id*                       | ID unik untuk setiap host                      | Integer   |
| host_name*                     | Nama host                                      | String    |
| neighbourhood*                 | Nama wilayah di Bangkok                        | String    |
| latittude                      | koordinat garis lintang                        | float     |
| longitude                      | koordinat garis bujur                          | float     |
| number_of_reviews              | jumlah review yang diberikan                   | Integer   |
| calculated_host_listings_count | jumlah review yang dimiliki host               | Integer   |
| availability_365*              | jumlah hari yang masih tersedia di tahun 2022  | Integer   |
| number_of_reviews_ltm          | Jumlah review yang diberikan di tahun 2022     | Integer   |
| room_type*                     | Tipe kamar (Entire, Private, Shared, Hotel)    | String    |
| price*                         | Harga per malam                                | Float     |
| minimum_nights*                | Minimum malam menginap                         | Integer   |
| booked_365*                    | Jumlah hari terbooking di tahun 2022           | Integer   |
| occupancy_days*                | Total hari terbooking dari 2012–2021           | Integer   |
| category_stay*                 | Kategori lama menginap (Short, Medium, dll.)   | String    |


## Conclusion
- di tahun 2022 sendiri, revenue airbnb mencapai 2.7 Billion Baht tertinggi dari tahun tahun sebelumnya. 

- 14 wilayah atau neighbour mendominasi dari segi jumlah possible booked days dan juga booked days di tahun 2022 yang berarti semakin banyak listing di daerah tersebut, semakin banyak juga kemungkinan customer memilih daerah tersebut untuk menyewa tempat di bangkok.

- Customer preference kepada entire home/apt sebagai tempat untuk disewa dari tahun 2012-2022 memberikan gambaran bahwa customer yang datang ke bangkok dan ingin vacation sangat senang dengan tipe ini karena memberikan privasi lebih dibandingkan dengan room type lainnya.

- Customer times preference yang terjadi trend shift dari extended stay menjadi short stay dapat dijadikan bahan pembelajaran kepada host bahwa flexibility di minimum-nights adalah prioritas bagi customer.


## Actionable Recommendation
- Airbnb di bangkok masih dapat berkembang dari sisi potensi customer. perkembangan ini bisa lebih di maksimalkan dengan memberikan iklan yang dapat dilihat potential customer dan juga memberikan discount atau bonus untuk customer baru.

- Airbnb dapat memberikan incentive kepada host untuk membuka tempat baru untuk di sewa di daerah yang under-penetrated seperti cut percentage dikurangi sehingga host dapat mendapatkan untung lebih dari revenuenya.

- Airbnb dapat memberikan bonus atau discount untuk customer yang memilih room type lain selain entire home/apt atau bahkan memberikan sugesti kepada host baru untuk menyewakan tempat dengan tipe 1 rumah sekaligus dan tidak menyarankan bentuk/ tipe ruangan lainnya untuk disewakan berdasarkan customer behaviour ketika memilih tempat untuk ditinggali berdasarkan tipe ruangan.

- Airbnb dapat memberikan nasihat kepada host untuk mengurangi minimum night to book supaya listing yang host sewa memiliki kesempatan yang lebih besar untuk dipilih dan disewa customer. Atau kalau host sulit melakukan hal tersebut, Airbnb dapat memberikan customer discount ketika menyewa tempat dengan minimum nights tinggi atau lebih lama menempati tempat tersebut.
---
