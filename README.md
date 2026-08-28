# 🧮 Calcuseless — The Most Inefficient Calculator Ever Built

**Calcuseless** is an experimental Python calculator written entirely using a single giant `match / case` statement. 

Instead of dynamically evaluating mathematical expressions, it hardcodes every possible calculation in advance.

---

## 📊 Benchmarks & Scaling Limits

| Version | Range | Code Lines | File Size | Execution / Parser Status |
| :--- | :--- | :--- | :--- | :--- |
| **Lite** | `0 - 100` | ~40,000 | ~1.2 MB | 🟢 Works instantly |
| **PRO** | `0 - 1,000` | ~4,000,000 | ~224 MB | 🟡 Slow load, GitHub LFS required |
| **ULTRA** | `0 - 10,000` | ~400,000,000 | **22.4 GB** | 🔴 **Crashes VS Code & Python AST (MemoryError)** |

---

## 💥 The ULTRA Experiment (10,000 Range)

- **Generation Time:** 583 seconds (~9.7 minutes)
- **Lines of Code:** 400,000,000+
- **File Size:** ~22.4 GB
- **Result:** Opened for ~1 second before Python process terminated with `MemoryError`. Successfully crashed VS Code syntax indexer.

*(Insert screenshot of the 22.4 GB file properties here)*

---

## 🛠️ How to Generate Locally

To generate your own local stress-test file:

```bash
python generator.py
