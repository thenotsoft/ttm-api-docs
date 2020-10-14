Exemplu de request:
-------

```http request
POST https://api.ttm.dev/v1/search/flight HTTP/1.1
Content-Type: application/json 
X-Api-Key: <aici tokenu de access primit>
```

body (json payload)
```json
{
  "flights": [
    {
      "from": ["lon"],
      "to": ["city:mow"],
      "date": {
        "departure": {
          "type": "specific",
          "value": "20-12-2020"
        },
        "return": {
          "type": "ONE_WAY"
        }
      }
    }
  ],
  "flightClass": "economy",
  "passengers": {
    "adults": 1,
    "children": 0,
    "infants": 0
  }
}
```

Requestu trebu sa contina parametrii obligatorii
-----

```flights``` acest parametru este de tip array si contine elemente de tip object, la care sunt urmatoarele parametri obligatoare

* ```form``` punctul de plecare
* ```to``` punctul de destinatie

   > acestea doua parametre is de tip ```string[]``` se indica codu la airport/oras/tara/gara de tren, si posibil de indicat si tipu concret ca exemplu ```airport:kiw``` din cre prima parte este tipu si a 2 deja codu airporotului, concomitent pot fii indicate max. 3 coduri
    
```date``` data de plecare si de intoarcere de tip ```object``` care contine urmatorii parametrii
    
* ```departure``` data de plecare
* ```return``` data de intoarcere
    
    > data contine parametru obligatoriu ```type``` care are 4 tipuri
    > * ```specific``` acest tip de data indica o data anumita, cu acest tip de data trebu sa fie indicata si keia ```value``` tip ```string``` in format ```d-m-Y```
    > * ```range``` acest tip de data indica un range intre data A si data B, cu acest tip de data obligatoriu trebu indicata keia ```start``` si ```end``` ambele de tip ```string``` in format ```d-m-Y```
    > * ```duration``` 
    > * ```one_way``` acest tip de date indica ca nu exista data de intoarcere, nu are kei adaugatoare. 
        Acest tip de data poate fii folosit numa la ```return```
                                        
    
```flightClass``` tipu de zbor, aici sunt 3 tipuri

> * ```economy```
> * ```premium-economy```
> * ```business```

```passengers``` este de tip object cu parametrii

> * ```adults``` adulti
> * ```children``` copii
> * ```infants``` bebelusi
>
> toate acestea parametri is de tip ```integer```