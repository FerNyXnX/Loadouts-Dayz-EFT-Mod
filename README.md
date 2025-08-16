# 🎮 DayZ Mod - Modificaciones de Ropa, Armas y Aditamentos
Este proyecto contiene modificaciones personalizadas para **DayZ**, enfocadas en ropa, armas y aditamentos.  
Todo el trabajo está basado en la edición de archivos **JSON**, siguiendo reglas estrictas para mantener la consistencia del mod.

---

## 📂 Estructura del Proyecto

├── Loadouts  ```Carpeta princpial``` <br>
│&nbsp;└── archivos.json  ```18 archivos principales```

---

## 📝 Reglas para Editar el Código

🔒 **No se debe añadir código inventado desde cero.**  
🔄 **Si se necesita un nuevo arreglo o ítem:**
1. Copiar un bloque JSON existente.  
2. Modificar únicamente los **identificadores, nombres o valores necesarios**.  
3. Mantener la misma estructura y convenciones.
4. Es necesario tener el servidor activo y entrar en el juego para esta labor.
5. Solamente esta permitido editar para Admins asignados.

Ejemplo:
```json
{
            "SlotName": "Body", # Categoría

            "Items": [
                {
                    "ClassName": "GorkaEJacket_Autumn", # Identificador
                    "Chance": 1.0, # Chance de aparición
                    "Quantity": {
                        "Min": 0.0,
                        "Max": 0.0
                    },
                    "Health": [
                        {
                            "Min": 0.699999988079071,
                            "Max": 1.0,
                            "Zone": ""
                        }
                    ],
                    "InventoryAttachments": [],
                    "InventoryCargo": [],
                    "ConstructionPartsBuilt": [],
                    "Sets": []
                }    
            ]
        }
```json

