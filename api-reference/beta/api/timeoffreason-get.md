---
title: Get timeOffReason
description: Получите timeOffReason по ID.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ad314b96290e772a18fb90a935c0eb6bc7392b02
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787340"
---
# <a name="get-timeoffreason"></a><span data-ttu-id="8aa03-103">Get timeOffReason</span><span class="sxs-lookup"><span data-stu-id="8aa03-103">Get timeOffReason</span></span>

<span data-ttu-id="8aa03-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8aa03-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8aa03-105">Извлечение свойств и связей объекта [TimeOffReason](../resources/timeoffreason.md) по ID.</span><span class="sxs-lookup"><span data-stu-id="8aa03-105">Retrieve the properties and relationships of a [timeOffReason](../resources/timeoffreason.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="8aa03-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8aa03-106">Permissions</span></span>

<span data-ttu-id="8aa03-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8aa03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8aa03-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8aa03-109">Permission type</span></span>      | <span data-ttu-id="8aa03-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8aa03-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8aa03-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8aa03-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8aa03-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8aa03-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8aa03-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8aa03-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8aa03-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8aa03-114">Not supported.</span></span>    |
|<span data-ttu-id="8aa03-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="8aa03-115">Application</span></span> | <span data-ttu-id="8aa03-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="8aa03-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span>  |

><span data-ttu-id="8aa03-117">\***Важно:** Разрешения приложения в настоящее время доступны только в закрытом режиме и недоступны для общего пользования.</span><span class="sxs-lookup"><span data-stu-id="8aa03-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="8aa03-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="8aa03-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="8aa03-119">Глобальные администраторы могут получать доступ к группам, в которых они не являются членами.</span><span class="sxs-lookup"><span data-stu-id="8aa03-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="8aa03-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8aa03-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8aa03-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8aa03-121">Optional query parameters</span></span>

<span data-ttu-id="8aa03-122">Этот метод не поддерживает параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8aa03-122">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8aa03-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8aa03-123">Request headers</span></span>

| <span data-ttu-id="8aa03-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8aa03-124">Header</span></span>       | <span data-ttu-id="8aa03-125">Значение</span><span class="sxs-lookup"><span data-stu-id="8aa03-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8aa03-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8aa03-126">Authorization</span></span>  | <span data-ttu-id="8aa03-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8aa03-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8aa03-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8aa03-129">Request body</span></span>
<span data-ttu-id="8aa03-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8aa03-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8aa03-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="8aa03-131">Response</span></span>

<span data-ttu-id="8aa03-132">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект timeOffReason](../resources/timeoffreason.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="8aa03-132">If successful, this method returns a `200 OK` response code and a [timeOffReason](../resources/timeoffreason.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8aa03-133">Пример</span><span class="sxs-lookup"><span data-stu-id="8aa03-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="8aa03-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="8aa03-134">Request</span></span>

<span data-ttu-id="8aa03-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8aa03-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8aa03-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="8aa03-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoffreason-get"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```
# <a name="c"></a>[<span data-ttu-id="8aa03-137">C#</span><span class="sxs-lookup"><span data-stu-id="8aa03-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoffreason-get-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8aa03-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8aa03-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoffreason-get-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8aa03-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8aa03-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoffreason-get-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8aa03-140">Java</span><span class="sxs-lookup"><span data-stu-id="8aa03-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timeoffreason-get-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8aa03-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="8aa03-141">Response</span></span>

<span data-ttu-id="8aa03-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8aa03-142">The following is an example of the response.</span></span> 

><span data-ttu-id="8aa03-143">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8aa03-143">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "description": "Get a timeOffReason by id",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


