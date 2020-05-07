---
title: Замена Тимеоффреасон
description: Замена существующего Тимеоффреасон.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3719ac2dedc45854bab2b2f82bde19fe1af2f6d2
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2020
ms.locfileid: "44155007"
---
# <a name="replace-timeoffreason"></a><span data-ttu-id="293bb-103">Замена Тимеоффреасон</span><span class="sxs-lookup"><span data-stu-id="293bb-103">Replace timeOffReason</span></span>

<span data-ttu-id="293bb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="293bb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="293bb-105">Замена существующего [тимеоффреасон](../resources/timeoffreason.md).</span><span class="sxs-lookup"><span data-stu-id="293bb-105">Replace an existing [timeOffReason](../resources/timeoffreason.md).</span></span>

<span data-ttu-id="293bb-106">Если указанный [тимеоффреасон](../resources/timeoffreason.md) не существует, этот метод возвращает значение `404 Not found`.</span><span class="sxs-lookup"><span data-stu-id="293bb-106">If the specified [timeOffReason](../resources/timeoffreason.md) doesn't exist, this method returns `404 Not found`.</span></span>

## <a name="permissions"></a><span data-ttu-id="293bb-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="293bb-107">Permissions</span></span>

<span data-ttu-id="293bb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="293bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="293bb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="293bb-110">Permission type</span></span>      | <span data-ttu-id="293bb-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="293bb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="293bb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="293bb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="293bb-113">Запланируйте. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="293bb-113">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="293bb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="293bb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="293bb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="293bb-115">Not supported.</span></span>    |
|<span data-ttu-id="293bb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="293bb-116">Application</span></span> | <span data-ttu-id="293bb-117">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="293bb-117">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="293bb-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="293bb-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="293bb-119">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="293bb-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="293bb-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="293bb-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

## <a name="request-headers"></a><span data-ttu-id="293bb-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="293bb-121">Request headers</span></span>

| <span data-ttu-id="293bb-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="293bb-122">Header</span></span>       | <span data-ttu-id="293bb-123">Значение</span><span class="sxs-lookup"><span data-stu-id="293bb-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="293bb-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="293bb-124">Authorization</span></span>  | <span data-ttu-id="293bb-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="293bb-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="293bb-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="293bb-127">Content-Type</span></span>  | <span data-ttu-id="293bb-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="293bb-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="293bb-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="293bb-130">Request body</span></span>

<span data-ttu-id="293bb-131">В тексте запроса добавьте представление объекта [тимеоффреасон](../resources/timeoffreason.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="293bb-131">In the request body, supply a JSON representation of a [timeOffReason](../resources/timeoffreason.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="293bb-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="293bb-132">Response</span></span>

<span data-ttu-id="293bb-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [тимеоффреасон](../resources/timeoffreason.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="293bb-133">If successful, this method returns a `200 OK` response code and a [timeOffReason](../resources/timeoffreason.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="293bb-134">Пример</span><span class="sxs-lookup"><span data-stu-id="293bb-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="293bb-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="293bb-135">Request</span></span>

<span data-ttu-id="293bb-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="293bb-136">The following is an example of the request.</span></span>

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
---


### <a name="response"></a><span data-ttu-id="293bb-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="293bb-137">Response</span></span>

<span data-ttu-id="293bb-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="293bb-138">The following is an example of the response.</span></span> 

><span data-ttu-id="293bb-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="293bb-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
