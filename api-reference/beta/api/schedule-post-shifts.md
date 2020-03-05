---
title: Создание смены
description: Создайте новую смену.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 819915ac4291fb2e3d85c9bcd8260ed2fac49308
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453823"
---
# <a name="create-shift"></a><span data-ttu-id="09828-103">Создание смены</span><span class="sxs-lookup"><span data-stu-id="09828-103">Create shift</span></span>

<span data-ttu-id="09828-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="09828-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09828-105">Создайте новый экземпляр [SHIFT](../resources/shift.md) в [расписании](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="09828-105">Create a new [shift](../resources/shift.md) instance in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="09828-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="09828-106">Permissions</span></span>

<span data-ttu-id="09828-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09828-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09828-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="09828-109">Permission type</span></span>      | <span data-ttu-id="09828-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="09828-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="09828-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="09828-111">Delegated (work or school account)</span></span> | <span data-ttu-id="09828-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09828-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="09828-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="09828-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09828-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09828-114">Not supported.</span></span>    |
|<span data-ttu-id="09828-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="09828-115">Application</span></span> | <span data-ttu-id="09828-116">Schedule. ReadWrite. ALL \*</span><span class="sxs-lookup"><span data-stu-id="09828-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="09828-117">\***Важно!** Разрешения на доступ к приложениям в настоящее время доступны только для частного просмотра и недоступны для использования в общедоступном режиме.</span><span class="sxs-lookup"><span data-stu-id="09828-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="09828-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="09828-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="09828-119">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="09828-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="09828-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="09828-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/shifts
```

## <a name="request-headers"></a><span data-ttu-id="09828-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="09828-121">Request headers</span></span>

| <span data-ttu-id="09828-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="09828-122">Header</span></span>       | <span data-ttu-id="09828-123">Значение</span><span class="sxs-lookup"><span data-stu-id="09828-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="09828-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="09828-124">Authorization</span></span>  | <span data-ttu-id="09828-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="09828-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="09828-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="09828-127">Content-Type</span></span>  | <span data-ttu-id="09828-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="09828-p104">application/json. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="09828-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="09828-130">Response</span></span>

<span data-ttu-id="09828-131">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [сдвига](../resources/shift.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="09828-131">If successful, this method returns a `201 Created` response code and a [shift](../resources/shift.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09828-132">Пример</span><span class="sxs-lookup"><span data-stu-id="09828-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="09828-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="09828-133">Request</span></span>

<span data-ttu-id="09828-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="09828-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="09828-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="09828-135">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="09828-136">C#</span><span class="sxs-lookup"><span data-stu-id="09828-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-post-shifts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="09828-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="09828-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-post-shifts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="09828-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="09828-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-post-shifts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="09828-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="09828-139">Response</span></span>

<span data-ttu-id="09828-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="09828-140">The following is an example of the response.</span></span> 

><span data-ttu-id="09828-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="09828-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
