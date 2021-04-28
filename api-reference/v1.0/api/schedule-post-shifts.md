---
title: Создание смены
description: Создайте новую смену.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a8e9cfcbc94d31f08ea7c2fc743a59bd1a1a7513
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053862"
---
# <a name="create-shift"></a><span data-ttu-id="0060f-103">Создание смены</span><span class="sxs-lookup"><span data-stu-id="0060f-103">Create shift</span></span>

<span data-ttu-id="0060f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0060f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0060f-105">Создание нового [экземпляра переноса](../resources/shift.md) в [расписании.](../resources/schedule.md)</span><span class="sxs-lookup"><span data-stu-id="0060f-105">Create a new [shift](../resources/shift.md) instance in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0060f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0060f-106">Permissions</span></span>

<span data-ttu-id="0060f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0060f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0060f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0060f-109">Permission type</span></span>      | <span data-ttu-id="0060f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0060f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0060f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0060f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0060f-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0060f-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0060f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0060f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0060f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0060f-114">Not supported.</span></span>    |
|<span data-ttu-id="0060f-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="0060f-115">Application</span></span> | <span data-ttu-id="0060f-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0060f-116">Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0060f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0060f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/shifts
```

## <a name="request-headers"></a><span data-ttu-id="0060f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0060f-118">Request headers</span></span>

| <span data-ttu-id="0060f-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0060f-119">Header</span></span>       | <span data-ttu-id="0060f-120">Значение</span><span class="sxs-lookup"><span data-stu-id="0060f-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0060f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0060f-121">Authorization</span></span>  | <span data-ttu-id="0060f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0060f-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0060f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0060f-124">Content-Type</span></span>  | <span data-ttu-id="0060f-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0060f-p103">application/json. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="0060f-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="0060f-127">Response</span></span>

<span data-ttu-id="0060f-128">В случае успешной работы этот метод возвращает код отклика и объект `201 Created` [переноса](../resources/shift.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="0060f-128">If successful, this method returns a `201 Created` response code and a [shift](../resources/shift.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0060f-129">Пример</span><span class="sxs-lookup"><span data-stu-id="0060f-129">Example</span></span>

#### <a name="request"></a><span data-ttu-id="0060f-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="0060f-130">Request</span></span>

<span data-ttu-id="0060f-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0060f-131">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0060f-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="0060f-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-post-shifts"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/shifts
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
# <a name="c"></a>[<span data-ttu-id="0060f-133">C#</span><span class="sxs-lookup"><span data-stu-id="0060f-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-post-shifts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0060f-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0060f-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-post-shifts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0060f-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0060f-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-post-shifts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0060f-136">Java</span><span class="sxs-lookup"><span data-stu-id="0060f-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-post-shifts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


#### <a name="response"></a><span data-ttu-id="0060f-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="0060f-137">Response</span></span>

<span data-ttu-id="0060f-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0060f-138">The following is an example of the response.</span></span> 

><span data-ttu-id="0060f-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0060f-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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

