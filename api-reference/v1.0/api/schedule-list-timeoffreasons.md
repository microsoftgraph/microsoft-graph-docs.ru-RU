---
title: Список timeOffReasons
description: Получите список timeOffReasons в расписании.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 840b41dbdbd5054c1b3512cfbe1084451a3d6a0c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053876"
---
# <a name="list-timeoffreasons"></a><span data-ttu-id="858d8-103">Список timeOffReasons</span><span class="sxs-lookup"><span data-stu-id="858d8-103">List timeOffReasons</span></span>

<span data-ttu-id="858d8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="858d8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="858d8-105">Получите список [timeOffReasons в](../resources/timeoffreason.md) [расписании.](../resources/schedule.md)</span><span class="sxs-lookup"><span data-stu-id="858d8-105">Get the list of [timeOffReasons](../resources/timeoffreason.md) in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="858d8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="858d8-106">Permissions</span></span>

<span data-ttu-id="858d8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="858d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="858d8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="858d8-109">Permission type</span></span>      | <span data-ttu-id="858d8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="858d8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="858d8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="858d8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="858d8-112">Schedule.Read.All, Group.Read.All,Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="858d8-112">Schedule.Read.All, Group.Read.All,Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="858d8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="858d8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="858d8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="858d8-114">Not supported.</span></span>    |
|<span data-ttu-id="858d8-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="858d8-115">Application</span></span> | <span data-ttu-id="858d8-116">Schedule.Read.All, Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="858d8-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="858d8-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="858d8-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="858d8-118">Глобальные администраторы могут получать доступ к группам, в которых они не являются членами.</span><span class="sxs-lookup"><span data-stu-id="858d8-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="858d8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="858d8-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timeOffReasons
```

## <a name="request-headers"></a><span data-ttu-id="858d8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="858d8-120">Request headers</span></span>

| <span data-ttu-id="858d8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="858d8-121">Header</span></span>       | <span data-ttu-id="858d8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="858d8-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="858d8-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="858d8-123">Authorization</span></span>  | <span data-ttu-id="858d8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="858d8-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="858d8-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="858d8-126">Request body</span></span>
<span data-ttu-id="858d8-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="858d8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="858d8-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="858d8-128">Response</span></span>

<span data-ttu-id="858d8-129">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [timeOffReason](../resources/timeoffreason.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="858d8-129">If successful, this method returns a `200 OK` response code and a collection of [timeOffReason](../resources/timeoffreason.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="858d8-130">Пример</span><span class="sxs-lookup"><span data-stu-id="858d8-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="858d8-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="858d8-131">Request</span></span>

<span data-ttu-id="858d8-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="858d8-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="858d8-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="858d8-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-list-timeoffreasons"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/timeOffReasons
```
# <a name="c"></a>[<span data-ttu-id="858d8-134">C#</span><span class="sxs-lookup"><span data-stu-id="858d8-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-list-timeoffreasons-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="858d8-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="858d8-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-list-timeoffreasons-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="858d8-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="858d8-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-list-timeoffreasons-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="858d8-137">Java</span><span class="sxs-lookup"><span data-stu-id="858d8-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-list-timeoffreasons-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


#### <a name="response"></a><span data-ttu-id="858d8-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="858d8-138">Response</span></span>

<span data-ttu-id="858d8-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="858d8-139">The following is an example of the response.</span></span> 

><span data-ttu-id="858d8-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="858d8-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeOffReason",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "value": [
    {
      "id": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
      "createdDateTime": "2019-03-12T22:10:38.242Z",
      "lastModifiedDateTime": "2019-03-12T22:10:38.242Z",
      "displayName": "Vacation",
      "iconType": "plane",
      "isActive": true,
      "lastModifiedBy": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
          "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
          "displayName": "John Doe"
        }
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get the list of timeOffReason in this schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

