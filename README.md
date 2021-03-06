<p align="center" >
<a href="#" align="center"> <img src="https://user-images.githubusercontent.com/13609011/84232431-3affaf80-ab2b-11ea-8ee7-7bbb77240e8c.jpeg" width="250" height="250" align="center"/></a>
</p>
<h1 align="center">
  Hyeonstagram Client </br>  <img alt="React" src="https://img.shields.io/badge/React-16.9.34-red.svg"> <img alt="Hooks" src="https://img.shields.io/badge/Hooks-0.5.0-blueviolet.svg"> <img alt="Apollo" src="https://img.shields.io/badge/React_Apollo-3.1.5-green.svg"> <img alt="platform" src="https://img.shields.io/badge/platform-Web-orange.svg">
</h1>

### ๐ฅ Motivation

> ์ธ์คํ๊ทธ๋จ์ ํด๋ก ์ฝ๋ฉํ๋ฉด์ React์ Hooks์ ๊น์ด ์๊ฒ ์ดํดํ๊ณ  GraphQL๊ณผ Prisma์ ๊ณต๋ถํ์ฌ ํ์คํ ๊ฐ๋ฐ์ ํ๊ธฐ ์ํด ํ๋ก์ ํธ๋ฅผ ์์ํ์์ต๋๋ค.


## ์๋น์ค ์๊ฐ

### [Instagram](https://www.instagram.com/) ํ์คํ ํด๋ก ์ฝ๋ฉ ํ๋ก์ ํธ
- ์จ๋ผ์ธ ์ฌ์ง ๊ณต์  ๋ฐ ์์ ๋คํธ์ํน ์๋น์ค
- ์ธ์คํ๊ทธ๋จ์ ํ๋ก ํธ์๋, ๋ฐฑ์๋ ๋ชจ๋ ํด๋ก  ์ฝ๋ฉํ์ฌ ์ฌ์ง ์๋ก๋, ํผ๋, Infinite Scroll, ํฌ์คํ/์ ์  ๊ฒ์, ๋๊ธ, ์ข์์, ํ๋ก์, Skeleton loading ๋ฑ ์ธ์คํ๊ทธ๋จ์ ์ฃผ์ ๊ธฐ๋ฅ๋ค์ ๊ตฌํํ์์ต๋๋ค.


## UI

### 1) ๋ฉ์ธ ํผ๋

