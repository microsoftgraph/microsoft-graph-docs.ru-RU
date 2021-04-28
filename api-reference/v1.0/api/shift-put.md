---
title: Замена смены
description: Замените существующую смену.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 888932c4732bca7f15a5eb61327cda9bb554b762
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52034898"
---
# <a name="replace-shift"></a><span data-ttu-id="ebdb7-103">Замена смены</span><span class="sxs-lookup"><span data-stu-id="ebdb7-103">Replace shift</span></span>

<span data-ttu-id="ebdb7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ebdb7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ebdb7-105">Замените [существующий сдвиг.](../resources/shift.md)</span><span class="sxs-lookup"><span data-stu-id="ebdb7-105">Replace an existing [shift](../resources/shift.md).</span></span>

<span data-ttu-id="ebdb7-106">Если указанной [смены](../resources/shift.md) не существует, этот метод `404 Not found` возвращается.</span><span class="sxs-lookup"><span data-stu-id="ebdb7-106">If the specified [shift](../resources/shift.md) doesn't exist, this method returns `404 Not found`.</span></span>

## <a name="permissions"></a><span data-ttu-id="ebdb7-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ebdb7-107">Permissions</span></span>

<span data-ttu-id="ebdb7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ebdb7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebdb7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ebdb7-110">Permission type</span></span>      | <span data-ttu-id="ebdb7-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ebdb7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ebdb7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ebdb7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ebdb7-113">Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebdb7-113">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ebdb7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ebdb7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ebdb7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ebdb7-115">Not supported.</span></span>    |
|<span data-ttu-id="ebdb7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ebdb7-116">Application</span></span> | <span data-ttu-id="ebdb7-117">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebdb7-117">Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ebdb7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ebdb7-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /teams/{teamId}/schedule/shifts/{shiftId}
```

## <a name="request-headers"></a><span data-ttu-id="ebdb7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ebdb7-119">Request headers</span></span>

| <span data-ttu-id="ebdb7-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ebdb7-120">Header</span></span>       | <span data-ttu-id="ebdb7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ebdb7-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ebdb7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ebdb7-122">Authorization</span></span>  | <span data-ttu-id="ebdb7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ebdb7-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ebdb7-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ebdb7-125">Content-Type</span></span>  | <span data-ttu-id="ebdb7-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ebdb7-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ebdb7-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ebdb7-128">Request body</span></span>

<span data-ttu-id="ebdb7-129">В теле запроса поставляем представление JSON объекта [переноса.](../resources/shift.md)</span><span class="sxs-lookup"><span data-stu-id="ebdb7-129">In the request body, supply a JSON representation of a [shift](../resources/shift.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ebdb7-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="ebdb7-130">Response</span></span>

<span data-ttu-id="ebdb7-131">В случае успешной работы этот метод возвращает код отклика и объект `200 OK` [переноса](../resources/shift.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ebdb7-131">If successful, this method returns a `200 OK` response code and a [shift](../resources/shift.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ebdb7-132">Пример</span><span class="sxs-lookup"><span data-stu-id="ebdb7-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ebdb7-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="ebdb7-133">Request</span></span>

<span data-ttu-id="ebdb7-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ebdb7-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ebdb7-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="ebdb7-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-put"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/shifts/{shiftId}
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
# <a name="c"></a>[<span data-ttu-id="ebdb7-136">C#</span><span class="sxs-lookup"><span data-stu-id="ebdb7-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-put-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ebdb7-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ebdb7-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-put-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ebdb7-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ebdb7-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-put-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ebdb7-139">Java</span><span class="sxs-lookup"><span data-stu-id="ebdb7-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/shift-put-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


#### <a name="response"></a><span data-ttu-id="ebdb7-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="ebdb7-140">Response</span></span>

<span data-ttu-id="ebdb7-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ebdb7-141">The following is an example of the response.</span></span> 

><span data-ttu-id="ebdb7-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ebdb7-142">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  ]
}
-->

