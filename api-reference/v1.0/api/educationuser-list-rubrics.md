---
title: Рубрики списков
description: Извлечение списка объектов educationrubric.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: c2241842b6ded3546b35fefb1e2a7cab30b4ff26
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912708"
---
# <a name="list-rubrics"></a><span data-ttu-id="25181-103">Рубрики списков</span><span class="sxs-lookup"><span data-stu-id="25181-103">List rubrics</span></span>

<span data-ttu-id="25181-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25181-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="25181-105">Извлечение списка [объектов educationRubric.](../resources/educationrubric.md)</span><span class="sxs-lookup"><span data-stu-id="25181-105">Retrieve a list of [educationRubric](../resources/educationrubric.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="25181-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="25181-106">Permissions</span></span>

<span data-ttu-id="25181-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25181-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="25181-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="25181-109">Permission type</span></span>                        | <span data-ttu-id="25181-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="25181-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="25181-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="25181-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="25181-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="25181-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="25181-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="25181-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25181-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25181-114">Not supported.</span></span> |
| <span data-ttu-id="25181-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="25181-115">Application</span></span>                            | <span data-ttu-id="25181-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25181-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="25181-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="25181-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/me/rubrics
```

## <a name="request-headers"></a><span data-ttu-id="25181-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="25181-118">Request headers</span></span>

| <span data-ttu-id="25181-119">Имя</span><span class="sxs-lookup"><span data-stu-id="25181-119">Name</span></span>      |<span data-ttu-id="25181-120">Описание</span><span class="sxs-lookup"><span data-stu-id="25181-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="25181-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="25181-121">Authorization</span></span> | <span data-ttu-id="25181-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="25181-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="25181-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="25181-123">Request body</span></span>

<span data-ttu-id="25181-124">Не поставляем тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="25181-124">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="25181-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="25181-125">Response</span></span>

<span data-ttu-id="25181-126">В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` [объектов educationRubric](../resources/educationrubric.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="25181-126">If successful, this method returns a `200 OK` response code and a collection of [educationRubric](../resources/educationrubric.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="25181-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="25181-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="25181-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="25181-128">Request</span></span>

<span data-ttu-id="25181-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="25181-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="25181-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="25181-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_rubrics"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/me/rubrics
```

### <a name="response"></a><span data-ttu-id="25181-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="25181-131">Response</span></span>

<span data-ttu-id="25181-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="25181-132">The following is an example of the response.</span></span>

> <span data-ttu-id="25181-133">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="25181-133">**Note:** The response object shown here might be shortened for readability.</span></span>

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


