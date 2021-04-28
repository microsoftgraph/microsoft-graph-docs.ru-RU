---
title: Создание timeOffReason
description: Создание нового timeOffReason.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6d57e287bee995f28cc738ac7a9b505ed143c59b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050348"
---
# <a name="create-timeoffreason"></a><span data-ttu-id="5054f-103">Создание timeOffReason</span><span class="sxs-lookup"><span data-stu-id="5054f-103">Create timeOffReason</span></span>

<span data-ttu-id="5054f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5054f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5054f-105">Создание нового [timeOffReason](../resources/timeoffreason.md).</span><span class="sxs-lookup"><span data-stu-id="5054f-105">Create a new [timeOffReason](../resources/timeoffreason.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5054f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5054f-106">Permissions</span></span>

<span data-ttu-id="5054f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5054f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5054f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5054f-109">Permission type</span></span>      | <span data-ttu-id="5054f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5054f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5054f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5054f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5054f-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5054f-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5054f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5054f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5054f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5054f-114">Not supported.</span></span>    |
|<span data-ttu-id="5054f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5054f-115">Application</span></span> | <span data-ttu-id="5054f-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5054f-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="5054f-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="5054f-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="5054f-118">Глобальные администраторы могут получать доступ к группам, в которых они не являются членами.</span><span class="sxs-lookup"><span data-stu-id="5054f-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="5054f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5054f-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timeOffReasons
```

## <a name="request-headers"></a><span data-ttu-id="5054f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5054f-120">Request headers</span></span>

| <span data-ttu-id="5054f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5054f-121">Header</span></span>       | <span data-ttu-id="5054f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5054f-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5054f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5054f-123">Authorization</span></span>  | <span data-ttu-id="5054f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5054f-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5054f-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5054f-126">Content-Type</span></span>  | <span data-ttu-id="5054f-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5054f-p104">application/json. Required.</span></span>  |

## <a name="response"></a><span data-ttu-id="5054f-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="5054f-129">Response</span></span>

<span data-ttu-id="5054f-130">В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект timeOffReason](../resources/timeoffreason.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="5054f-130">If successful, this method returns a `201 Created` response code and a [timeOffReason](../resources/timeoffreason.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5054f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="5054f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="5054f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="5054f-132">Request</span></span>

<span data-ttu-id="5054f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5054f-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5054f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="5054f-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-post-timeoffreasons"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/timeOffReasons
Content-type: application/json

{
  "displayName": "Vacation",
  "iconType": "plane",
  "isActive": true
}
```
# <a name="c"></a>[<span data-ttu-id="5054f-135">C#</span><span class="sxs-lookup"><span data-stu-id="5054f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-post-timeoffreasons-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5054f-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5054f-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-post-timeoffreasons-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5054f-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5054f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-post-timeoffreasons-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5054f-138">Java</span><span class="sxs-lookup"><span data-stu-id="5054f-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-post-timeoffreasons-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="5054f-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="5054f-139">Response</span></span>

<span data-ttu-id="5054f-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5054f-140">The following is an example of the response.</span></span> 

><span data-ttu-id="5054f-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5054f-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeOffReason"
} -->

```http
HTTP/1.1 201 Created
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
      "displayName": "John Doe"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Creates a new timeOffReason",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

