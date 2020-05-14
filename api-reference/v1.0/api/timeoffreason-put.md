---
title: Замена Тимеоффреасон
description: Замена существующего Тимеоффреасон.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e5736e70125af9ba41d9c2017171865717797998
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2020
ms.locfileid: "44218295"
---
# <a name="replace-timeoffreason"></a><span data-ttu-id="71e6f-103">Замена Тимеоффреасон</span><span class="sxs-lookup"><span data-stu-id="71e6f-103">Replace timeOffReason</span></span>

<span data-ttu-id="71e6f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71e6f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="71e6f-105">Замена существующего [тимеоффреасон](../resources/timeoffreason.md).</span><span class="sxs-lookup"><span data-stu-id="71e6f-105">Replace an existing [timeOffReason](../resources/timeoffreason.md).</span></span>

<span data-ttu-id="71e6f-106">Если указанный [тимеоффреасон](../resources/timeoffreason.md) не существует, этот метод возвращает значение `404 Not found` .</span><span class="sxs-lookup"><span data-stu-id="71e6f-106">If the specified [timeOffReason](../resources/timeoffreason.md) doesn't exist, this method returns `404 Not found`.</span></span>

## <a name="permissions"></a><span data-ttu-id="71e6f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="71e6f-107">Permissions</span></span>

<span data-ttu-id="71e6f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71e6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71e6f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71e6f-110">Permission type</span></span>      | <span data-ttu-id="71e6f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="71e6f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71e6f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71e6f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="71e6f-113">Запланируйте. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="71e6f-113">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="71e6f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71e6f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71e6f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71e6f-115">Not supported.</span></span>    |
|<span data-ttu-id="71e6f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="71e6f-116">Application</span></span> | <span data-ttu-id="71e6f-117">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71e6f-117">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="71e6f-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="71e6f-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="71e6f-119">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="71e6f-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="71e6f-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71e6f-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

## <a name="request-headers"></a><span data-ttu-id="71e6f-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="71e6f-121">Request headers</span></span>

| <span data-ttu-id="71e6f-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="71e6f-122">Header</span></span>       | <span data-ttu-id="71e6f-123">Значение</span><span class="sxs-lookup"><span data-stu-id="71e6f-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="71e6f-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="71e6f-124">Authorization</span></span>  | <span data-ttu-id="71e6f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="71e6f-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="71e6f-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="71e6f-127">Content-Type</span></span>  | <span data-ttu-id="71e6f-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="71e6f-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="71e6f-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="71e6f-130">Request body</span></span>

<span data-ttu-id="71e6f-131">В тексте запроса добавьте представление объекта [тимеоффреасон](../resources/timeoffreason.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="71e6f-131">In the request body, supply a JSON representation of a [timeOffReason](../resources/timeoffreason.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="71e6f-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="71e6f-132">Response</span></span>

<span data-ttu-id="71e6f-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [тимеоффреасон](../resources/timeoffreason.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="71e6f-133">If successful, this method returns a `200 OK` response code and a [timeOffReason](../resources/timeoffreason.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71e6f-134">Пример</span><span class="sxs-lookup"><span data-stu-id="71e6f-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="71e6f-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="71e6f-135">Request</span></span>

<span data-ttu-id="71e6f-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="71e6f-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="71e6f-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="71e6f-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoffreason-put"
}-->
```http
PUT https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
Content-type: application/json
Prefer: return=representation

{
  "displayName": "Vacation",
  "iconType": "plane",
  "isActive": true
}
```
# <a name="c"></a>[<span data-ttu-id="71e6f-138">C#</span><span class="sxs-lookup"><span data-stu-id="71e6f-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoffreason-put-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="71e6f-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71e6f-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoffreason-put-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="71e6f-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="71e6f-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoffreason-put-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="71e6f-141">Java</span><span class="sxs-lookup"><span data-stu-id="71e6f-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timeoffreason-put-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="71e6f-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="71e6f-142">Response</span></span>

<span data-ttu-id="71e6f-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="71e6f-143">The following is an example of the response.</span></span> 

><span data-ttu-id="71e6f-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="71e6f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
