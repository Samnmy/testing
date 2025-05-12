## Functionalities

1.  *Add Products:* Add new products to the inventory with their name, price, and quantity. If a product with the same name already exists, its quantity will be updated.
2.  *Consult Products:* Search for a product by its name and display its current details (price and quantity).
3.  *Update Product Prices:* Modify the price of an existing product.
4.  *Delete Products:* Remove a product from the inventory after a confirmation prompt.
5.  *Calculate Total Inventory Value:* Compute and display the sum of (price * quantity) for all products in the inventory, showing the total and a breakdown for each item.

## Acceptance Criteria Met

* *Initial Products:* The program initializes with at least 5 pre-added products when it starts.
* *Product Consultation:* If a product is not found during consultation, a clear "not found" message is displayed.
* *Price Update Validation:* New prices must be positive numbers. The system validates this input.
* *Product Deletion Confirmation:* Before deleting a product, the system asks for confirmation.
* *Total Inventory Value Precision:* The total inventory value is calculated precisely and displayed with two decimal places.
* *Code Structure and Comments:* The code is well-structured into functions for each operation and includes explanatory comments.
* *Language:* All code and comments are 100% in English.

## How to Run the Program

1.  *Save the code:* Save the provided Python code into a file named inventory_manager.py.
2.  *Open a terminal or command prompt:* Navigate to the directory where you saved the inventory_manager.py file.
3.  *Execute the script:* Run the program using the Python interpreter:

    ```bash
    python inventory_manager.py
    ```

4.  *Interact with the menu:* Follow the on-screen instructions to choose from the available options (add, consult, update price, delete, calculate total value, or exit).

## Usage Examples (Input and Output)

Below are examples of how to interact with the system and the expected outputs.

### 1. Start of the Program (Initial Products)

When you start the program, some products are automatically added to the inventory as default values.

* *Entrance:*

(No user interaction, executed automatically when calling main())

* *Exit:*

Product 'Computer monitor' added/updated successfully.
Product 'Computer case' added/updated successfully.
Product 'Motherboard' added/updated successfully.
Product 'RAM' added/updated successfully.
Product 'Graphics card' added/updated successfully.
Product 'hard disk SSD' added/updated successfully.
--- Inventory Management System ---
* Add Product
* Consult Product
* Update Product Price
   4.DeleteProduct
* Calculate Total Inventory Value
   6.Exit
Enter your choice:

---

### 2. Option 1: Add a New Product

* *Entrance:*

Enter your choice: 1
Enter product name: Keyboard
Enter product price: 75000.50
Enter product quantity: 20

* *Exit:*

Product 'Keyboard' added/updated successfully.
--- Inventory Management System ---
* Add Product
* Consult Product
* Update Product Price
   4.DeleteProduct
* Calculate Total Inventory Value
   6.Exit
Enter your choice:

---

### 3. Option 1: Update the Quantity of an Existing Product

(Note: The original RAM amount was 30, now it is 30 + 10 = 40)

* *Entrance:*

Enter your choice: 1
Enter product name: ram
Enter product price: 80000.45
Enter product quantity: 10

* *Exit:*

Product 'ram' already exists. Updating quantity.
Product 'ram' added/updated successfully.
--- Inventory Management System ---
* Add Product
* Consult Product
* Update Product Price
   4.DeleteProduct
* Calculate Total Inventory Value
   6.Exit
Enter your choice:

---

### 4. Option 1: Invalid Entry When Adding Product (Price)

* *Entrance:*

Enter your choice: 1
Enter product name: Mouse
Enter product price: abc

* *Exit:*

Invalid input. Price must be a number and quantity an integer.
--- Inventory Management System ---
* Add Product
* Consult Product
* Update Product Price
   4.DeleteProduct
* Calculate Total Inventory Value
   6.Exit
Enter your choice:

---

### 5. Option 2: Consult an Existing Product

* *Entrance:*

Enter your choice: 2
Enter product name to consult: Graphics Card

* *Exit:*

Product Details for 'Graphics Card'

Name: Graphics Card Price: $4000000.12 Quantity: 40
--- Inventory Management System ---
* Add Product
* Consult Product
* Update Product Price
   4.DeleteProduct
* Calculate Total Inventory Value
   6.Exit
Enter your choice:

---

### 6. Option 2: Consult a Non-Existing Product

* *Entrance:*

Enter your choice: 2
Enter product name to consult: Curved monitor

* *Exit:*

