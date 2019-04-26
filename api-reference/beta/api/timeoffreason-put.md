---
title: Замена Тимеоффреасон
description: Замена существующего Тимеоффреасон.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 18e3130e87d3c47a636c6190a593b7dc7539b806
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33330430"
---
# <a name="replace-timeoffreason"></a><span data-ttu-id="b9aec-103">Замена Тимеоффреасон</span><span class="sxs-lookup"><span data-stu-id="b9aec-103">Replace timeOffReason</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9aec-104">Замена существующего [тимеоффреасон](../resources/timeoffreason.md).</span><span class="sxs-lookup"><span data-stu-id="b9aec-104">Replace an existing [timeOffReason](../resources/timeoffreason.md).</span></span>

<span data-ttu-id="b9aec-105">Если указанный [тимеоффреасон](../resources/timeoffreason.md) не существует, этот метод возвращает значение `404 Not found`.</span><span class="sxs-lookup"><span data-stu-id="b9aec-105">If the specified [timeOffReason](../resources/timeoffreason.md) doesn't exist, this method returns `404 Not found`.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9aec-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b9aec-106">Permissions</span></span>

<span data-ttu-id="b9aec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9aec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9aec-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b9aec-109">Permission type</span></span>      | <span data-ttu-id="b9aec-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b9aec-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9aec-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b9aec-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b9aec-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9aec-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b9aec-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b9aec-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9aec-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9aec-114">Not supported.</span></span>    |
|<span data-ttu-id="b9aec-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b9aec-115">Application</span></span> | <span data-ttu-id="b9aec-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9aec-116">Not supported.</span></span> |

> <span data-ttu-id="b9aec-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="b9aec-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="b9aec-118">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="b9aec-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="b9aec-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b9aec-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

## <a name="request-headers"></a><span data-ttu-id="b9aec-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b9aec-120">Request headers</span></span>

| <span data-ttu-id="b9aec-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b9aec-121">Header</span></span>       | <span data-ttu-id="b9aec-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b9aec-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b9aec-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b9aec-123">Authorization</span></span>  | <span data-ttu-id="b9aec-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b9aec-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b9aec-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b9aec-126">Content-Type</span></span>  | <span data-ttu-id="b9aec-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b9aec-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b9aec-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b9aec-128">Request body</span></span>

<span data-ttu-id="b9aec-129">В тексте запроса добавьте представление объекта [Тимеоффреасон](../resources/timeoffreason.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b9aec-129">In the request body, supply a JSON representation of a [timeOffReason](../resources/timeoffreason.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b9aec-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9aec-130">Response</span></span>

<span data-ttu-id="b9aec-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [тимеоффреасон](../resources/timeoffreason.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b9aec-131">If successful, this method returns a `200 OK` response code and a [timeOffReason](../resources/timeoffreason.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9aec-132">Пример</span><span class="sxs-lookup"><span data-stu-id="b9aec-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b9aec-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b9aec-133">Request</span></span>

<span data-ttu-id="b9aec-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b9aec-134">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="b9aec-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9aec-135">Response</span></span>

<span data-ttu-id="b9aec-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b9aec-136">The following is an example of the response.</span></span> 

><span data-ttu-id="b9aec-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b9aec-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
