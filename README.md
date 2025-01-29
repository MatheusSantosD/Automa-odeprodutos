# Automating Product Registration with Python

# Overview

This repository provides a streamlined solution for automating product registration tasks using Python and the pyautogui library. Whether you need to import large datasets or perform repetitive data entry in web-based systems, this project showcases how automation can significantly enhance productivity.

By leveraging a combination of structured data from CSV files and automation scripts, this code performs key tasks like logging into a system, navigating through forms, and registering products with precision.

import pyautogui
import time
import pandas as pd


tabela = pd.read_csv("produtos.csv")
print(tabela)



pyautogui.PAUSE = 1

# pyautogui.clike -> clicar
# pyautogui.write -> escrever
# pyautogui.press -> pressionar uma tecla





# Passo 1: Abrir o sistema da empresa
#    https://dlp.hashtagtreinamentos.com/python/intensivao/login

pyautogui.press('win')

pyautogui.write('edge')

pyautogui.press('enter')

pyautogui.write('https://dlp.hashtagtreinamentos.com/python/intensivao/login')
pyautogui.press('enter')


# pedir pro computador esperar 3 segundos
time.sleep(3)


# Passo 2: Fazer login

pyautogui.click(x=683, y=461)

pyautogui.write("pythonimpressionador@gmail.com")

pyautogui.press('tab')

pyautogui.write("hashtag")

pyautogui.click(x=951, y=647)



# Passo 3: importar a base de dados dos produtos

for linha in  tabela.index:

    pyautogui.click(x=656, y=306)
    
    pyautogui.write(str(tabela.loc[linha, "codigo"]))
    
    pyautogui.press('tab')
    
    pyautogui.write(str(tabela.loc[linha, "marca"])) 
    
    pyautogui.press('tab')
    
    pyautogui.write(str(tabela.loc[linha, "tipo"]))  
    
    pyautogui.press('tab')
    
    pyautogui.write(str(tabela.loc[linha, "categoria"]))
    
    pyautogui.press('tab')
    
    pyautogui.write(str(tabela.loc[linha, "preco_unitario"]))
    
    pyautogui.press('tab')
    
    pyautogui.write(str(tabela.loc[linha, "custo"]))
    
    pyautogui.press('tab')
    
    if not pd.isna(tabela.loc[linha, "obs"]): 
    
        pyautogui.write(str(tabela.loc[linha, "obs"]))


    pyautogui.click(x=854, y=622)
    
    pyautogui.scroll(5000)  
    


# Passo 4: cadastras 1 produto


for linha in tabela.index:

    pyautogui.click(x=668, y=305)
    
    pyautogui.write(str(tabela.loc[linha, "codigo"]))
    
    pyautogui.press('tab')
    



# Passo 5: Repetir o passo 4 até acabar todos os produtos

if not pd.isna(tabela.loc[linha, "obs"]):

    pyautogui.write(str(tabela.loc[linha, "obs"]))
    
    pyautogui.click(x=668, y=305)
    
    pyautogui.scroll(5000)
    