Product 'Curved Monitor' not found in inventory.
--- Inventory Management System ---
* Add Product
* Consult Product
* Update Product Price
   4.DeleteProduct
* Calculate Total Inventory Value
   6.Exit
Enter your choice:

---

### 7. Option 3: Update the Price of a Product

* *Entrance:*

Enter your choice: 3
Enter product name to update price: computer monitor
Enter new price: 620000.00

* *Exit:*

Price for 'computer monitor' updated from $600000.85 to $620000.00.
--- Inventory Management System ---
* Add Product
* Consult Product
* Update Product Price
   4.DeleteProduct
* Calculate Total Inventory Value
   6.Exit
Enter your choice:

---

### 8. Option 4: Delete a Product (Confirming Deletion)

* *Entrance:*

Enter your choice: 4
Enter product name to delete: Keyboard
The product 'Keyboard' exists
Are you sure you want to delete 'Keyboard' with a price of '75000.5' and with '20' quantities? (yes/no): yes

* *Exit:*

Product 'Keyboard' deleted successfully.
--- Inventory Management System ---
* Add Product
* Consult Product
* Update Product Price
   4.DeleteProduct
* Calculate Total Inventory Value
   6.Exit
Enter your choice:

---

### 9. Option 4: Delete a Product (Cancelling Deletion)

* *Entrance:*

Enter your choice: 4
Enter product name to delete: Hard Disk SSD
The product 'Hard Disk SSD' exists
Are you sure you want to delete 'Hard Disk SSD' with a price of '100000.14451' and with '35' quantities? (yes/no): no

* *Exit:*

Deletion of 'Hard Disk SSD' cancelled.
--- Inventory Management System ---
* Add Product
* Consult Product
* Update Product Price
   4.DeleteProduct
* Calculate Total Inventory Value
   6.Exit
Enter your choice:

---

### 10. Option 4: Try to Delete a Non-Existing Product

* *Entrance:*

Enter your choice: 4
Enter product name to delete: Mouse

* *Exit:*

The product 'Mouse' does not exist
Product 'Mouse' not found in inventory. Cannot delete.
--- Inventory Management System ---
* Add Product
* Consult Product
* Update Product Price
   4.DeleteProduct
* Calculate Total Inventory Value
   6.Exit
Enter your choice:

---

### 11. Option 5: Calculate Total Inventory Value

(Note: Exact values may vary slightly due to the precision of the floats and the previous operations in the example)

* *Input:*

Enter your choice: 5

* *Output:*

--- Inventory Value Breakdown --- Computer monitor (Price: $620,000.00, Qty: 15) = $93,000,000.00 Computer case (Price: $300,000.26, Qty: 15) = $45,000,003.90 Motherboard (Price: $300,000.32, Qty: 15) = $45,000,000.80 RAM (Price: $80,000.45, Qty: 40) = $32,000,018.00 Graphics card (Price: $4000000.12, Qty: 40) = $160000004.80 Hard disk ssd (Price: $100000.14, Qty: 35) = $3500004.90
Total Inventory Value: $225500036.40
--- Inventory Management System ---
* Add Product
* Consult Product
* Update Product Price
   4.DeleteProduct
* Calculate Total Inventory Value
   6.Exit
Enter your choice:

---

### 12. Invalid Option

* *Entrance:*

Enter your choice: 9

* *Exit:*

Invalid option. Please try again.
--- Inventory Management System ---
* Add Product
* Consult Product
* Update Product Price
   4.DeleteProduct
* Calculate Total Inventory Value
   6.Exit
Enter your choice:

---

### 13. Option 6: Exit the System

* *Enter:*

Enter your choice: 6

* *Exit:*

Exiting Inventory Management System. Goodbye!

(The program will terminate at this point)

# Sistema de Gestión de Inventario - Español

Esta es una aplicación de consola basada en Python diseñada para gestionar el inventario de productos. Permite a los usuarios añadir, consultar, actualizar precios, eliminar productos y calcular el valor total del inventario.

## Funcionalidades

1. *Añadir productos:* Añade nuevos productos al inventario con su nombre, precio y cantidad. Si ya existe un producto con el mismo nombre, se actualizará su cantidad.
2. *Consultar productos:* Busca un producto por su nombre y muestra su información actual (precio y cantidad).
3. *Actualizar precios de productos:* Modifica el precio de un producto existente.
4. *Eliminar productos:* Elimina un producto del inventario tras una solicitud de confirmación.
5. *Calcular el valor total del inventario:* Calcula y muestra la suma de (precio * cantidad) de todos los productos del inventario, mostrando el total y un desglose de cada artículo.

