# 🧮 Matrix Calculator App

A feature-rich React-based matrix calculator that allows users to **create**, **edit**, and **perform operations** on matrices, including support for **fractions** and **negative values** during input. Built for educational and practical matrix manipulation needs.

---

## ✨ Features

- 🔢 Create and name matrices (auto-naming support like `X1`, `X2`, etc.)
- 🧮 Perform matrix operations:
  - Addition
  - Subtraction
  - Multiplication
  - Transpose
  - Determinant
  - Inverse (if supported)
- 📝 Edit matrices with live updates
- ✅ Input support for:
  - Negative numbers
  - Fractions (e.g., `1/2`, `-3/4`)
- 🧼 Smart input handling: auto-normalizes invalid or partial values
- 📦 Stores original display values for UI clarity

---

## ⚙️ How It Works

### Matrix Creation

- Specify dimensions (max 10x10)
- Enter values manually, including fractional values (`"1/2"`) or negative numbers
- Leave cells empty or `"-"` to default to `0`

### Matrix Operations

Supports the following:

- ✅ **Add/Subtract:** Only if dimensions match
- ✅ **Multiply:** If `cols(A) == rows(B)`
- ✅ **Transpose:** Flips rows/columns
- ✅ **Determinant:** Only for square matrices
- ✅ **Inverse:** For non-singular square matrices

### Editing & Saving

- Click on an existing matrix to edit
- Save changes to update matrix values
- Inputs are parsed to numeric format on save

---

## 🧪 Input Handling & Parsing

Handles edge cases such as:

- `"-"` or `""` → `0`
- `"1/2"` → `0.5`
- `"abc"` → ignored or replaced by `0`

---



## 📊 Sample Result Structure

```json
{
  "type": "matrix",
  "name": "Result",
  "rows": 2,
  "cols": 2,
  "values": [[1, 2], [3, 4]]
}
```

or for scalar output (e.g., determinant):

```json
{
  "type": "scalar",
  "value": 10
}
```

---

## 🚀 Future Enhancements

- Export/import matrices
- Support for eigenvalues/eigenvectors
- Advanced formatting of fractional outputs
- History of operations

---

## 🧱 Built With

- [React.js](https://reactjs.org/)
- [Vite.js](https://vite.dev/)
- [TailwindCSS](https://tailwindcss.com/)
- Clean separation of UI logic and matrix math

---

## 🛡️ License

This project is licensed under the MIT License.

---

## 🙋‍♀️ Contribution

Email me at md.khaliduzzaman@bracu.ac.bd to contribute.


