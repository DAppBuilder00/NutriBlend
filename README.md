# NutriBlend Smoothie Generator 🥤

A modern web-based smoothie recipe generator that allows users to create healthy smoothie recipes instantly and download them as PDF files.

---

## 🚀 Features

* 🍓 Generate healthy smoothie recipes
* 🧠 Dynamic recipe display
* 📄 Download recipes as PDF
* 📱 Responsive web design
* ⚡ Fast and lightweight
* 🎨 Modern UI design

---

## 🛠 Technologies Used

* HTML5
* CSS3
* JavaScript
* jsPDF Library

---

## 📦 Installation

1. Clone or download the project

```bash
git clone https://github.com/yourusername/nutriblend-smoothie-generator.git
```

2. Open the project folder

3. Run the project using:

* VS Code Live Server
* or open `index.html` directly in browser

---

## 📄 jsPDF Setup

This project uses the jsPDF library for exporting recipes as PDF files.

Add this script before your main JavaScript file:

```html
<script src="https://cdnjs.cloudflare.com/ajax/libs/jspdf/2.5.1/jspdf.umd.min.js"></script>
<script src="script.js"></script>
```

---

## 📁 Project Structure

```plaintext
NutriBlend/
│
├── index.html
├── style.css
├── script.js
└── README.md
```

---

## 🧩 Example PDF Download Function

```javascript
document
  .getElementById("downloadRecipe")
  .addEventListener("click", () => {

    const recipeText = smoothieResult.innerText;

    if (!recipeText || recipeText.includes("will appear here")) {
      alert("Please generate a smoothie first.");
      return;
    }

    const doc = new window.jspdf.jsPDF();

    const lines = doc.splitTextToSize(recipeText, 180);

    doc.text("NutriBlend Recipe", 10, 10);
    doc.text(lines, 10, 20);

    doc.save("NutriBlend-Recipe.pdf");
});
```

---

## 🎯 Future Improvements

* AI-generated smoothie recommendations
* Nutritional calculator
* Save recipe history
* Dark mode
* User accounts
* Export to DOCX
* Meal planning system

---

## 📸 Preview

Add screenshots of your app here.

---

## 🤝 Contributing

Contributions are welcome!

Fork the project and submit a pull request.

---

## 📜 License

This project is open-source and available under the MIT License.

---

## 👨‍💻 Author

Created by Westlie de los Santos.
