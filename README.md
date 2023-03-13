# API Proyecto 2223-2: F1 🏎️

## Pilotos

La api de pilotos se puede consumir a través de este url [https://raw.githubusercontent.com/Algorimtos-y-Programacion-2223-2/api-proyecto/main/drivers.json](https://raw.githubusercontent.com/Algorimtos-y-Programacion-2223-2/api-proyecto/main/drivers.json) y devuelve una lista de objetos compuestos de la siguiente forma:

```json
{
  "driverId": "string",
  "permanentNumber": "string",
  "code": "string",
  "team": "string",
  "firstName": "string",
  "lastName": "string",
  "dateOfBirth": "string:yyyy-mm-dd",
  "nationality": "string"
}
```

## Constructores

La api de constructores se puede consumir a través de este url [https://raw.githubusercontent.com/Algorimtos-y-Programacion-2223-2/api-proyecto/main/constructors.json](https://raw.githubusercontent.com/Algorimtos-y-Programacion-2223-2/api-proyecto/main/constructors.json) y devuelve una lista de objetos compuestos de la siguiente forma:

```json
{
  "id": "string",
  "name": "string",
  "nationality": "string"
}
```

## Carreras

La api de carreras se puede consumir a través de este url [https://raw.githubusercontent.com/Algorimtos-y-Programacion-2223-2/api-proyecto/main/races.json](https://raw.githubusercontent.com/Algorimtos-y-Programacion-2223-2/api-proyecto/main/races.json) y devuelve una lista de objetos compuestos de la siguiente forma:

```json
{
  "round": "string:int",
  "name": "string",
  "circuit": {
    "circuitId": "string",
    "name": "string",
    "Location": {
      "lat": "float",
      "long": "float",
      "locality": "string",
      "country": "string"
    }
  },
  "map": {
    "vip": ["int:", "int:"],
    "general": ["int:", "int:"]
  },
  "date": "string:yyyy-mm-dd",
  "restaurants": [
    {
      "name": "string",
      "items": [
        {
          "name": "string",
          "type": "string:oneOf('food:fast','food:restaurant','drink:not-alcoholic','drink:alcoholic')",
          "price": "string:float"
        }
      ]
    }
  ]
}
```
