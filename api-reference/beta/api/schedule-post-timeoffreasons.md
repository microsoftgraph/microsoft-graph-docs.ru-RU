---
title: Создание Тимеоффреасон
description: Создание нового Тимеоффреасон.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 0f12d104db2748d5277565326b54d083bea8cdee
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35457585"
---
# <a name="create-timeoffreason"></a><span data-ttu-id="a33d2-103">Создание Тимеоффреасон</span><span class="sxs-lookup"><span data-stu-id="a33d2-103">Create timeOffReason</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a33d2-104">Создание нового [тимеоффреасон](../resources/timeoffreason.md).</span><span class="sxs-lookup"><span data-stu-id="a33d2-104">Create a new [timeOffReason](../resources/timeoffreason.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a33d2-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a33d2-105">Permissions</span></span>

<span data-ttu-id="a33d2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a33d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a33d2-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a33d2-108">Permission type</span></span>      | <span data-ttu-id="a33d2-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a33d2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a33d2-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a33d2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a33d2-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a33d2-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a33d2-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a33d2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a33d2-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a33d2-113">Not supported.</span></span>    |
|<span data-ttu-id="a33d2-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a33d2-114">Application</span></span> | <span data-ttu-id="a33d2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a33d2-115">Not supported.</span></span> |

> <span data-ttu-id="a33d2-116">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="a33d2-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="a33d2-117">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="a33d2-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="a33d2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a33d2-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timeOffReasons
```

## <a name="request-headers"></a><span data-ttu-id="a33d2-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a33d2-119">Request headers</span></span>

| <span data-ttu-id="a33d2-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a33d2-120">Header</span></span>       | <span data-ttu-id="a33d2-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a33d2-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a33d2-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a33d2-122">Authorization</span></span>  | <span data-ttu-id="a33d2-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a33d2-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a33d2-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a33d2-125">Content-Type</span></span>  | <span data-ttu-id="a33d2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a33d2-126">application/json</span></span>  |

## <a name="response"></a><span data-ttu-id="a33d2-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="a33d2-127">Response</span></span>

<span data-ttu-id="a33d2-128">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [тимеоффреасон](../resources/timeoffreason.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a33d2-128">If successful, this method returns a `201 Created` response code and a [timeOffReason](../resources/timeoffreason.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a33d2-129">Пример</span><span class="sxs-lookup"><span data-stu-id="a33d2-129">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a33d2-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="a33d2-130">Request</span></span>

<span data-ttu-id="a33d2-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a33d2-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a33d2-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="a33d2-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-post-timeoffreasons"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffReasons
Content-type: application/json

{
  "displayName": "Vacation",
  "iconType": "plane",
  "isActive": true
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a33d2-133">C#</span><span class="sxs-lookup"><span data-stu-id="a33d2-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-post-timeoffreasons-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a33d2-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="a33d2-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-post-timeoffreasons-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a33d2-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="a33d2-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-post-timeoffreasons-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a33d2-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="a33d2-136">Response</span></span>

<span data-ttu-id="a33d2-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a33d2-137">The following is an example of the response.</span></span> 

><span data-ttu-id="a33d2-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a33d2-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
