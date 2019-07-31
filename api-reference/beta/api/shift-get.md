---
title: Получение Shift
description: Получение сдвига по ИДЕНТИФИКАТОРу.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a3df7bf69b31582a197bed55b7b4906a4aef610f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35982835"
---
# <a name="get-shift"></a><span data-ttu-id="7bfc5-103">Получение Shift</span><span class="sxs-lookup"><span data-stu-id="7bfc5-103">Get shift</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7bfc5-104">Получение свойств и связей объекта [SHIFT](../resources/shift.md) по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="7bfc5-104">Retrieve the properties and relationships of a [shift](../resources/shift.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="7bfc5-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7bfc5-105">Permissions</span></span>

<span data-ttu-id="7bfc5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7bfc5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7bfc5-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7bfc5-108">Permission type</span></span>      | <span data-ttu-id="7bfc5-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7bfc5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7bfc5-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7bfc5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7bfc5-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bfc5-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7bfc5-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7bfc5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7bfc5-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7bfc5-113">Not supported.</span></span>    |
|<span data-ttu-id="7bfc5-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7bfc5-114">Application</span></span> | <span data-ttu-id="7bfc5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7bfc5-115">Not supported.</span></span> |

> <span data-ttu-id="7bfc5-116">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="7bfc5-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="7bfc5-117">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="7bfc5-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="7bfc5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7bfc5-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/shifts/{shiftId}
```

## <a name="request-headers"></a><span data-ttu-id="7bfc5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7bfc5-119">Request headers</span></span>

| <span data-ttu-id="7bfc5-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7bfc5-120">Header</span></span>       | <span data-ttu-id="7bfc5-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7bfc5-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7bfc5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7bfc5-122">Authorization</span></span>  | <span data-ttu-id="7bfc5-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7bfc5-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7bfc5-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7bfc5-125">Content-Type</span></span>  | <span data-ttu-id="7bfc5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7bfc5-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7bfc5-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7bfc5-127">Request body</span></span>
<span data-ttu-id="7bfc5-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7bfc5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7bfc5-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="7bfc5-129">Response</span></span>

<span data-ttu-id="7bfc5-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [сдвига](../resources/shift.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7bfc5-130">If successful, this method returns a `200 OK` response code and a [shift](../resources/shift.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7bfc5-131">Пример</span><span class="sxs-lookup"><span data-stu-id="7bfc5-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="7bfc5-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="7bfc5-132">Request</span></span>

<span data-ttu-id="7bfc5-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7bfc5-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7bfc5-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="7bfc5-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-get"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/shifts/{shiftId}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7bfc5-135">C#</span><span class="sxs-lookup"><span data-stu-id="7bfc5-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-get-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7bfc5-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="7bfc5-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-get-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7bfc5-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="7bfc5-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-get-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7bfc5-138">Java</span><span class="sxs-lookup"><span data-stu-id="7bfc5-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/shift-get-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7bfc5-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="7bfc5-139">Response</span></span>

<span data-ttu-id="7bfc5-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7bfc5-140">The following is an example of the response.</span></span> 

><span data-ttu-id="7bfc5-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7bfc5-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Get a shift by id",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
