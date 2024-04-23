import customtkinter
from tkinter import *

customtkinter.set_appearance_mode("dark")
customtkinter.set_default_color_theme("dark-blue")

janela = customtkinter.Ctk()
janela.geometry("700x400")
janela.title("Sistema de Login")
janela.resizable(False, False)

# Frame
frame = customtkinter.CtkFrame(master=janela, width=350, height=396)
frame.place(x=345, y=0)

# Frame widgets
label = customtkinter.CtkLabel(master=frame, text="Sistema de Login", text_font=("Roboto", 20))
label.place(x=25, y=5)

entry1 = customtkinter.CTkEntry(master=frame, placeholder_text="nome de usuario", width=300, text_font=("Roboto", 14))
entry1.place(x=25, y=105)
label1 = customtkinter.CTkLabel(master=frame, text="*O campo nome de usuário é obrigatório.", text_color="green", text_font=("Roboto", 8))
label1.place(x=25, y=135)

entry2 = customtkinter.CTkEntry(master=frame, placeholder_text="senha de usuario", width=300, text_font=("Roboto", 14))
entry2.place(x=25, y=175)
label2 = customtkinter.CTkLabel(master=frame, text="*O campo senha de usuário é obrigatório.", text_color="green", text_font=("Roboto", 8))
label2.place(x=25, y=205)

checkbox = customtkinter.CTKCheckBox(master=frame, text="Lembrar-se de mim sempre")
checkbox.place(x=25, y=235)

button = customtkinter.CTkButton(master=frame, text="Login", width=300)
button.place(x=25, y=285)

janela.mainloop()
