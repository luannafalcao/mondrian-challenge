# CSS Grid Mondrian Challenge

This project is a front-end study that recreates Piet Mondrian’s painting  
**_Composition No. III with Red, Blue, Yellow and Black_ (1929)** using only **HTML & CSS Grid**.

The exercise explores proportions, line thickness, and responsiveness in a minimalist layout, showing how code can interpret and honor the structure of a real painting.

🌐 [View the live project here](https://luannafalcao.github.io/mondrian-challenge/)

---

## 🎨 About the Artwork
Piet Mondrian (1872–1944) was a Dutch painter and one of the founders of *De Stijl*.  
His works reduce painting to essential elements: straight lines, right angles, and primary colors.  
This challenge translates those ideas into CSS rules.

Reference image:  
![Mondrian Composition No. III](https://www.christies.com/img/LotImages/2015/NYR/2015_NYR_03736_0006C_000(piet_mondrian_composition_no_iii_with_red_blue_yellow_and_black_1929090924).jpg?maxwidth=1010&maxheight=650)

---

## 🛠️ Goal
- Recreate the composition using **CSS Grid only**
- Control black line thickness via `gap` + `padding`
- Ensure responsiveness with `aspect-ratio`

---

## 📐 Approach
- Defined **fractional `grid-template-columns` and `grid-template-rows`** based on the painting’s proportions
- Used **`gap` + `padding`** on the container to simulate thick black lines
- Positioned blocks with `grid-column` / `grid-row`

---

## 💻 Technical Details (challenge code only)

### HTML
```html
<div class="mondrian">
  <div class="item1"></div>
  <div class="item2"></div>
  <div class="item3"></div>
  <div class="item4"></div>
  <div class="item5"></div>
  <div class="item6"></div>
  <div class="item7"></div>
  <div class="item8"></div>
</div>
```

### CSS
```CSS
.mondrian {
  display: grid;
  grid-template-columns: 4.64fr 2.64fr 2.64fr 0.67fr;
  grid-template-rows: 9.16fr 2.91fr 3.48fr 0.45fr;
  gap: 10px;
  background-color: rgb(0, 0, 0);
  aspect-ratio: 1 / 1;
  box-shadow: -4px 5px 7px 1px rgba(0, 0, 0, 0.1), 0 2px 4px rgba(0, 0, 0, 0.1);
  max-width: 600px;
  margin: 0 auto;
}

.item1 { grid-column: 1 / 2; grid-row: 1 / 2; background-color: #e42c20; }
.item2 { grid-column: 2 / 5; grid-row: 1 / 2; background-color: #eeeeee; }
.item3 { grid-column: 1 / 2; grid-row: 2 / 5; background-color: #ebece7; }
.item4 {grid-row: 2 / 4; grid-column: 2 / 4; background-color: #eef1e6;}
.item5 {grid-column: 4 / 5; grid-row: 2 / 3; background-color: #144594;}
.item6 {grid-row: 3 / 5; background-color: #e9eae5; border-top: 6px solid #000;}
.item7 {grid-row: 4 / 5; background-color: #fbd721;}
.item8 {grid-row: 4 / 5; background-color: #242225;}
```

## 📜 License

This project is for educational purposes.

Artwork reference © Piet Mondrian.

Code © 2025 by Luanna 
