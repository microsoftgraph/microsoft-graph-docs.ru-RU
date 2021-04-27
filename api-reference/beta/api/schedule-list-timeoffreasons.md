---
title: Список timeOffReasons
description: Получите список timeOffReasons в расписании.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 428ede3f9f91f4239651f3a8efeb59f5faa4cebf
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052742"
---
# <a name="list-timeoffreasons"></a><span data-ttu-id="73a07-103">Список timeOffReasons</span><span class="sxs-lookup"><span data-stu-id="73a07-103">List timeOffReasons</span></span>

<span data-ttu-id="73a07-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73a07-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="73a07-105">Получите список [timeOffReasons в](../resources/timeoffreason.md) [расписании.](../resources/schedule.md)</span><span class="sxs-lookup"><span data-stu-id="73a07-105">Get the list of [timeOffReasons](../resources/timeoffreason.md) in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="73a07-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="73a07-106">Permissions</span></span>

<span data-ttu-id="73a07-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73a07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73a07-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="73a07-109">Permission type</span></span>      | <span data-ttu-id="73a07-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="73a07-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73a07-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="73a07-111">Delegated (work or school account)</span></span> | <span data-ttu-id="73a07-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73a07-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="73a07-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="73a07-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73a07-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73a07-114">Not supported.</span></span>    |
|<span data-ttu-id="73a07-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="73a07-115">Application</span></span> | <span data-ttu-id="73a07-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="73a07-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span> |

><span data-ttu-id="73a07-117">\***Важно:** Разрешения приложения в настоящее время доступны только в закрытом режиме и недоступны для общего пользования.</span><span class="sxs-lookup"><span data-stu-id="73a07-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="73a07-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="73a07-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="73a07-119">Глобальные администраторы могут получать доступ к группам, в которых они не являются членами.</span><span class="sxs-lookup"><span data-stu-id="73a07-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="73a07-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="73a07-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timeOffReasons
```

## <a name="request-headers"></a><span data-ttu-id="73a07-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="73a07-121">Request headers</span></span>

| <span data-ttu-id="73a07-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="73a07-122">Header</span></span>       | <span data-ttu-id="73a07-123">Значение</span><span class="sxs-lookup"><span data-stu-id="73a07-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="73a07-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="73a07-124">Authorization</span></span>  | <span data-ttu-id="73a07-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="73a07-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="73a07-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="73a07-127">Request body</span></span>
<span data-ttu-id="73a07-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="73a07-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73a07-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="73a07-129">Response</span></span>

<span data-ttu-id="73a07-130">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [timeOffReason](../resources/timeoffreason.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="73a07-130">If successful, this method returns a `200 OK` response code and a collection of [timeOffReason](../resources/timeoffreason.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73a07-131">Пример</span><span class="sxs-lookup"><span data-stu-id="73a07-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="73a07-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="73a07-132">Request</span></span>

<span data-ttu-id="73a07-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="73a07-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="73a07-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="73a07-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-list-timeoffreasons"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffReasons
```
# <a name="c"></a>[<span data-ttu-id="73a07-135">C#</span><span class="sxs-lookup"><span data-stu-id="73a07-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-list-timeoffreasons-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="73a07-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="73a07-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-list-timeoffreasons-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="73a07-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="73a07-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-list-timeoffreasons-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="73a07-138">Java</span><span class="sxs-lookup"><span data-stu-id="73a07-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-list-timeoffreasons-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="73a07-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="73a07-139">Response</span></span>

<span data-ttu-id="73a07-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="73a07-140">The following is an example of the response.</span></span> 

><span data-ttu-id="73a07-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="73a07-141">**Note:** The response object shown here might be shortened for readability.</span></span>
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


