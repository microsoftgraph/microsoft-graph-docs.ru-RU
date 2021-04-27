---
title: Замените timeOffReason
description: Замените существующее времяOffReason.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 247b15e3d522100ee8d286fbd01d12efcaf7ad76
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048948"
---
# <a name="replace-timeoffreason"></a><span data-ttu-id="b77bf-103">Замените timeOffReason</span><span class="sxs-lookup"><span data-stu-id="b77bf-103">Replace timeOffReason</span></span>

<span data-ttu-id="b77bf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b77bf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b77bf-105">Замените [существующее времяOffReason](../resources/timeoffreason.md).</span><span class="sxs-lookup"><span data-stu-id="b77bf-105">Replace an existing [timeOffReason](../resources/timeoffreason.md).</span></span>

<span data-ttu-id="b77bf-106">Если указанного [времениOffReason](../resources/timeoffreason.md) не существует, этот метод `404 Not found` возвращается.</span><span class="sxs-lookup"><span data-stu-id="b77bf-106">If the specified [timeOffReason](../resources/timeoffreason.md) doesn't exist, this method returns `404 Not found`.</span></span>

## <a name="permissions"></a><span data-ttu-id="b77bf-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b77bf-107">Permissions</span></span>

<span data-ttu-id="b77bf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b77bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b77bf-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b77bf-110">Permission type</span></span>      | <span data-ttu-id="b77bf-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b77bf-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b77bf-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b77bf-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b77bf-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b77bf-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b77bf-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b77bf-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b77bf-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b77bf-115">Not supported.</span></span>    |
|<span data-ttu-id="b77bf-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="b77bf-116">Application</span></span> | <span data-ttu-id="b77bf-117">Schedule.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="b77bf-117">Schedule.ReadWrite.All\*</span></span>  |

><span data-ttu-id="b77bf-118">\***Важно:** Разрешения приложения в настоящее время доступны только в закрытом режиме и недоступны для общего пользования.</span><span class="sxs-lookup"><span data-stu-id="b77bf-118">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="b77bf-119">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="b77bf-119">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="b77bf-120">Глобальные администраторы могут получать доступ к группам, в которых они не являются членами.</span><span class="sxs-lookup"><span data-stu-id="b77bf-120">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="b77bf-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b77bf-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

## <a name="request-headers"></a><span data-ttu-id="b77bf-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b77bf-122">Request headers</span></span>

| <span data-ttu-id="b77bf-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b77bf-123">Header</span></span>       | <span data-ttu-id="b77bf-124">Значение</span><span class="sxs-lookup"><span data-stu-id="b77bf-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b77bf-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b77bf-125">Authorization</span></span>  | <span data-ttu-id="b77bf-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b77bf-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b77bf-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b77bf-128">Content-Type</span></span>  | <span data-ttu-id="b77bf-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b77bf-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b77bf-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b77bf-131">Request body</span></span>

<span data-ttu-id="b77bf-132">В теле запроса поставляем представление JSON объекта [TimeOffReason.](../resources/timeoffreason.md)</span><span class="sxs-lookup"><span data-stu-id="b77bf-132">In the request body, supply a JSON representation of a [timeOffReason](../resources/timeoffreason.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b77bf-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="b77bf-133">Response</span></span>

<span data-ttu-id="b77bf-134">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект timeOffReason](../resources/timeoffreason.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b77bf-134">If successful, this method returns a `200 OK` response code and a [timeOffReason](../resources/timeoffreason.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b77bf-135">Пример</span><span class="sxs-lookup"><span data-stu-id="b77bf-135">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b77bf-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="b77bf-136">Request</span></span>

<span data-ttu-id="b77bf-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b77bf-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b77bf-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="b77bf-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoffreason-put"
}-->
```http
PUT https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
Content-type: application/json
Prefer: return=representation

{
  "displayName": "Vacation",
  "iconType": "plane",
  "isActive": true
}
```
# <a name="c"></a>[<span data-ttu-id="b77bf-139">C#</span><span class="sxs-lookup"><span data-stu-id="b77bf-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoffreason-put-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b77bf-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b77bf-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoffreason-put-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b77bf-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b77bf-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoffreason-put-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b77bf-142">Java</span><span class="sxs-lookup"><span data-stu-id="b77bf-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timeoffreason-put-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b77bf-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="b77bf-143">Response</span></span>

<span data-ttu-id="b77bf-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b77bf-144">The following is an example of the response.</span></span> 

><span data-ttu-id="b77bf-145">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b77bf-145">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeOffReason"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

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
      "displayName": "Alex Wilbur"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Replace an existing timeOffReason",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


