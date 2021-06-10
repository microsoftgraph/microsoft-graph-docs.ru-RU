---
title: Get timeCard
description: Получите карточку timeCard по ID.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3ffeb7f57769cc84500b9c0dbb913c214ba6e144
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869536"
---
# <a name="get-timecard"></a><span data-ttu-id="30fa0-103">Get timeCard</span><span class="sxs-lookup"><span data-stu-id="30fa0-103">Get timeCard</span></span>

<span data-ttu-id="30fa0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30fa0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30fa0-105">Извлечение свойств и связей объекта [timeCard](../resources/timeCard.md) по ID.</span><span class="sxs-lookup"><span data-stu-id="30fa0-105">Retrieve the properties and relationships of a [timeCard](../resources/timeCard.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="30fa0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="30fa0-106">Permissions</span></span>

<span data-ttu-id="30fa0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30fa0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30fa0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="30fa0-109">Permission type</span></span>      | <span data-ttu-id="30fa0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="30fa0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="30fa0-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="30fa0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="30fa0-112">Schedule.Read.All, Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30fa0-112">Schedule.Read.All, Schedule.ReadWrite.All</span></span>    |
|<span data-ttu-id="30fa0-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="30fa0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30fa0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30fa0-114">Not supported.</span></span>    |
|<span data-ttu-id="30fa0-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="30fa0-115">Application</span></span> | <span data-ttu-id="30fa0-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="30fa0-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span> |

><span data-ttu-id="30fa0-117">\***Важно:** При использовании разрешений приложения необходимо включить в запрос `MS-APP-ACTS-AS` заготвую.</span><span class="sxs-lookup"><span data-stu-id="30fa0-117">\* **Important:** When you use application permissions, you must include the `MS-APP-ACTS-AS` header in the request.</span></span>

## <a name="http-request"></a><span data-ttu-id="30fa0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="30fa0-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timecards/{timecardID}

```

## <a name="optional-query-parameters"></a><span data-ttu-id="30fa0-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="30fa0-119">Optional query parameters</span></span>
<span data-ttu-id="30fa0-120">Этот метод не поддерживает параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="30fa0-120">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="30fa0-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="30fa0-121">Request headers</span></span>

| <span data-ttu-id="30fa0-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="30fa0-122">Header</span></span>       | <span data-ttu-id="30fa0-123">Значение</span><span class="sxs-lookup"><span data-stu-id="30fa0-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="30fa0-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="30fa0-124">Authorization</span></span>  | <span data-ttu-id="30fa0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="30fa0-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="30fa0-127">MS-APP-ACTS-AS</span><span class="sxs-lookup"><span data-stu-id="30fa0-127">MS-APP-ACTS-AS</span></span> | <span data-ttu-id="30fa0-128">ID пользователя, от имени которого действует приложение.</span><span class="sxs-lookup"><span data-stu-id="30fa0-128">The ID of the user on behalf of whom the app is acting.</span></span> <span data-ttu-id="30fa0-129">Требуется при использовании области разрешений приложения.</span><span class="sxs-lookup"><span data-stu-id="30fa0-129">Required when you use the application permission scope.</span></span> |

## <a name="request-body"></a><span data-ttu-id="30fa0-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="30fa0-130">Request body</span></span>
<span data-ttu-id="30fa0-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="30fa0-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="30fa0-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="30fa0-132">Response</span></span>

<span data-ttu-id="30fa0-133">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект timeCard](../resources/timeCard.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="30fa0-133">If successful, this method returns a `200 OK` response code and a [timeCard](../resources/timeCard.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30fa0-134">Пример</span><span class="sxs-lookup"><span data-stu-id="30fa0-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="30fa0-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="30fa0-135">Request</span></span>
<span data-ttu-id="30fa0-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="30fa0-136">The following is an example of the request.</span></span> 

# <a name="http"></a>[<span data-ttu-id="30fa0-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="30fa0-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timecard-get"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/fd15cad8-80f6-484f-9666-3caf695fbf32/schedule/timeCards/TCK_cc09588d-d9d2-4fa0-85dc-2aa5ef983972
```
# <a name="c"></a>[<span data-ttu-id="30fa0-138">C#</span><span class="sxs-lookup"><span data-stu-id="30fa0-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timecard-get-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="30fa0-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="30fa0-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timecard-get-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="30fa0-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="30fa0-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timecard-get-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="30fa0-141">Java</span><span class="sxs-lookup"><span data-stu-id="30fa0-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timecard-get-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="30fa0-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="30fa0-142">Response</span></span>

<span data-ttu-id="30fa0-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="30fa0-143">The following is an example of the response.</span></span> 

><span data-ttu-id="30fa0-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="30fa0-144">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeCard"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "TCK_cc09588d-d9d2-4fa0-85dc-2aa5ef983972",
    "createdDateTime": "2021-05-27T22:58:41.327Z",
    "lastModifiedDateTime": "2021-05-27T23:02:04.187Z",
    "userId": "70e47528-2fae-42b5-9d8e-ee73ccd90603",
    "state": "clockedOut",
    "confirmedBy": "user,manager",
    "notes": null,
    "lastModifiedBy": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
            "id": "70e47528-2fae-42b5-9d8e-ee73ccd90603",
            "displayName": "Jing Jing GuTwo"
        }
    },
    "clockInEvent": {
        "dateTime": "2021-05-27T22:58:41.327Z",
        "atApprovedLocation": null,
        "notes": {
            "contentType": "text",
            "content": "clock in notes"
        }
    },
    "clockOutEvent": {
        "dateTime": "2021-05-27T23:01:46.205Z",
        "atApprovedLocation": null,
        "notes": {
            "contentType": "text",
            "content": "clock out smaple notes"
        }
    },
    "breaks": [
        {
            "breakId": "BRK_138f4751-68b1-44c1-aca2-2b26cba9e73f",
            "notes": null,
            "start": {
                "dateTime": "2021-05-27T22:59:59.328Z",
                "atApprovedLocation": null,
                "notes": {
                    "contentType": "text",
                    "content": "start break smaple notes"
                }
            },
            "end": {
                "dateTime": "2021-05-27T23:01:10.205Z",
                "atApprovedLocation": null,
                "notes": {
                    "contentType": "text",
                    "content": "end break smaple notes"
                }
            }
        }
    ],
    "originalEntry": {
        "clockInEvent": {
            "dateTime": "2021-05-27T22:58:41.327Z",
            "atApprovedLocation": null,
            "notes": {
                "contentType": "text",
                "content": "clock in notes"
            }
        },
        "clockOutEvent": {
            "dateTime": "2021-05-27T23:01:46.205Z",
            "atApprovedLocation": null,
            "notes": {
                "contentType": "text",
                "content": "clock out smaple notes"
            }
        },
        "breaks": [
            {
                "breakId": "BRK_138f4751-68b1-44c1-aca2-2b26cba9e73f",
                "notes": null,
                "start": {
                    "dateTime": "2021-05-27T22:59:59.328Z",
                    "atApprovedLocation": null,
                    "notes": {
                        "contentType": "text",
                        "content": "start break smaple notes"
                    }
                },
                "end": {
                    "dateTime": "2021-05-27T23:01:10.205Z",
                    "atApprovedLocation": null,
                    "notes": {
                        "contentType": "text",
                        "content": "end break smaple notes"
                    }
                }
            }
        ]
    },
    "createdBy": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
            "id": "70e47528-2fae-42b5-9d8e-ee73ccd90603",
            "displayName": "Jing Jing GuTwo"
        }
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get a timeCard by ID",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
