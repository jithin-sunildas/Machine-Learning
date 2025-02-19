# 📊 Gantt Chart with Activity Codes

This project visualizes a **Gantt Chart** using **Matplotlib** and **Seaborn** in Jupyter Notebook. The project consists of two separate visualizations:

1. **Activity Codes Chart** - Maps activity codes to their respective tasks.
2. **Gantt Chart** - Uses activity codes instead of full task names to show task durations over time.

---

## 📂 Project Structure

- `gantt_chart.ipynb` - Jupyter Notebook containing the code to generate both charts.
- `README.md` - Project documentation.

---

## 📌 Dependencies

Ensure you have the following Python libraries installed:

```bash
pip install matplotlib seaborn pandas
```

Alternatively, if using Jupyter Notebook, install dependencies inside a cell:

```python
!pip install matplotlib seaborn pandas
```

---

## 📜 How to Use

1. Open **Jupyter Notebook** and run each cell sequentially.
2. **First Cell** generates the **Activity Codes Chart**.
3. **Second Cell** generates the **Gantt Chart with Activity Codes**.
4. Customize task names, durations, and start dates as needed.

---

## 📊 Output Example

### **Activity Codes Chart**
- A bar plot mapping **Activity Codes** to their respective tasks.

### **Gantt Chart**
- A timeline of activities with **Activity Codes** on the y-axis and corresponding task durations.

---

## 🛠 Customization

- Modify the `tasks` list in the code to change activities, start dates, and durations.
- Change the color scheme by modifying the `sns.color_palette("muted")[i % 6]` in the Gantt chart.

---

## 📄 License
This project is **open-source** and free to use or modify.

