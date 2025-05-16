PDF Search Engine with GUI

==========================

A simple **PDF Search Engine GUI** application built with **Python**, **Tkinter**, **Whoosh**, and **PyPDF**. It allows users to **index and search PDF files** based on their content using full-text search. This project was created as part of an **Information Retrieval course final project**.

🚀 Features

-----------

-   ✅ Indexes all PDF files in a selected directory

-   ✅ Full-text extraction from PDFs using pypdf

-   ✅ Search UI built with tkinter

-   ✅ Displays ranked results with:

    -   File name

    -   Snippet of matched text

    -   Relevance score

-   ✅ Multithreaded indexing and search (no UI freeze)

-   ✅ Styled GUI with status bar and result panel

-   ✅ Uses Whoosh with stemming analyzer for indexing and searching

🛠️ Technologies Used

---------------------

-   **Python 3**

-   **Tkinter** - GUI Framework

-   **PyPDF** - PDF text extraction

-   **Whoosh** - Full-text indexing and search

-   **NLTK** *(partially planned)* - Natural Language Processing (lemmatization, stopword removal, etc.)

📂 Folder Structure

-------------------

```

.

├── main.py                 # Main GUI and search/index logic

├── whoosh_index/          # Directory where search index is stored

├── D:\books\              # Default folder where PDF files are read from

```

> 🔸 You can change the BOOKS_DIR path in the script or use the "Change Dir" button in the UI.

🧠 How It Works

---------------

### Indexing

-   Extracts text from each page of each PDF

-   Indexes the full content of the file using Whoosh

-   Uses stemming to improve recall during search

### Searching

-   User inputs a query

-   Results are fetched from the index

-   Displays matching file name, a highlighted snippet, and a score

🖥️ GUI Preview

---------------

-   📂 Select PDF directory

-   🔍 Input search query

-   ⚡ Index and search operations run in background threads

-   📜 Scrollable results box with highlights and scores

❌ Limitations (To Be Implemented)

---------------------------------

These are required to fully satisfy the IR course project requirements:

-   ❌ PDF: Does not show page numbers of matched text

-   ❌ TXT, CSV, Excel (.xlsx), JSON, Web pages: Not supported yet

-   ❌ No advanced NLP preprocessing (stopword removal, lemmatization, etc.)

-   ❌ Query operators like AND, OR, fuzzy (~), wildcards (*) not supported yet

-   ❌ No dropdown to filter file types

-   ❌ Evaluation metrics like Precision, Recall, F1-score not implemented

📅 Deadline & Context

---------------------

-   This project was developed for the **Information Retrieval course**

-   **Deadline**: May 17, 2025

📌 Requirements

---------------

Install dependencies:

```

pip install whoosh pypdf nltk

```

> You may also need to download NLTK resources if preprocessing is added later.

📦 How to Run

-------------

```

python main.py

```

-   Default directory is D:\books

-   Use the GUI to:

    -   Index files

    -   Enter and submit search queries

📜 License

----------

This project is created for **educational purposes** and may be extended freely.
