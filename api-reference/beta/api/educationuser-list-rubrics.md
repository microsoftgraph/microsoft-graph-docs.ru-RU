---
title: Список рубрикс
description: Получение списка объектов едукатионрубрик.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 316c49a9e0b6591ad64bd30e4ce80809eb8f0ac6
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461332"
---
# <a name="list-rubrics"></a><span data-ttu-id="9fb1f-103">Список рубрикс</span><span class="sxs-lookup"><span data-stu-id="9fb1f-103">List rubrics</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9fb1f-104">Получение списка объектов [едукатионрубрик](../resources/educationrubric.md) .</span><span class="sxs-lookup"><span data-stu-id="9fb1f-104">Retrieve a list of [educationRubric](../resources/educationrubric.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="9fb1f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9fb1f-105">Permissions</span></span>

<span data-ttu-id="9fb1f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9fb1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9fb1f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9fb1f-108">Permission type</span></span>                        | <span data-ttu-id="9fb1f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9fb1f-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9fb1f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9fb1f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9fb1f-111">EduAssignments. ReadBasic, EduAssignments. Реадвритебасик, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9fb1f-111">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="9fb1f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9fb1f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9fb1f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9fb1f-113">Not supported.</span></span> |
| <span data-ttu-id="9fb1f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9fb1f-114">Application</span></span>                            | <span data-ttu-id="9fb1f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9fb1f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9fb1f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9fb1f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/me/rubrics
```

## <a name="request-headers"></a><span data-ttu-id="9fb1f-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9fb1f-117">Request headers</span></span>

| <span data-ttu-id="9fb1f-118">Имя</span><span class="sxs-lookup"><span data-stu-id="9fb1f-118">Name</span></span>      |<span data-ttu-id="9fb1f-119">Описание</span><span class="sxs-lookup"><span data-stu-id="9fb1f-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9fb1f-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9fb1f-120">Authorization</span></span> | <span data-ttu-id="9fb1f-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="9fb1f-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="9fb1f-122">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9fb1f-122">Request body</span></span>

<span data-ttu-id="9fb1f-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9fb1f-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9fb1f-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="9fb1f-124">Response</span></span>

<span data-ttu-id="9fb1f-125">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [едукатионрубрик](../resources/educationrubric.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9fb1f-125">If successful, this method returns a `200 OK` response code and a collection of [educationRubric](../resources/educationrubric.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9fb1f-126">Примеры</span><span class="sxs-lookup"><span data-stu-id="9fb1f-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9fb1f-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="9fb1f-127">Request</span></span>

<span data-ttu-id="9fb1f-128">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9fb1f-128">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9fb1f-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="9fb1f-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_rubrics"
}-->

```http
GET https://graph.microsoft.com/beta/education/me/rubrics
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9fb1f-130">C#</span><span class="sxs-lookup"><span data-stu-id="9fb1f-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-rubrics-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9fb1f-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9fb1f-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-rubrics-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9fb1f-132">Цель — C</span><span class="sxs-lookup"><span data-stu-id="9fb1f-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-rubrics-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9fb1f-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="9fb1f-133">Response</span></span>

<span data-ttu-id="9fb1f-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9fb1f-134">The following is an example of the response.</span></span>

> <span data-ttu-id="9fb1f-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9fb1f-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationRubric",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
        {
            "displayName":"Example Credit Rubric",
            "id":"c4459fcb-a761-4f70-ac5b-e9466cb77c2a",
            "description":{
                "content":"This is an example of a credit rubric (no points)",
                "contentType":"text"
            },
            "levels":[
                {
                    "levelId":"dec665d4-cf1b-4481-ac61-1d5b6188f4f5",
                    "displayName":"Good",
                    "description":{
                        "content":"",
                        "contentType":"text"
                    }
                },
                {
                    "levelId":"3f2e4b0f-508e-4005-984b-17e061bc5377",
                    "displayName":"Poor",
                    "description":{
                        "content":"",
                        "contentType":"text"
                    }
                }
            ],
            "qualities":[
                {
                    "qualityId":"dc79dcbf-b536-4797-9c5b-902f28129fd0",
                    "description":{
                        "content":"Argument",
                        "contentType":"text"
                    },
                    "criteria":[
                        {
                            "id":"8937fa15-4a7c-4f27-bd01-ca3471d2d1d5",
                            "description":{
                                "content":"The essay's argument is persuasive.",
                                "contentType":"text"
                            }
                        },
                        {
                            "id":"4dfb5263-1d3f-4f0a-93ef-d24d800d0f69",
                            "description":{
                                "content":"The essay's argument does not make sense.",
                                "contentType":"text"
                            }
                        }
                    ]
                },
                {
                    "qualityId":"7e087062-ac25-4629-8386-a946350936db",
                    "description":{
                        "content":"Spelling and Grammar",
                        "contentType":"text"
                    },
                    "criteria":[
                        {
                            "id":"12276eb2-122c-4ad2-ba92-335ea798c88e",
                            "description":{
                                "content":"The essay uses proper spelling and grammar with few or no errors.",
                                "contentType":"text"
                            }
                        },
                        {
                            "id":"3db7e6b2-2b1b-4f8e-9fca-bea701159145",
                            "description":{
                                "content":"The essay has numerous errors in spelling and/or grammar.",
                                "contentType":"text"
                            }
                        }
                    ]
                }
            ]
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List rubrics",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
