# Scrollimport tkinter as tk
from tkinter import scrolledtext

def main():
    # Create the main window
    root = tk.Tk()
    root.title("Simple Scroll Example")

    # Create a ScrolledText widget
    text_area = scrolledtext.ScrolledText(root, wrap=tk.WORD, width=80, height=20)
    text_area.pack(padx=10, pady=10, fill=tk.BOTH, expand=True)

    # Add some sample text to demonstrate scrolling
    sample_text = "This is a sample text to demonstrate scrolling in Tkinter.\n" * 50
    text_area.insert(tk.END, sample_text)

    # Run the application
    root.mainloop()

if __name__ == "__main__":
    main()
