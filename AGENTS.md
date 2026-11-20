# CS234 Pixel Barki Project Rules (Mandatory for Codex)

Read `Pixel_Barki_DSA_Final_Project_2.pdf` in the workspace root before writing any code. Every single file generated or modified MUST strictly obey these constraints:

## 1. Tech Stack & Portability
- **Backend:** C++17 (`g++ -std=c++17 -pthread` on Linux, MinGW `g++` or MSVC `cl.exe` on Windows). Uses `"httplib.h"` (already located in `backend/httplib.h`) on port `8080` with CORS enabled.
- **Frontend:** Plain HTML, CSS, and Vanilla JavaScript inside `frontend/` (no React, Node, npm, or build frameworks).
- **Storage:** Pure binary files via `std::fstream` in `data/` (`canvas.bin`, `users.bin`, `history.log`, `config.bin`) and `snapshots/<time>.huf`. Zero SQL/NoSQL databases.

## 2. Strict Data Structure Rules (Zero STL Shortcuts)
- All 15 data structures and algorithms listed in the PDF table MUST be implemented manually from scratch in clean C++ header/source files inside `backend/`.
- **STRICTLY FORBIDDEN:** `std::stack`, `std::queue`, `std::priority_queue`, `std::list`, `std::map`, `std::unordered_map`, `std::set`, `std::unordered_set`, `std::sort`.
- **ALLOWED:** `std::string`, raw arrays, `std::vector` ONLY as a plain growable array, `<fstream>`, `<iostream>`, `<cstdint>`, `<cstring>`, `<ctime>`, `<thread>`, `<mutex>`, and `"httplib.h"`.

## 3. Student's Personal C++ Coding Style (Mandatory for Oral Viva)
- Write simple, beginner-friendly, transparent C++ code. No complex templates, lambdas, `auto` everywhere, or clever one-liners.
- Use classic `for (int i = 0; i < n; i++)` and `while` loops only. NEVER use range-based `for (auto x : y)` loops.
- Keep each function body as a clean, contiguous block of code with NO blank lines or comments inside function bodies, and exactly one blank line between function definitions.