![Feed mov](https://user-images.githubusercontent.com/13609011/84231891-21119d00-ab2a-11ea-86df-9fd15f30eb93.gif)

- ์ข์์ / ์ข์์ ์ทจ์
    - ์ข์์ ์ฟผ๋ฆฌ ์์ฒญ์ ๋ณด๋ด๊ธฐ ์  Frontend์์ ๋จผ์  ์ข์์ ์ฒ๋ฆฌ โ ๋ฐ์์๋ Up
- ๋๊ธ ์์ฑ
- ์ด๋ฏธ์ง ์ฌ๋ผ์ด๋ฉ
    - CSS translateX + transition ๋ฅผ ์ด์ฉํ์ฌ ์ฌ๋ผ์ด๋ฉ ๊ตฌํ

### 2) ๋ฌดํ ์คํฌ๋กค (Infinite scroll)

![Infinity Scroll mov](https://user-images.githubusercontent.com/13609011/84231909-2969d800-ab2a-11ea-8735-28393d38c753.gif)

- Infinity Scroll
    - Observer ๋ฅผ ์ด์ฉํด ๋งจ ์๋ ๊ฒ์๋ฌผ ๊ฐ์ง
    - โ ์๋ฒ์ offset๊ณผ limit ๋ฅผ parameter๋ก ์ ๋ฌํ์ฌ ์ถ๊ฐ ํผ๋ ๋ฐ์ดํฐ ๊ฐ์ ธ์ด
- ๋ง์ง๋ง ๊ฒ์๋ฌผ ๊ฒ์๋ฌผ ๋๋ฌ ์ ์๋ด ๋ฉ์ธ์ง
    - Toastify ์ฌ์ฉ

### 3) ํ์๊ฐ์ & ๋ก๊ทธ์ธ
<table>
   <tr>
     <th align="center">
       <img width="400" alt="1" src="https://user-images.githubusercontent.com/13609011/84231919-2e2e8c00-ab2a-11ea-9b4f-8c2f99061132.gif"/>
       <br><br>[ํ์๊ฐ์]
     </th>
     <th align="center">
       <img width="400" alt="2" src="https://user-images.githubusercontent.com/13609011/84231912-2bcc3200-ab2a-11ea-9542-711d59f6cad8.gif"/>
       <br><br>[๋ก๊ทธ์ธ] 
    </th>
  </tr>
</table>

- ์ด๋ฉ์ผ ์ธ์ฆ ์ฝ๋ ๋ฐฉ์ ๋ก๊ทธ์ธ
- ํ์๊ฐ์
    - Nodemailer ์ฌ์ฉ

### 4) Skeleton loading

<table>
   <tr>
     <th align="center">
       <img width="400" alt="1" src="https://user-images.githubusercontent.com/13609011/84231912-2bcc3200-ab2a-11ea-9542-711d59f6cad8.gif"/>
       <br><br>[ํผ๋]
     </th>
     <th align="center">
       <img width="400" alt="2" src="https://user-images.githubusercontent.com/13609011/84231936-34bd0380-ab2a-11ea-9949-9cae4adf19c6.gif"/>
       <br><br>[์ ์  ํ] 
    </th>
  </tr>
</table>

- ์ฟผ๋ฆฌ ๋ฐ์ดํฐ ๋ก๋ฉ
- ์ด๋ฏธ์ง ๋ฆฌ์์ค ๋ก๋ฉ

### 5) ์ ์  ํ

<table>
   <tr>
     <th align="center">
       <img width="400" alt="1" src="https://user-images.githubusercontent.com/13609011/84231933-338bd680-ab2a-11ea-9506-b359cbb1faba.gif"/>
       <br><br>[์ ์  ํ]
     </th>
     <th align="center">
       <img width="400" alt="2" src="https://user-images.githubusercontent.com/13609011/84231936-34bd0380-ab2a-11ea-9949-9cae4adf19c6.gif"/>
       <br><br>[๋ฐ์ํ] 
    </th>
  </tr>
</table>


- ๊ฒ์๊ธ ๋ง์ฐ์ค hover์ ์ข์์, ๋๊ธ ์ค๋ฒ๋ ์ด
- ๋ถ๋ถ ๋ฐ์ํ ๋์์ธ (๊ฒ์๊ธ ์ฌ์ด gap)
    - ๋ฏธ๋์ด ์ฟผ๋ฆฌ ์ด์ฉ

### 6) Following & Unfollowing
<table>
   <tr>
     <th align="center">
       <img width="400" alt="1" src="https://user-images.githubusercontent.com/13609011/84231904-27077e00-ab2a-11ea-92f8-905738e872f8.gif"/>
       <br><br>[Following]
     </th>
     <th align="center">
       <img width="400" alt="2" src="https://user-images.githubusercontent.com/13609011/84231927-31c21300-ab2a-11ea-8602-14d9c73283c7.gif"/>
       <br><br>[Unfollowing] 
    </th>
  </tr>
</table>


- ํผ๋์ Following ํ ์ฌ๋๋ค์ ๊ฒ์๋ฌผ๋ง ๋ณด์ฌ์ง
- Unfollow ํ๋ฉด ํผ๋์ ํด๋น ์ฌ๋์ ๊ฒ์๋ฌผ์ด ์ฌ๋ผ์ง


## ํ์ฉ๊ธฐ์ 
- **[Hooks]()**: ํจ์ํ ์ปดํฌ๋ํธ์ React State์ ์๋ช์ฃผ๊ธฐ ๊ด๋ฆฌ๋ฅผ ๋์์ฃผ๋ ๋ชจ๋๋ก ๊ธฐ์กด์ ํจ์ํ ์ปดํฌ๋ํธ์์ ํ  ์ ์์๋ ๋ค์ํ ์์์ ํ  ์ ์๊ฒ ๋์์ค๋๋ค. (ํด๋์คํ ์ปดํฌ๋ํธ ๊ธฐ๋ฅ ๊ฑฐ์ ๋๋ถ๋ถ์ ๋์ฒด๊ฐ๋ฅ)
- **[Styled-component]()**: CSS ํ์ผ ์์ด ์๋ฐ์คํฌ๋ฆฝํธ ์์์ CSS ์์์ ํ  ์์๊ฒ ๋์์ฃผ๋ ๋ชจ๋๋ก HTML element + CSS + Javascript ์ฝ๋๋ฅผ Component๋ก ์บก์ํ์์ผ ์ฝ๋๋ฅผ ๊ด๋ฆฌํ๊ธฐ ์ฉ์ดํ๋๋ก ๋์์ค๋ค. (ํด๋์ค ๊ธฐ๋ฐ Component ์คํ์ผ๋ง ๋์ฒด)
- **[Apollo]()**: GraphQL์ ํด๋ผ์ด์ธํธ ๋ผ์ด๋ธ๋ฌ๋ฆฌ ์ค ํ๋๋ก GraphQL ์ํ ๊ด๋ฆฌ ํ๋ซํผ์๋๋ค.
- **[Axios]()**: ํ์ผ ์๋ก๋๋ฅผ ์ฒ๋ฆฌํ๊ธฐ ์ํด ๋์ํ HTTP ํด๋ผ์ด์ธํธ ๋ผ์ด๋ธ๋ฌ๋ฆฌ๋ก์จ, ๋น๋๊ธฐ ๋ฐฉ์์ผ๋ก Node.js ์๋ฒ์ HTTP ๋ฐ์ดํฐ ์์ฒญ์ ์คํํฉ๋๋ค. (ํ์ผ ๊ด๋ฆฌ์ ์์ด์๋ RESTfull ๋ฐฉ์์ด GraphQL ๋ฐฉ์๋ณด๋ค ํจ๊ณผ์ )
- **[Sass]()**: CSS์ ์ ์ง๋ณด์์ ๋ถํธํจ์ ๊ฐ์ ํ์ฌ ํจ์จ์ ์ธ ์คํ์ผ๋ง์ ๋์์ฃผ๋ ๋ผ์ด๋ธ๋ฌ๋ฆฌ์๋๋ค.
- **[Intersection Observer]()**: ๊ธฐ์กด Scroll Event๋ก Infinite Scroll์ ๊ตฌํํ๋ฉด ์๋ฆฌ๋จผํธ์ offset์ ๊ตฌํ๊ธฐ ์ํด ๋ถํ์ํ ํจ์ ํธ์ถ๊ณผ ๋งค๋ฒ layout์ ์๋ก ๊ทธ๋ ค ์ฑ๋ฅ์ ๋ฌธ์ ๊ฐ ๋ฐ์ํ๊ฒ ๋๋ ๋ฐ, Intersection Observer๋ ํ๊ฒ ์๋ฆฌ๋จผํธ์, ํ๊ฒ ์๋ฆฌ๋จผํธ์ ๋ถ๋ชจ๋ ๋ทฐํฌํธ๊ฐ ๊ต์ฐจํ๋ ๋ถ๋ถ์ ๋ณํ๋ฅผ ๋น๋๊ธฐ์ ์ผ๋ก ๊ด์ฐฐํ์ฌ ์ด๋ฌํ ๋ฌธ์ ์ ์ ํด๊ฒฐํด์ค๋ค.
- **[Toastify]()**: Notification, Alert๋ฅผ ์ฝ๊ณ  ์์๊ฒ ์ฒ๋ฆฌํ๋๋ก ๋์์ค๋ค.

