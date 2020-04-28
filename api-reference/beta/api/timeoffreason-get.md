---
title: Получение Тимеоффреасон
description: Получение Тимеоффреасон по ИДЕНТИФИКАТОРу.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: cb9c436537e233c14e4f9d9eb1a2c6cb01cc6fe2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452290"
---
# <a name="get-timeoffreason"></a><span data-ttu-id="a09ab-103">Получение Тимеоффреасон</span><span class="sxs-lookup"><span data-stu-id="a09ab-103">Get timeOffReason</span></span>

<span data-ttu-id="a09ab-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a09ab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a09ab-105">Получение свойств и связей объекта [тимеоффреасон](../resources/timeoffreason.md) по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="a09ab-105">Retrieve the properties and relationships of a [timeOffReason](../resources/timeoffreason.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="a09ab-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a09ab-106">Permissions</span></span>

<span data-ttu-id="a09ab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a09ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a09ab-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a09ab-109">Permission type</span></span>      | <span data-ttu-id="a09ab-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a09ab-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a09ab-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a09ab-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a09ab-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a09ab-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a09ab-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a09ab-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a09ab-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a09ab-114">Not supported.</span></span>    |
|<span data-ttu-id="a09ab-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a09ab-115">Application</span></span> | <span data-ttu-id="a09ab-116">Schedule. Read. All *, Schedule. ReadWrite. ALL*</span><span class="sxs-lookup"><span data-stu-id="a09ab-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span>  |

><span data-ttu-id="a09ab-117">\***Важно!** Разрешения на доступ к приложениям в настоящее время доступны только для частного просмотра и недоступны для использования в общедоступном режиме.</span><span class="sxs-lookup"><span data-stu-id="a09ab-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="a09ab-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="a09ab-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="a09ab-119">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="a09ab-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="a09ab-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a09ab-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

## <a name="request-headers"></a><span data-ttu-id="a09ab-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a09ab-121">Request headers</span></span>

| <span data-ttu-id="a09ab-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a09ab-122">Header</span></span>       | <span data-ttu-id="a09ab-123">Значение</span><span class="sxs-lookup"><span data-stu-id="a09ab-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a09ab-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a09ab-124">Authorization</span></span>  | <span data-ttu-id="a09ab-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a09ab-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a09ab-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a09ab-127">Request body</span></span>
<span data-ttu-id="a09ab-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a09ab-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a09ab-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="a09ab-129">Response</span></span>

<span data-ttu-id="a09ab-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [тимеоффреасон](../resources/timeoffreason.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a09ab-130">If successful, this method returns a `200 OK` response code and a [timeOffReason](../resources/timeoffreason.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a09ab-131">Пример</span><span class="sxs-lookup"><span data-stu-id="a09ab-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a09ab-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a09ab-132">Request</span></span>

<span data-ttu-id="a09ab-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a09ab-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a09ab-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="a09ab-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoffreason-get"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```
# <a name="c"></a>[<span data-ttu-id="a09ab-135">C#</span><span class="sxs-lookup"><span data-stu-id="a09ab-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoffreason-get-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a09ab-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a09ab-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoffreason-get-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a09ab-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a09ab-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoffreason-get-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a09ab-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="a09ab-138">Response</span></span>

<span data-ttu-id="a09ab-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a09ab-139">The following is an example of the response.</span></span> 

><span data-ttu-id="a09ab-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a09ab-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
