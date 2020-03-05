---
title: Создание Едукатионрубрик
description: Создание нового объекта Едукатионрубрик.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: d8f236022bed6f6a92cceeafee108e59ae970ddd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42423583"
---
# <a name="create-educationrubric"></a><span data-ttu-id="f33e2-103">Создание Едукатионрубрик</span><span class="sxs-lookup"><span data-stu-id="f33e2-103">Create educationRubric</span></span>

<span data-ttu-id="f33e2-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f33e2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f33e2-105">Создание нового объекта [едукатионрубрик](../resources/educationrubric.md) .</span><span class="sxs-lookup"><span data-stu-id="f33e2-105">Create a new [educationRubric](../resources/educationrubric.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f33e2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f33e2-106">Permissions</span></span>

<span data-ttu-id="f33e2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f33e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f33e2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f33e2-109">Permission type</span></span>                        | <span data-ttu-id="f33e2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f33e2-110">Permissions (from least to most privileged)</span></span>             |
| :------------------------------------- | :------------------------------------------------------ |
| <span data-ttu-id="f33e2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f33e2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f33e2-112">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f33e2-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="f33e2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f33e2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f33e2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f33e2-114">Not supported.</span></span>                                          |
| <span data-ttu-id="f33e2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f33e2-115">Application</span></span>                            | <span data-ttu-id="f33e2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f33e2-116">Not supported.</span></span>                                          |

## <a name="http-request"></a><span data-ttu-id="f33e2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f33e2-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /education/me/rubrics
```

## <a name="request-headers"></a><span data-ttu-id="f33e2-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f33e2-118">Request headers</span></span>

| <span data-ttu-id="f33e2-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f33e2-119">Name</span></span>          | <span data-ttu-id="f33e2-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f33e2-120">Description</span></span>    |
| :------------ | :------------- |
| <span data-ttu-id="f33e2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f33e2-121">Authorization</span></span> | <span data-ttu-id="f33e2-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="f33e2-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f33e2-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f33e2-123">Request body</span></span>

<span data-ttu-id="f33e2-124">В тексте запроса добавьте представление объекта [едукатионрубрик](../resources/educationrubric.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f33e2-124">In the request body, supply a JSON representation of an [educationRubric](../resources/educationrubric.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f33e2-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="f33e2-125">Response</span></span>

<span data-ttu-id="f33e2-126">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и новый объект [едукатионрубрик](../resources/educationrubric.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f33e2-126">If successful, this method returns `201 Created` response code and a new [educationRubric](../resources/educationrubric.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f33e2-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="f33e2-127">Examples</span></span>

### <a name="example-1-posting-a-credit-rubric"></a><span data-ttu-id="f33e2-128">Пример 1: учет кредитных Rubric</span><span class="sxs-lookup"><span data-stu-id="f33e2-128">Example 1: Posting a Credit Rubric</span></span>

#### <a name="request"></a><span data-ttu-id="f33e2-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="f33e2-129">Request</span></span>

<span data-ttu-id="f33e2-130">Ниже приведен пример запроса на разноску кредита Rubric (Rubric без точек).</span><span class="sxs-lookup"><span data-stu-id="f33e2-130">The following is an example of the request to post a credit rubric (a rubric with no points).</span></span>

# <a name="http"></a>[<span data-ttu-id="f33e2-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="f33e2-131">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="f33e2-132">C#</span><span class="sxs-lookup"><span data-stu-id="f33e2-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationrubric-from-educationuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f33e2-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f33e2-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationrubric-from-educationuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f33e2-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f33e2-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationrubric-from-educationuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f33e2-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="f33e2-135">Response</span></span>

<span data-ttu-id="f33e2-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f33e2-136">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="f33e2-137">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f33e2-137">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f33e2-138">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f33e2-138">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-posting-a-points-rubric"></a><span data-ttu-id="f33e2-139">Пример 2: отправка точек Rubric</span><span class="sxs-lookup"><span data-stu-id="f33e2-139">Example 2: Posting a Points Rubric</span></span>

<span data-ttu-id="f33e2-140">Ниже приведен пример запроса на размещение Rubric с точками.</span><span class="sxs-lookup"><span data-stu-id="f33e2-140">The following is an example of the request to post a rubric with points.</span></span>
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

#### <a name="response"></a><span data-ttu-id="f33e2-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="f33e2-141">Response</span></span>

<span data-ttu-id="f33e2-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f33e2-142">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="f33e2-143">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f33e2-143">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f33e2-144">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f33e2-144">All the properties will be returned from an actual call.</span></span>

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
