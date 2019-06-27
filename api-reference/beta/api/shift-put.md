---
title: Замена Shift
description: Замените существующую смену.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: af8c8af020521c6db3a353efe633d070588a44cb
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271647"
---
# <a name="replace-shift"></a><span data-ttu-id="b0580-103">Замена Shift</span><span class="sxs-lookup"><span data-stu-id="b0580-103">Replace shift</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0580-104">Замените существующую [смену](../resources/shift.md).</span><span class="sxs-lookup"><span data-stu-id="b0580-104">Replace an existing [shift](../resources/shift.md).</span></span>

<span data-ttu-id="b0580-105">Если указанная [Смена](../resources/shift.md) не существует, этот метод возвращает `404 Not found`значение.</span><span class="sxs-lookup"><span data-stu-id="b0580-105">If the specified [shift](../resources/shift.md) doesn't exist, this method returns `404 Not found`.</span></span>

## <a name="permissions"></a><span data-ttu-id="b0580-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b0580-106">Permissions</span></span>

<span data-ttu-id="b0580-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0580-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0580-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b0580-109">Permission type</span></span>      | <span data-ttu-id="b0580-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b0580-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b0580-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b0580-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b0580-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0580-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b0580-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b0580-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0580-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0580-114">Not supported.</span></span>    |
|<span data-ttu-id="b0580-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b0580-115">Application</span></span> | <span data-ttu-id="b0580-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0580-116">Not supported.</span></span> |

> <span data-ttu-id="b0580-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="b0580-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="b0580-118">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="b0580-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="b0580-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b0580-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/shifts/{shiftId}
```

## <a name="request-headers"></a><span data-ttu-id="b0580-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b0580-120">Request headers</span></span>

| <span data-ttu-id="b0580-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b0580-121">Header</span></span>       | <span data-ttu-id="b0580-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b0580-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b0580-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b0580-123">Authorization</span></span>  | <span data-ttu-id="b0580-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b0580-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b0580-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b0580-126">Content-Type</span></span>  | <span data-ttu-id="b0580-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b0580-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b0580-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b0580-128">Request body</span></span>

<span data-ttu-id="b0580-129">В тексте запроса добавьте представление объекта сдвига в формате [](../resources/shift.md) JSON.</span><span class="sxs-lookup"><span data-stu-id="b0580-129">In the request body, supply a JSON representation of a [shift](../resources/shift.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b0580-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0580-130">Response</span></span>

<span data-ttu-id="b0580-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [сдвига](../resources/shift.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b0580-131">If successful, this method returns a `200 OK` response code and a [shift](../resources/shift.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0580-132">Пример</span><span class="sxs-lookup"><span data-stu-id="b0580-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b0580-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b0580-133">Request</span></span>

<span data-ttu-id="b0580-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b0580-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "shift-put"
}-->
```http
PUT https://graph.microsoft.com/beta/teams/{teamId}/schedule/shifts/{shiftId}
Content-type: application/json
Prefer: return=representation

{
  "id": "SHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8",
  "createdDateTime": "2019-03-14T04:32:51.451Z",
  "lastModifiedDateTime": "2019-03-14T05:32:51.451Z",
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "schedulingGroupId": "TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  },
  "sharedShift": {
    "displayName": "Day shift",
    "notes": "Please do inventory as part of your shift.",
    "startDateTime": "2019-03-11T15:00:00Z",
    "endDateTime": "2019-03-12T00:00:00Z",
    "theme": "blue",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2019-03-11T15:00:00Z",
        "endDateTime": "2019-03-11T15:15:00Z",
        "code": "",
        "displayName": "Lunch"
      }
    ]
  },
  "draftShift": {
    "displayName": "Day shift",
    "notes": "Please do inventory as part of your shift.",
    "startDateTime": "2019-03-11T15:00:00Z",
    "endDateTime": "2019-03-12T00:00:00Z",
    "theme": "blue",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2019-03-11T15:00:00Z",
        "endDateTime": "2019-03-11T15:30:00Z",
        "code": "",
        "displayName": "Lunch"
      }
    ]
  }
}
```

#### <a name="response"></a><span data-ttu-id="b0580-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0580-135">Response</span></span>

<span data-ttu-id="b0580-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b0580-136">The following is an example of the response.</span></span> 

><span data-ttu-id="b0580-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b0580-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.shift"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "id": "string",
  "userId": "string",
  "schedulingGroupId": "string",
  "sharedShift": {
    "notes": "string",
    "displayName": "string",
    "startDateTime": "2018-10-04T00:58:45.340Z",
    "endDateTime": "2018-10-04T00:58:45.340Z",
    "theme": "white",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2018-10-04T00:58:45.340Z",
        "endDateTime": "2018-10-04T00:58:45.340Z",
        "code": "string",
        "displayName": "string"
      }
    ]
  },
  "draftShift": {
    "notes": "string",
    "displayName": "string",
    "startDateTime": "2018-10-04T00:58:45.340Z",
    "endDateTime": "2018-10-04T00:58:45.340Z",
    "theme": "white",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2018-10-04T00:58:45.340Z",
        "endDateTime": "2018-10-04T00:58:45.340Z",
        "code": "string",
        "displayName": "string"
      }
    ]
  },
  "createdDateTime": "2018-10-04T00:58:45.340Z",
  "lastModifiedDateTime": "2018-10-04T00:58:45.340Z",
  "lastModifiedBy": {
    "user": {
      "id": "string",
      "displayName": "string"
    },
    "application": {
      "id": "string",
      "displayName": "string"
    },
    "device": {
      "id": "string",
      "displayName": "string"
    }
  }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="b0580-139">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="b0580-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b0580-140">C#</span><span class="sxs-lookup"><span data-stu-id="b0580-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/shift-put-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b0580-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="b0580-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/shift-put-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="b0580-142">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b0580-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/shift-put-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Replace an existing shift",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/shift-put.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/shift-put.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/shift-put.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
