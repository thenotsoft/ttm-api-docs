Exemplu de respuns:
-------

```json
{
    "result": "ok",
    "data": {
        "search_id": "99d9e616-1e6f-4ad3-9eb3-79aeb04b42ba",
        "search_request": {
            "flights": [
                {
                    "from": [
                        {
                            "code": "kiv",
                            "type": "airport"
                        }
                    ],
                    "to": [
                        {
                            "code": "par",
                            "type": null
                        }
                    ],
                    "date": {
                        "departure": {
                            "type": "specific",
                            "value": "15-12-2020"
                        },
                        "return": {
                            "type": "one_way"
                        }
                    }
                }
            ],
            "passengers": {
                "adults": 1,
                "children": 0,
                "infants": 0
            },
            "flight_class": "economy"
        },
        "total": 0,
        "offers": [
            {
                "id": "661504fb-8b04-4891-96cd-7ba1309d588d",
                "stay_nights": 0,
                "airline_type": "lowcost",
                "virtual_interlining": false,
                "baggage_recheck_required": false,
                "journey_time": 7200,
                "operating_carrier": "sp6",
                "price": {
                    "amount": "86.00",
                    "currency": "EUR"
                },
                "fee": {
                    "adults": {
                        "amount": "15.00",
                        "currency": "EUR"
                    },
                    "children": {
                        "amount": "0.00",
                        "currency": "EUR"
                    },
                    "infants": {
                        "amount": "0.00",
                        "currency": "EUR"
                    },
                    "total": {
                        "amount": "15.00",
                        "currency": "EUR"
                    }
                },
                "fare": {
                    "adults": {
                        "amount": "86.00",
                        "currency": "EUR"
                    },
                    "children": {
                        "amount": "0.00",
                        "currency": "EUR"
                    },
                    "infants": {
                        "amount": "0.00",
                        "currency": "EUR"
                    },
                    "total": {
                        "amount": "86.00",
                        "currency": "EUR"
                    }
                },
                "parts": [
                    {
                        "type": "out",
                        "badges": [],
                        "segments": [
                            {
                                "from": {
                                    "name": "Chisinau Arpt",
                                    "code": "KIV",
                                    "longitude": 28.93083,
                                    "latitude": 46.92778,
                                    "type": "airport",
                                    "city": {
                                        "name": "Chisinau",
                                        "code": "KIV",
                                        "longitude": 28.93083,
                                        "latitude": 46.92778,
                                        "type": "city",
                                        "country": {
                                            "name": "Moldova Republic Of",
                                            "code": "MD",
                                            "iso3": "MDA",
                                            "numeric_iso": 498,
                                            "type": "country",
                                            "continent": {
                                                "name": "Europe",
                                                "code": "EU",
                                                "type": "continent"
                                            }
                                        }
                                    }
                                },
                                "to": {
                                    "name": "Vnukovo Arpt",
                                    "code": "VKO",
                                    "longitude": 37.26149,
                                    "latitude": 55.59153,
                                    "type": "airport",
                                    "city": {
                                        "name": "Moscow",
                                        "code": "MOW",
                                        "longitude": 37.26149,
                                        "latitude": 55.59153,
                                        "type": "city",
                                        "country": {
                                            "name": "Russian Federation",
                                            "code": "RU",
                                            "iso3": "RUS",
                                            "numeric_iso": 643,
                                            "type": "country",
                                            "continent": {
                                                "name": "Europe",
                                                "code": "EU",
                                                "type": "continent"
                                            }
                                        }
                                    }
                                },
                                "properties": {
                                    "wait_time": 0,
                                    "bag_re_check": false,
                                    "re_check": false,
                                    "guarantee": false
                                },
                                "flight": {
                                    "number": "121",
                                    "duration": 7200,
                                    "plane": null
                                },
                                "carrier": {
                                    "name": "Fly One",
                                    "code": "5F",
                                    "type": "airline"
                                },
                                "date": {
                                    "departure": "2021-01-15T10:00:00+0000",
                                    "arrival": "2021-01-15T13:00:00+0000"
                                },
                                "terminal": {
                                    "departure": null,
                                    "arrival": null
                                }
                            }
                        ],
                        "journey_time": 7200
                    }
                ]
            }

          ...

        ]
    }
}
```

TBD...