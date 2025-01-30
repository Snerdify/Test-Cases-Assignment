# 📌 Test Cases Assignment

## 📝 Generating Test Cases using Google Gemini

This repository contains a Colab notebook that utilizes **Google Gemini** to generate **manual test cases** based on up to **five screenshots** of a user journey on **Amazon**.

---

## 📌 Steps to Run in Google Colab

1. **Upload the screenshots** to the Colab environment.
2. **Run the notebook**, which will:
   - Read the screenshots in Python.
   - Use the available **Gemini model** (`1.5-flash`, `1.5-flash-8b`, or `1.5-flash-002`) to generate structured test cases.
   - Generate **three test cases per image** in the required format.
   - The coordinates of the UI elements in the screenshots
   - The cropped images of the UI elements in the screenshots
   - The highlighted UI elements 
3. **Save the output** in JSON format inside the `output-files` folder.

---

## 📸 Input Screenshots

The input consists of **five screenshots** from the Amazon website, covering different stages of the user journey:

1. **`amazon-home.png`** → Amazon home page.
2. **`amazon-search.png`** → Search results page while looking for a product.
3. **`product-details.png`** → Product details page after clicking a product.
4. **`add-to-cart.png`** → Sidebar where the user can add the product to the cart.
5. **`confirmation.png`** → Confirmation page after successfully adding the product to the cart.

---

## 📌 Test Case Format

Each generated test case follows this structured format:

```json
{
  "title": "Short and descriptive test case name",
  "objective": "Purpose of the test case (e.g., verifying user interactions, UI elements)",
  "steps": [
    {
      "action": "User action to perform (e.g., click a button, enter text)",
      "data": "(Optional) Input data required for the step",
      "expected_result": "Expected outcome after performing the action"
    }
  ]
}
```

🔹 **Each image generates 3 test cases.**

---

## 📂 Output

- The generated structured JSON output for the test-cases is stored in the `output-files` folder.
- You can also directly generate this file after running the code in the Colab notebook.
- I have also uploaded the description-json( descriptions of screenshots by gemini) file . [ This is a cleaned up json response , done manually]
---

## 🚀 Running the Notebook

To execute this project:

1. **Open Google Colab.**
2. **Clone this repository**:
   ```bash
   git clone https://github.com/your-username/Test-Cases-Assignment.git
   ```
3. **Navigate to the Colab notebook** and execute the cells.
4. **Download the JSON output** from `output-files` after completion.

---

## 💡 Notes

- Ensure that your API key is properly configured in Colab for Gemini API access.
- The Colab notebook automatically selects an available Gemini model for processing.
- The generated JSON test cases follow a structured format for ease of use.

---

🎯 **Happy Testing! 🚀**





