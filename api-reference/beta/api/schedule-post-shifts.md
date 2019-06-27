---
title: Создание смены
description: Создайте новую смену.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a4612b92eb0caa03bae6c460a42bf4f13734d773
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264017"
---
# <a name="create-shift"></a><span data-ttu-id="bda7f-103">Создание смены</span><span class="sxs-lookup"><span data-stu-id="bda7f-103">Create shift</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bda7f-104">Создайте новый экземпляр [SHIFT](../resources/shift.md) в расписании [](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="bda7f-104">Create a new [shift](../resources/shift.md) instance in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bda7f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bda7f-105">Permissions</span></span>

<span data-ttu-id="bda7f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bda7f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bda7f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bda7f-108">Permission type</span></span>      | <span data-ttu-id="bda7f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bda7f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bda7f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bda7f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bda7f-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bda7f-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="bda7f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bda7f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bda7f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bda7f-113">Not supported.</span></span>    |
|<span data-ttu-id="bda7f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bda7f-114">Application</span></span> | <span data-ttu-id="bda7f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bda7f-115">Not supported.</span></span> |

> <span data-ttu-id="bda7f-116">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="bda7f-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="bda7f-117">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="bda7f-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="bda7f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bda7f-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/shifts
```

## <a name="request-headers"></a><span data-ttu-id="bda7f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bda7f-119">Request headers</span></span>

| <span data-ttu-id="bda7f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bda7f-120">Header</span></span>       | <span data-ttu-id="bda7f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="bda7f-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bda7f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bda7f-122">Authorization</span></span>  | <span data-ttu-id="bda7f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bda7f-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bda7f-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bda7f-125">Content-Type</span></span>  | <span data-ttu-id="bda7f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bda7f-126">application/json</span></span>  |

## <a name="response"></a><span data-ttu-id="bda7f-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="bda7f-127">Response</span></span>

<span data-ttu-id="bda7f-128">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [сдвига](../resources/shift.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bda7f-128">If successful, this method returns a `201 Created` response code and a [shift](../resources/shift.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bda7f-129">Пример</span><span class="sxs-lookup"><span data-stu-id="bda7f-129">Example</span></span>

#### <a name="request"></a><span data-ttu-id="bda7f-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="bda7f-130">Request</span></span>

<span data-ttu-id="bda7f-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bda7f-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "schedule-post-shifts"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{teamId}/schedule/shifts
Content-type: application/json

{
  "id": "SHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8",
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "schedulingGroupId": "TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
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

#### <a name="response"></a><span data-ttu-id="bda7f-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="bda7f-132">Response</span></span>

<span data-ttu-id="bda7f-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bda7f-133">The following is an example of the response.</span></span> 

><span data-ttu-id="bda7f-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bda7f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.shift"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 401

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="bda7f-136">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="bda7f-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="bda7f-137">C#</span><span class="sxs-lookup"><span data-stu-id="bda7f-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/schedule-post-shifts-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bda7f-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="bda7f-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/schedule-post-shifts-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="bda7f-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="bda7f-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/schedule-post-shifts-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Creates a new shift",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/schedule-post-shifts.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/schedule-post-shifts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/schedule-post-shifts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
