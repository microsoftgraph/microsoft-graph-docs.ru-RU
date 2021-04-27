---
title: Создание educationRubric
description: Создайте новый объект educationRubric.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 7bac8951155143276447edf743fea1eaf048bc6b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52042690"
---
# <a name="create-educationrubric"></a><span data-ttu-id="689be-103">Создание educationRubric</span><span class="sxs-lookup"><span data-stu-id="689be-103">Create educationRubric</span></span>

<span data-ttu-id="689be-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="689be-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="689be-105">Создайте новый [объект educationRubric.](../resources/educationrubric.md)</span><span class="sxs-lookup"><span data-stu-id="689be-105">Create a new [educationRubric](../resources/educationrubric.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="689be-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="689be-106">Permissions</span></span>

<span data-ttu-id="689be-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="689be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="689be-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="689be-109">Permission type</span></span>                        | <span data-ttu-id="689be-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="689be-110">Permissions (from least to most privileged)</span></span>             |
| :------------------------------------- | :------------------------------------------------------ |
| <span data-ttu-id="689be-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="689be-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="689be-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="689be-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="689be-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="689be-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="689be-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="689be-114">Not supported.</span></span>                                          |
| <span data-ttu-id="689be-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="689be-115">Application</span></span>                            | <span data-ttu-id="689be-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="689be-116">Not supported.</span></span>                                          |

## <a name="http-request"></a><span data-ttu-id="689be-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="689be-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /education/me/rubrics
```

## <a name="request-headers"></a><span data-ttu-id="689be-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="689be-118">Request headers</span></span>

| <span data-ttu-id="689be-119">Имя</span><span class="sxs-lookup"><span data-stu-id="689be-119">Name</span></span>          | <span data-ttu-id="689be-120">Описание</span><span class="sxs-lookup"><span data-stu-id="689be-120">Description</span></span>    |
| :------------ | :------------- |
| <span data-ttu-id="689be-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="689be-121">Authorization</span></span> | <span data-ttu-id="689be-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="689be-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="689be-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="689be-123">Request body</span></span>

<span data-ttu-id="689be-124">В органе запроса поставляем представление JSON объекта [educationRubric.](../resources/educationrubric.md)</span><span class="sxs-lookup"><span data-stu-id="689be-124">In the request body, supply a JSON representation of an [educationRubric](../resources/educationrubric.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="689be-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="689be-125">Response</span></span>

<span data-ttu-id="689be-126">В случае успеха этот метод возвращает код ответа и `201 Created` новый [объект educationRubric](../resources/educationrubric.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="689be-126">If successful, this method returns `201 Created` response code and a new [educationRubric](../resources/educationrubric.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="689be-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="689be-127">Examples</span></span>

### <a name="example-1-posting-a-credit-rubric"></a><span data-ttu-id="689be-128">Пример 1. Публикация кредитной рубрики</span><span class="sxs-lookup"><span data-stu-id="689be-128">Example 1: Posting a Credit Rubric</span></span>

#### <a name="request"></a><span data-ttu-id="689be-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="689be-129">Request</span></span>

<span data-ttu-id="689be-130">Ниже приводится пример запроса на публикацию кредитной рубрики (рубрика без баллов).</span><span class="sxs-lookup"><span data-stu-id="689be-130">The following is an example of the request to post a credit rubric (a rubric with no points).</span></span>

# <a name="http"></a>[<span data-ttu-id="689be-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="689be-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationrubric_from_educationuser_1"
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
# <a name="c"></a>[<span data-ttu-id="689be-132">C#</span><span class="sxs-lookup"><span data-stu-id="689be-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationrubric-from-educationuser-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="689be-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="689be-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationrubric-from-educationuser-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="689be-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="689be-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationrubric-from-educationuser-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="689be-135">Java</span><span class="sxs-lookup"><span data-stu-id="689be-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationrubric-from-educationuser-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="689be-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="689be-136">Response</span></span>

<span data-ttu-id="689be-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="689be-137">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="689be-138">Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="689be-138">The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-posting-a-points-rubric"></a><span data-ttu-id="689be-139">Пример 2. Публикация рубрики Points</span><span class="sxs-lookup"><span data-stu-id="689be-139">Example 2: Posting a Points Rubric</span></span>

<span data-ttu-id="689be-140">Ниже приводится пример запроса на публикацию рубрики с точками.</span><span class="sxs-lookup"><span data-stu-id="689be-140">The following is an example of the request to post a rubric with points.</span></span>

# <a name="http"></a>[<span data-ttu-id="689be-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="689be-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationrubric_from_educationuser_2"
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
# <a name="c"></a>[<span data-ttu-id="689be-142">C#</span><span class="sxs-lookup"><span data-stu-id="689be-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationrubric-from-educationuser-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="689be-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="689be-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationrubric-from-educationuser-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="689be-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="689be-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationrubric-from-educationuser-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="689be-145">Java</span><span class="sxs-lookup"><span data-stu-id="689be-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationrubric-from-educationuser-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="689be-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="689be-146">Response</span></span>

<span data-ttu-id="689be-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="689be-147">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="689be-148">Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="689be-148">The response object shown here might be shortened for readability.</span></span>

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


