---
title: Замените timeCard
description: Обновление существующей записи timeCard.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: cbfb5f30991ebd8ae2c2208a1e366557c6eafc1c
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870453"
---
# <a name="replace-timecard"></a><span data-ttu-id="616a8-103">Замените timeCard</span><span class="sxs-lookup"><span data-stu-id="616a8-103">Replace timeCard</span></span>

<span data-ttu-id="616a8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="616a8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="616a8-105">Замените [существующую систему timeCard](../resources/timecard.md) обновленными значениями.</span><span class="sxs-lookup"><span data-stu-id="616a8-105">Replace an existing [timeCard](../resources/timecard.md) with updated values.</span></span>

## <a name="permissions"></a><span data-ttu-id="616a8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="616a8-106">Permissions</span></span>

<span data-ttu-id="616a8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="616a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="616a8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="616a8-109">Permission type</span></span>      | <span data-ttu-id="616a8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="616a8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="616a8-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="616a8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="616a8-112">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="616a8-112">Schedule.ReadWrite.All</span></span>    |
|<span data-ttu-id="616a8-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="616a8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="616a8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="616a8-114">Not supported.</span></span>    |
|<span data-ttu-id="616a8-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="616a8-115">Application</span></span> | <span data-ttu-id="616a8-116">Schedule.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="616a8-116">Schedule.ReadWrite.All\*</span></span>  |

><span data-ttu-id="616a8-117">\***Важно:** При использовании разрешений приложения необходимо включить в запрос `MS-APP-ACTS-AS` заготвую.</span><span class="sxs-lookup"><span data-stu-id="616a8-117">\* **Important:** When you use application permissions, you must include the `MS-APP-ACTS-AS` header in the request.</span></span>

## <a name="http-request"></a><span data-ttu-id="616a8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="616a8-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/timecards/{timeCardID}
```

## <a name="request-headers"></a><span data-ttu-id="616a8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="616a8-119">Request headers</span></span>

| <span data-ttu-id="616a8-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="616a8-120">Header</span></span>       | <span data-ttu-id="616a8-121">Значение</span><span class="sxs-lookup"><span data-stu-id="616a8-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="616a8-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="616a8-122">Authorization</span></span>  | <span data-ttu-id="616a8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="616a8-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="616a8-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="616a8-125">Content-Type</span></span>  | <span data-ttu-id="616a8-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="616a8-p103">application/json. Required.</span></span>  |
| <span data-ttu-id="616a8-128">MS-APP-ACTS-AS</span><span class="sxs-lookup"><span data-stu-id="616a8-128">MS-APP-ACTS-AS</span></span> | <span data-ttu-id="616a8-129">ID пользователя, от имени которого действует приложение.</span><span class="sxs-lookup"><span data-stu-id="616a8-129">The ID of the user on behalf of whom the app is acting.</span></span> <span data-ttu-id="616a8-130">Требуется при использовании области разрешений приложения.</span><span class="sxs-lookup"><span data-stu-id="616a8-130">Required when you use the application permission scope.</span></span> |

## <a name="request-body"></a><span data-ttu-id="616a8-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="616a8-131">Request body</span></span>

<span data-ttu-id="616a8-132">В теле запроса поставляем JSON-представление объекта [timeCard.](../resources/timecard.md)</span><span class="sxs-lookup"><span data-stu-id="616a8-132">In the request body, supply a JSON representation of a [timeCard](../resources/timecard.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="616a8-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="616a8-133">Response</span></span>

<span data-ttu-id="616a8-134">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="616a8-134">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="616a8-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="616a8-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="616a8-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="616a8-136">Request</span></span>

<span data-ttu-id="616a8-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="616a8-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="616a8-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="616a8-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timecard_replace"
}-->

```http
PUT https://graph.microsoft.com/beta/teams/fd15cad8-80f6-484f-9666-3caf695fbf32/schedule/timeCards/TCK_3cd7413f-0337-433b-9a49-da0923185b3f
Content-type: application/json

{
    "userId": "70e47528-2fae-42b5-9d8e-ee73ccd90603",
    "state": "clockedOut",
    "confirmedBy": "None",
    "notes": null,
    "clockInEvent": {
        "dateTime": "2021-05-21T21:58:41.327Z",
        "atApprovedLocation": null,
        "notes": {
            "contentType": "text",
            "content": "update sample notes"
        }
    },
    "clockOutEvent": {
        "dateTime": "2021-05-21T22:01:46.205Z",
        "atApprovedLocation": null,
        "notes": {
            "contentType": "text",
            "content": "update sample notes"
        }
    },
    "breaks": [
        {
            "breakId": "BRK_138f4751-68b1-44c1-aca2-2b26cba9e73f",
            "notes": null,
            "start": {
                "dateTime": "2021-05-21T21:59:59.328Z",
                "atApprovedLocation": null,
                "notes": {
                    "contentType": "text",
                    "content": "update sample notes"
                }
            },
            "end": {
                "dateTime": "2021-05-21T22:01:10.205Z",
                "atApprovedLocation": null,
                "notes": {
                    "contentType": "text",
                    "content": "update sample notes"
                }
            }
        }
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="616a8-139">C#</span><span class="sxs-lookup"><span data-stu-id="616a8-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timecard-replace-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="616a8-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="616a8-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timecard-replace-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="616a8-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="616a8-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timecard-replace-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="616a8-142">Java</span><span class="sxs-lookup"><span data-stu-id="616a8-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timecard-replace-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="616a8-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="616a8-143">Response</span></span>

<span data-ttu-id="616a8-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="616a8-144">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "name": "timecard_replace"
} -->

```http
HTTP/1.1 204 No Content
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Replace an existing timeCard",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