## Criterios de aceptación cumplidos

* *Productos iniciales:* El programa se inicializa con al menos 5 productos preagregados al iniciarse.
* *Consulta de productos:* Si no se encuentra un producto durante la consulta, se muestra un mensaje claro de "no encontrado".
* *Validación de actualización de precios:* Los nuevos precios deben ser números positivos. El sistema valida esta entrada.
* *Confirmación de eliminación de producto:* Antes de eliminar un producto, el sistema solicita confirmación.
* *Precisión del valor total del inventario:* El valor total del inventario se calcula con precisión y se muestra con dos decimales.
* *Estructura del código y comentarios:* El código está bien estructurado en funciones para cada operación e incluye comentarios explicativos.
* *Idioma:* Todo el código y los comentarios están 100 % en inglés.

## Cómo ejecutar el programa

1. *Guardar el código:* Guarde el código Python proporcionado en un archivo llamado inventory_manager.py.
2. *Abrir una terminal o símbolo del sistema:* Navegue al directorio donde guardó el archivo inventory_manager.py.
3. *Ejecutar el script:* Ejecute el programa usando el intérprete de Python:

```bash
python inventory_manager.py

* Interactuar con el menú: Siga las instrucciones en pantalla para elegir entre las opciones disponibles (añadir, consultar, actualizar precio, eliminar, calcular el valor total o salir).
Ejemplos de Uso (Entrada y Salida)
A continuación, se muestran ejemplos de cómo interactuar con el sistema y las salidas esperadas.
1. Inicio del Programa (Productos Iniciales)
Al iniciar el programa, se agregan automáticamente algunos productos al inventario como valores predeterminados.
* Entrada:
<!-- end list -->
(Ninguna interacción del usuario, se ejecuta automáticamente al llamar `main()`)

* Salida:
<!-- end list -->
Product 'Computer monitor' added/updated successfully.
Product 'Computer case' added/updated successfully.
Product 'Motherboard' added/updated successfully.
Product 'RAM' added/updated successfully.
Product 'Graphics card' added/updated successfully.
Product 'hard disk SSD' added/updated successfully.

--- Inventory Management System ---
1. Add Product
2. Consult Product
3. Update Product Price
4. Delete Product
5. Calculate Total Inventory Value
6. Exit
-----------------------------------
Enter your choice:

2. Opción 1: Agregar un Nuevo Producto
* Entrada:
<!-- end list -->
Enter your choice: 1
Enter product name: Teclado
Enter product price: 75000.50
Enter product quantity: 20

* Salida:
<!-- end list -->
Product 'Teclado' added/updated successfully.

--- Inventory Management System ---
1. Add Product
2. Consult Product
3. Update Product Price
4. Delete Product
5. Calculate Total Inventory Value
6. Exit
-----------------------------------
Enter your choice:

3. Opción 1: Actualizar la Cantidad de un Producto Existente
(Nota: La cantidad de RAM original era 30, ahora es 30 + 10 = 40)
* Entrada:
<!-- end list -->
Enter your choice: 1
Enter product name: ram
Enter product price: 80000.45
Enter product quantity: 10

* Salida:
<!-- end list -->
Product 'ram' already exists. Updating quantity.
Product 'ram' added/updated successfully.

--- Inventory Management System ---
1. Add Product
2. Consult Product
3. Update Product Price
4. Delete Product
5. Calculate Total Inventory Value
6. Exit
-----------------------------------
Enter your choice:

4. Opción 1: Entrada Inválida al Agregar Producto (Precio)
* Entrada:
<!-- end list -->
Enter your choice: 1
Enter product name: Mouse
Enter product price: abc

* Salida:
<!-- end list -->
Invalid input. Price must be a number and quantity an integer.

--- Inventory Management System ---
1. Add Product
2. Consult Product
3. Update Product Price
4. Delete Product
5. Calculate Total Inventory Value
6. Exit
-----------------------------------
Enter your choice:

5. Opción 2: Consultar un Producto Existente
* Entrada:
<!-- end list -->
Enter your choice: 2
Enter product name to consult: Graphics Card

* Salida:
<!-- end list -->
    Product Details for 'Graphics Card'
Name: Graphics Card
Price: $4000000.12
Quantity: 40
----------------------------------------

--- Inventory Management System ---
1. Add Product
2. Consult Product
3. Update Product Price
4. Delete Product
5. Calculate Total Inventory Value
6. Exit
-----------------------------------
Enter your choice:

6. Opción 2: Consultar un Producto No Existente
* Entrada:
<!-- end list -->
Enter your choice: 2
Enter product name to consult: Monitor curvo

* Salida:
<!-- end list -->
Product 'Monitor curvo' not found in inventory.

--- Inventory Management System ---
1. Add Product
2. Consult Product
3. Update Product Price
4. Delete Product
5. Calculate Total Inventory Value
6. Exit
-----------------------------------
Enter your choice:

7. Opción 3: Actualizar el Precio de un Producto
* Entrada:
<!-- end list -->
Enter your choice: 3
Enter product name to update price: computer monitor
Enter new price: 620000.00

* Salida:
<!-- end list -->
Price for 'computer monitor' updated from $600000.85 to $620000.00.

--- Inventory Management System ---
1. Add Product
2. Consult Product
3. Update Product Price
4. Delete Product
5. Calculate Total Inventory Value
6. Exit
-----------------------------------
Enter your choice:

8. Opción 4: Eliminar un Producto (Confirmando la Eliminación)
* Entrada:
<!-- end list -->
Enter your choice: 4
Enter product name to delete: Teclado
The product 'Teclado' exists
Are you sure you want to delete 'Teclado' with a price of '75000.5' and with '20' quantities? (yes/no): yes

* Salida:
<!-- end list -->
Product 'Teclado' deleted successfully.

--- Inventory Management System ---
1. Add Product
2. Consult Product
3. Update Product Price
4. Delete Product
5. Calculate Total Inventory Value
6. Exit
-----------------------------------
Enter your choice:

9. Opción 4: Eliminar un Producto (Cancelando la Eliminación)
* Entrada:
<!-- end list -->
Enter your choice: 4
Enter product name to delete: Hard Disk SSD
The product 'Hard Disk SSD' exists
Are you sure you want to delete 'Hard Disk SSD' with a price of '100000.14451' and with '35' quantities? (yes/no): no

* Salida:
<!-- end list -->
Deletion of 'Hard Disk SSD' cancelled.

--- Inventory Management System ---
1. Add Product
2. Consult Product
3. Update Product Price
4. Delete Product
5. Calculate Total Inventory Value
6. Exit
-----------------------------------
Enter your choice:

10. Opción 4: Intentar Eliminar un Producto No Existente
* Entrada:
<!-- end list -->
Enter your choice: 4
Enter product name to delete: Mouse

* Salida:
<!-- end list -->
The product 'Mouse' does not exist
Product 'Mouse' not found in inventory. Cannot delete.

--- Inventory Management System ---
1. Add Product
2. Consult Product
3. Update Product Price
4. Delete Product
5. Calculate Total Inventory Value
6. Exit
-----------------------------------
Enter your choice:

11. Opción 5: Calcular el Valor Total del Inventario
(Nota: Los valores exactos pueden variar ligeramente debido a la precisión de los floats y las operaciones previas en el ejemplo)
* Entrada:
<!-- end list -->
Enter your choice: 5

* Salida:
<!-- end list -->
--- Inventory Value Breakdown ---
Computer monitor (Price: $620000.00, Qty: 15) = $9300000.00
Computer case (Price: $300000.26, Qty: 15) = $4500003.90
Motherboard (Price: $3000000.32, Qty: 15) = $45000004.80
Ram (Price: $80000.45, Qty: 40) = $3200018.00
Graphics card (Price: $4000000.12, Qty: 40) = $160000004.80
Hard disk ssd (Price: $100000.14, Qty: 35) = $3500004.90
------------------------------------------
Total Inventory Value: $225500036.40
------------------------------------------

--- Inventory Management System ---
1. Add Product
2. Consult Product
3. Update Product Price
4. Delete Product
5. Calculate Total Inventory Value
6. Exit
-----------------------------------
Enter your choice:

12. Opción Inválida
* Entrada:
<!-- end list -->
Enter your choice: 9

* Salida:
<!-- end list -->
Invalid option. Please try again.

--- Inventory Management System ---
1. Add Product
2. Consult Product
3. Update Product Price
4. Delete Product
5. Calculate Total Inventory Value
6. Exit
-----------------------------------
Enter your choice:

13. Option 6: Exit the System
* Enter:
<!-- end list -->
Enter your choice: 6

* Exit:
<!-- end list -->
Exiting Inventory Management System. Goodbye!

(The program will terminate at this point)
