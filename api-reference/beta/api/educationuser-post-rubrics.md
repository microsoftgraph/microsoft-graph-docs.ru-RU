---
title: Создание Едукатионрубрик
description: Создание нового объекта Едукатионрубрик.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 60c9f0338cd79db41221efd379227dbbb2055bd5
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48955169"
---
# <a name="create-educationrubric"></a>Создание Едукатионрубрик

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создание нового объекта [едукатионрубрик](../resources/educationrubric.md) .

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий)             |
| :------------------------------------- | :------------------------------------------------------ |
| Делегированные (рабочая или учебная учетная запись)     | EduAssignments. Реадвритебасик, EduAssignments. ReadWrite |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                                          |
| Для приложений                            | Не поддерживается.                                          |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /education/me/rubrics
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание    |
| :------------ | :------------- |
| Authorization | Bearer {token} |

## <a name="request-body"></a>Тело запроса

В тексте запроса добавьте представление объекта [едукатионрубрик](../resources/educationrubric.md) в формате JSON.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [едукатионрубрик](../resources/educationrubric.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="example-1-posting-a-credit-rubric"></a>Пример 1: учет кредитных Rubric

#### <a name="request"></a>Запрос

Ниже приведен пример запроса на разноску кредита Rubric (Rubric без точек).

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationrubric_from_educationuser"
}-->

```http
POST https://graph.microsoft.com/beta/education/me/rubrics
Content-type: application/json

{
    "displayName":"Example Credit Rubric",
    "description":{
        "content":"This is an example of a credit rubric (no points)",
        "contentType":"text"
    },
    "levels":[
        {
            "displayName":"Good",
            "description":{
                "content":"",
                "contentType":"text"
            }
        },
        {
            "displayName":"Poor",
            "description":{
                "content":"",
                "contentType":"text"
            }
        }
    ],
    "qualities":[
        {
            "description":{
                "content":"Argument",
                "contentType":"text"
            },
            "criteria":[
                {
                    "description":{
                        "content":"The essay's argument is persuasive.",
                        "contentType":"text"
                    }
                },
                {
                    "description":{
                        "content":"The essay's argument does not make sense.",
                        "contentType":"text"
                    }
                }
            ]
        },
        {
            "description":{
                "content":"Spelling and Grammar",
                "contentType":"text"
            },
            "criteria":[
                {
                    "description":{
                        "content":"The essay uses proper spelling and grammar with few or no errors.",
                        "contentType":"text"
                    }
                },
                {
                    "description":{
                        "content":"The essay has numerous errors in spelling and/or grammar.",
                        "contentType":"text"
                    }
                }
            ]
        }
    ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationrubric-from-educationuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationrubric-from-educationuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationrubric-from-educationuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationrubric-from-educationuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

Ниже приведен пример отклика.

> [!NOTE]
> Объект Response, показанный здесь, может быть укорочен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationRubric"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "displayName": "Example Credit Rubric",
    "id": "63618139-2e8d-4f56-a762-dd734736816f",
    "description": {
        "content": "This is an example of a credit rubric (no points)",
        "contentType": "text"
    },
    "qualities": [
        {
            "qualityId": "461e866a-4844-4a3f-9a3c-e5464a32acf1",
            "description": {
                "content": "Argument",
                "contentType": "text"
            },
            "criteria": [
                {
                    "description": {
                        "content": "The essay's argument is persuasive.",
                        "contentType": "text"
                    }
                },
                {
                    "description": {
                        "content": "The essay's argument does not make sense.",
                        "contentType": "text"
                    }
                }
            ]
        },
        {
            "qualityId": "ccb47c1c-1a01-4027-93d7-f14b9fe86fdd",
            "description": {
                "content": "Spelling and Grammar",
                "contentType": "text"
            },
            "criteria": [
                {
                    "description": {
                        "content": "The essay uses proper spelling and grammar with few or no errors.",
                        "contentType": "text"
                    }
                },
                {
                    "description": {
                        "content": "The essay has numerous errors in spelling and/or grammar.",
                        "contentType": "text"
                    }
                }
            ]
        }
    ],
    "levels": [
        {
            "levelId": "564e68f6-984b-4574-bea7-ffae3c92633f",
            "displayName": "Good",
            "description": {
                "content": "",
                "contentType": "text"
            }
        },
        {
            "levelId": "3f082e35-46e3-4944-baea-ea6c7e36ef37",
            "displayName": "Poor",
            "description": {
                "content": "",
                "contentType": "text"
            }
        }
    ]
}
```

### <a name="example-2-posting-a-points-rubric"></a>Пример 2: отправка точек Rubric

