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

```Ejemplo:```
```js
{
            "SlotName": "Body", // Categoría

            "Items": [
                {
                    "ClassName": "GorkaEJacket_Autumn", // Identificador
                    "Chance": 1.0, // Chance de aparición
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
```

```Ejemplo con aditamentos```
```Js
{
            "ClassName": "WEAPON", // Tipo
            "Chance": 1.0, // Chance de aparición
            "Quantity": {
                "Min": 0.0,
                "Max": 0.0
            },
            "Health": [],
            "InventoryAttachments": [
                {
                    "SlotName": "Shoulder", // Categoría
                    "Items": [
                        {
                            "ClassName": "GCGN_MP7", // Identificador (Arma)
                            "Chance": 1.0, // Chance de aparición
                            "Quantity": {
                                "Min": 0.0,
                                "Max": 0.0
                            },
                            "Health": [],
                            "InventoryAttachments": [
                                {
                                    "SlotName": "",
                                    "Items": [
                                        {
                                            "ClassName": "GCGN_MP7_40Rnd", // Identificador (Cargador)
                                            "Chance": 1.0, // Chance de aparición
                                            "Quantity": {
                                                "Min": 0.0,
                                                "Max": 0.0
                                            },
                                            "Health": [],
                                            "InventoryAttachments": [],
                                            "InventoryCargo": [],
                                            "ConstructionPartsBuilt": [],
                                            "Sets": []
                                        },
                                        {
                                            "ClassName": "SNAFU_Aimpoint_ACO", // Identificador (Aditamento-mira)
                                            "Chance": 1.0, // Chance de aparición
                                            "Quantity": {
                                                "Min": 0.0,
                                                "Max": 0.0
                                            },
                                            "Health": [],
                                            "InventoryAttachments": [
                                                {
                                                    "SlotName": "",
                                                    "Items": [
                                                        {
                                                            "ClassName": "Battery9V", // Identificador (aditamento de la mira)
                                                            "Chance": 1.0, // Chance de aparición
                                                            "Quantity": {
                                                                "Min": 0.0,
                                                                "Max": 0.0
                                                            },
                                                            "Health": [],
                                                            "InventoryAttachments": [],
                                                            "InventoryCargo": [],
                                                            "ConstructionPartsBuilt": [],
                                                            "Sets": []
                                                        }
                                                    ]
                                                }
                                            ],
                                            "InventoryCargo": [],
                                            "ConstructionPartsBuilt": [],
                                            "Sets": []
                                        }
                                    ]
                                }
                            ],
                            "InventoryCargo": [],
                            "ConstructionPartsBuilt": [],
                            "Sets": []
                        }
                    ]
                }
            ],
            "InventoryCargo": [ // Cargamento en el inventario
                {
                    "ClassName": "GCGN_MP7_40Rnd", // Identificador (Cargador)
                    "Chance": 1.0, // Chance de aparición
                    "Quantity": {
                        "Min": 0.0,
                        "Max": 0.0
                    },
                    "Health": [],
                    "InventoryAttachments": [],
                    "InventoryCargo": [],
                    "ConstructionPartsBuilt": [],
                    "Sets": []
                },
                {
                    "ClassName": "GCGN_MP7_40Rnd", // Identificador (Cargador)
                    "Chance": 1.0, // Chance de aparición
                    "Quantity": {
                        "Min": 0.0,
                        "Max": 0.0
                    },
                    "Health": [],
                    "InventoryAttachments": [],
                    "InventoryCargo": [],
                    "ConstructionPartsBuilt": [],
                    "Sets": []
                },
                {
                    "ClassName": "GCGN_MP7_40Rnd", // Identificador (Cargador)
                    "Chance": 1.0, // Chance de aparición
                    "Quantity": {
                        "Min": 0.0,
                        "Max": 0.0
                    },
                    "Health": [],
                    "InventoryAttachments": [],
                    "InventoryCargo": [],
                    "ConstructionPartsBuilt": [],
                    "Sets": []
                }
            ],
            "ConstructionPartsBuilt": [],
            "Sets": []
        }
```

# Los tipos de categorías de ropa son: <br>
```js
'Body' - Torso 
'Legs' - Piernas 
'Feet' - Pies 
'Gloves' - Guantes 
'Vest' - Chalecos 
'Hips' - Cinturones 
'HELMET' - Cascos 
'Mask' - Mascaras 
'Armband' - Brazaletes 
'BackPack' - Mochilas
```

# 🚀 Instalación y modificaciónes
`En la terminal de VSCode`

## Clona este repositorio:
```js
git clone https://github.com/FerNyXnX/Loadouts-Dayz-EFT-Mod.git
```

## Abrir la carpeta del repositorio en VSCode

```js
cd Loadouts-Dayz-EFT-Mod
```

```js
code .
```
`Esto abrirá todo el proyecto en VSCode.`

## Preparar los cambios para el commit

```js
 git add .
```
## Guardar los cambios

```js
git commit -m "Descripción de los cambios"

```
`Para la descripción de los cambios debe ser un mensaje breve y claro`

`Ejemplo:`
```js
git commit -m "Renombrados identificadores de ropa"

```
```js
git commit -m "Actualización general"

```
## Jalar los archivos antes de subirlos
```js
git pull origin main

```

## Subir los cambios a GitHub
```js
git push origin main  
```

## Archivos Realizados

`BigPipe` <br>
`Birdeye` <br>
`Knight` <br>
`Cultist` <br>
`Shturman` <br>
`Killa` <br>
`Glukhar` <br>
`Sanitar` <br>
`Reshala` <br>
`Santa` <br>
`Tagilla` <br>
`Guardias_Shturman`
```js 
Raiders // Faltan más armas
Scavs// Faltan más armas
Guardias_Reshala // Faltan
Guardias_Glukhar // Faltan
Guardias_Sanitar // Faltan
```

# 🤝 Contribuciones

Respetar las reglas de edición descritas.

No inventar nuevos códigos fuera de la estructura ya existente.

Hacer pull requests claros con la descripción de los cambios.
