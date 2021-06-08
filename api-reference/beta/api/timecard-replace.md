---
title: Замените timeCard
description: Обновление существующей записи timeCard.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 095c5fcdda15496ab41570aa940ad09585f9a633
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787898"
---
# <a name="replace-timecard"></a><span data-ttu-id="91b43-103">Замените timeCard</span><span class="sxs-lookup"><span data-stu-id="91b43-103">Replace timeCard</span></span>

<span data-ttu-id="91b43-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91b43-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91b43-105">Замените [существующую систему timeCard](../resources/timecard.md) обновленными значениями.</span><span class="sxs-lookup"><span data-stu-id="91b43-105">Replace an existing [timeCard](../resources/timecard.md) with updated values.</span></span>

## <a name="permissions"></a><span data-ttu-id="91b43-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="91b43-106">Permissions</span></span>

<span data-ttu-id="91b43-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91b43-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91b43-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="91b43-109">Permission type</span></span>      | <span data-ttu-id="91b43-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="91b43-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91b43-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="91b43-111">Delegated (work or school account)</span></span> | <span data-ttu-id="91b43-112">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91b43-112">Schedule.ReadWrite.All</span></span>    |
|<span data-ttu-id="91b43-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="91b43-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91b43-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91b43-114">Not supported.</span></span>    |
|<span data-ttu-id="91b43-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="91b43-115">Application</span></span> | <span data-ttu-id="91b43-116">Schedule.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="91b43-116">Schedule.ReadWrite.All\*</span></span>  |

><span data-ttu-id="91b43-117">\***Важно:** При использовании разрешений приложения необходимо включить в запрос `MS-APP-ACTS-AS` заготвую.</span><span class="sxs-lookup"><span data-stu-id="91b43-117">\* **Important:** When you use application permissions, you must include the `MS-APP-ACTS-AS` header in the request.</span></span>

## <a name="http-request"></a><span data-ttu-id="91b43-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="91b43-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/timecards/{timeCardID}
```

## <a name="request-headers"></a><span data-ttu-id="91b43-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="91b43-119">Request headers</span></span>

| <span data-ttu-id="91b43-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="91b43-120">Header</span></span>       | <span data-ttu-id="91b43-121">Значение</span><span class="sxs-lookup"><span data-stu-id="91b43-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="91b43-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="91b43-122">Authorization</span></span>  | <span data-ttu-id="91b43-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="91b43-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="91b43-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="91b43-125">Content-Type</span></span>  | <span data-ttu-id="91b43-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="91b43-p103">application/json. Required.</span></span>  |
| <span data-ttu-id="91b43-128">MS-APP-ACTS-AS</span><span class="sxs-lookup"><span data-stu-id="91b43-128">MS-APP-ACTS-AS</span></span> | <span data-ttu-id="91b43-129">ID пользователя, от имени которого действует приложение.</span><span class="sxs-lookup"><span data-stu-id="91b43-129">The ID of the user on behalf of whom the app is acting.</span></span> <span data-ttu-id="91b43-130">Требуется при использовании области разрешений приложения.</span><span class="sxs-lookup"><span data-stu-id="91b43-130">Required when you use the application permission scope.</span></span> |

## <a name="request-body"></a><span data-ttu-id="91b43-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="91b43-131">Request body</span></span>

<span data-ttu-id="91b43-132">В теле запроса поставляем JSON-представление объекта [timeCard.](../resources/timecard.md)</span><span class="sxs-lookup"><span data-stu-id="91b43-132">In the request body, supply a JSON representation of a [timeCard](../resources/timecard.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="91b43-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="91b43-133">Response</span></span>

<span data-ttu-id="91b43-134">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="91b43-134">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="91b43-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="91b43-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="91b43-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="91b43-136">Request</span></span>

<span data-ttu-id="91b43-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="91b43-137">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="91b43-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="91b43-138">Response</span></span>

<span data-ttu-id="91b43-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="91b43-139">The following is an example of the response.</span></span> 
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
