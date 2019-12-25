---
title: Создание смены
description: Создайте новую смену.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ed3e1e5d908d3683afeebe19a37b640cae567593
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867983"
---
# <a name="create-shift"></a><span data-ttu-id="88d31-103">Создание смены</span><span class="sxs-lookup"><span data-stu-id="88d31-103">Create shift</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88d31-104">Создайте новый экземпляр [SHIFT](../resources/shift.md) в [расписании](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="88d31-104">Create a new [shift](../resources/shift.md) instance in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="88d31-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="88d31-105">Permissions</span></span>

<span data-ttu-id="88d31-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88d31-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88d31-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="88d31-108">Permission type</span></span>      | <span data-ttu-id="88d31-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="88d31-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="88d31-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="88d31-110">Delegated (work or school account)</span></span> | <span data-ttu-id="88d31-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88d31-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="88d31-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="88d31-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88d31-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88d31-113">Not supported.</span></span>    |
|<span data-ttu-id="88d31-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="88d31-114">Application</span></span> | <span data-ttu-id="88d31-115">Schedule. ReadWrite. ALL \*</span><span class="sxs-lookup"><span data-stu-id="88d31-115">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="88d31-116">\***Важно!** Разрешения на доступ к приложениям в настоящее время доступны только для частного просмотра и недоступны для использования в общедоступном режиме.</span><span class="sxs-lookup"><span data-stu-id="88d31-116">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="88d31-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="88d31-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="88d31-118">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="88d31-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="88d31-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="88d31-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/shifts
```

## <a name="request-headers"></a><span data-ttu-id="88d31-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="88d31-120">Request headers</span></span>

| <span data-ttu-id="88d31-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="88d31-121">Header</span></span>       | <span data-ttu-id="88d31-122">Значение</span><span class="sxs-lookup"><span data-stu-id="88d31-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="88d31-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="88d31-123">Authorization</span></span>  | <span data-ttu-id="88d31-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="88d31-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="88d31-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="88d31-126">Content-Type</span></span>  | <span data-ttu-id="88d31-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="88d31-p104">application/json. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="88d31-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="88d31-129">Response</span></span>

<span data-ttu-id="88d31-130">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [сдвига](../resources/shift.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="88d31-130">If successful, this method returns a `201 Created` response code and a [shift](../resources/shift.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88d31-131">Пример</span><span class="sxs-lookup"><span data-stu-id="88d31-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="88d31-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="88d31-132">Request</span></span>

<span data-ttu-id="88d31-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="88d31-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="88d31-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="88d31-134">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="88d31-135">C#</span><span class="sxs-lookup"><span data-stu-id="88d31-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-post-shifts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="88d31-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="88d31-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-post-shifts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="88d31-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="88d31-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-post-shifts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="88d31-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="88d31-138">Response</span></span>

<span data-ttu-id="88d31-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="88d31-139">The following is an example of the response.</span></span> 

><span data-ttu-id="88d31-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="88d31-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
