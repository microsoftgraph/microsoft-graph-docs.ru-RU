---
title: Получение Shift
description: Получение сдвига по ИДЕНТИФИКАТОРу.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 259ea0afdc1d2d5740a4bafd16925bafaedaaeee
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36410159"
---
# <a name="get-shift"></a><span data-ttu-id="ab4a0-103">Получение Shift</span><span class="sxs-lookup"><span data-stu-id="ab4a0-103">Get shift</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab4a0-104">Получение свойств и связей объекта [SHIFT](../resources/shift.md) по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="ab4a0-104">Retrieve the properties and relationships of a [shift](../resources/shift.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="ab4a0-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ab4a0-105">Permissions</span></span>

<span data-ttu-id="ab4a0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab4a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab4a0-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ab4a0-108">Permission type</span></span>      | <span data-ttu-id="ab4a0-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ab4a0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab4a0-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ab4a0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ab4a0-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab4a0-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ab4a0-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ab4a0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab4a0-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab4a0-113">Not supported.</span></span>    |
|<span data-ttu-id="ab4a0-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ab4a0-114">Application</span></span> | <span data-ttu-id="ab4a0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab4a0-115">Not supported.</span></span> |

> <span data-ttu-id="ab4a0-116">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="ab4a0-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="ab4a0-117">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="ab4a0-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="ab4a0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ab4a0-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/shifts/{shiftId}
```

## <a name="request-headers"></a><span data-ttu-id="ab4a0-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ab4a0-119">Request headers</span></span>

| <span data-ttu-id="ab4a0-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ab4a0-120">Header</span></span>       | <span data-ttu-id="ab4a0-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ab4a0-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ab4a0-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ab4a0-122">Authorization</span></span>  | <span data-ttu-id="ab4a0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ab4a0-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ab4a0-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ab4a0-125">Content-Type</span></span>  | <span data-ttu-id="ab4a0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ab4a0-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ab4a0-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ab4a0-127">Request body</span></span>
<span data-ttu-id="ab4a0-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ab4a0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab4a0-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab4a0-129">Response</span></span>

<span data-ttu-id="ab4a0-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [сдвига](../resources/shift.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ab4a0-130">If successful, this method returns a `200 OK` response code and a [shift](../resources/shift.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab4a0-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ab4a0-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ab4a0-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ab4a0-132">Request</span></span>

<span data-ttu-id="ab4a0-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ab4a0-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ab4a0-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="ab4a0-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-get"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/shifts/{shiftId}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ab4a0-135">C#</span><span class="sxs-lookup"><span data-stu-id="ab4a0-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-get-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ab4a0-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ab4a0-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-get-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ab4a0-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="ab4a0-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-get-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ab4a0-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab4a0-138">Response</span></span>

<span data-ttu-id="ab4a0-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ab4a0-139">The following is an example of the response.</span></span> 

><span data-ttu-id="ab4a0-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ab4a0-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