Ниже приведен пример запроса на размещение Rubric с точками.
<!-- {
  "blockType": "request",
  "name": "create_educationrubric_from_educationuser"
}-->

```http
POST https://graph.microsoft.com/beta/education/me/rubrics
Content-type: application/json

{
    "displayName":"Example Points Rubric",
    "description":{
        "content":"This is an example of a rubric with points",
        "contentType":"text"
    },
    "levels":[
        {
            "displayName":"Good",
            "description":{
                "content":"",
                "contentType":"text"
            },
            "grading":{
                "@odata.type":"#microsoft.graph.educationAssignmentPointsGradeType",
                "maxPoints":2
            }
        },
        {
            "displayName":"Poor",
            "description":{
                "content":"",
                "contentType":"text"
            },
            "grading":{
                "@odata.type":"#microsoft.graph.educationAssignmentPointsGradeType",
                "maxPoints":1
            }
        }
    ],
    "qualities":[
        {
            "description":{
                "content":"Argument",
                "contentType":"text"
            },
            "criteria":[
                {
                    "description":{
                        "content":"The essay's argument is persuasive.",
                        "contentType":"text"
                    }
                },
                {
                    "description":{
                        "content":"The essay's argument does not make sense.",
                        "contentType":"text"
                    }
                }
            ],
            "weight":50.0
        },
        {
            "description":{
                "content":"Spelling and Grammar",
                "contentType":"text"
            },
            "criteria":[
                {
                    "description":{
                        "content":"The essay uses proper spelling and grammar with few or no errors.",
                        "contentType":"text"
                    }
                },
                {
                    "description":{
                        "content":"The essay has numerous errors in spelling and/or grammar.",
                        "contentType":"text"
                    }
                }
            ],
            "weight":50.0
        }
    ],
    "grading":{
        "@odata.type":"#microsoft.graph.educationAssignmentPointsGradeType"
    }
}
```

#### <a name="response"></a>Отклик

Ниже приведен пример отклика.

> [!NOTE]
> Объект Response, показанный здесь, может быть укорочен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationRubric"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "displayName": "Example Points Rubric",
    "id": "bf040af7-a5ff-4abe-a8c8-1bdc532344c2",
    "description": {
        "content": "This is an example of a rubric with points",
        "contentType": "text"
    },
    "levels": [
        {
            "levelId": "519cd134-c513-40b9-aa71-fdb0d063c084",
            "displayName": "Good",
            "description": {
                "content": "",
                "contentType": "text"
            },
            "grading": {
                "@odata.type": "#microsoft.graph.educationAssignmentPointsGradeType",
                "maxPoints": 2
            }
        },
        {
            "levelId": "db2a0c91-abef-44cb-b8b1-ef1f85ef4a77",
            "displayName": "Poor",
            "description": {
                "content": "",
                "contentType": "text"
            },
            "grading": {
                "@odata.type": "#microsoft.graph.educationAssignmentPointsGradeType",
                "maxPoints": 1
            }
        }
    ],
    "qualities": [
        {
            "qualityId": "bbf3fb4a-a794-4b51-a1ad-c22fb891c5d8",
            "weight": 50.0,
            "description": {
                "content": "Argument",
                "contentType": "text"
            },
            "criteria": [
                {
                    "id": "5e637d79-f26b-4ea6-acd7-73824f0c0967",
                    "description": {
                        "content": "The essay's argument is persuasive.",
                        "contentType": "text"
                    }
                },
                {
                    "id": "ebdcc27f-d1ec-4aa3-9da7-bd8d7842e3d3",
                    "description": {
                        "content": "The essay's argument does not make sense.",
                        "contentType": "text"
                    }
                }
            ]
        },
        {
            "qualityId": "ebe97fd7-47f7-4e9a-b31b-221ad731fc5a",
            "weight": 50.0,
            "description": {
                "content": "Spelling and Grammar",
                "contentType": "text"
            },
            "criteria": [
                {
                    "id": "5417252a-f810-41eb-9a83-09276a258a08",
                    "description": {
                        "content": "The essay uses proper spelling and grammar with few or no errors.",
                        "contentType": "text"
                    }
                },
                {
                    "id": "5de220bd-74b9-41a7-85d5-9be7c6cb7933",
                    "description": {
                        "content": "The essay has numerous errors in spelling and/or grammar.",
                        "contentType": "text"
                    }
                }
            ]
        }
    ],
    "grading": {
        "@odata.type": "#microsoft.graph.educationAssignmentPointsGradeType",
        "maxPoints": 100
    }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationRubric",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


