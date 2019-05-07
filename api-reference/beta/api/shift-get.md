---
title: Получение Shift
description: Получение сдвига по ИДЕНТИФИКАТОРу.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 207c9b40557d2f75ba73ecb76983dc9b9c8129f2
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638657"
---
# <a name="get-shift"></a><span data-ttu-id="82b08-103">Получение Shift</span><span class="sxs-lookup"><span data-stu-id="82b08-103">Get shift</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82b08-104">Получение свойств и связей объекта [SHIFT](../resources/shift.md) по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="82b08-104">Retrieve the properties and relationships of a [shift](../resources/shift.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="82b08-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="82b08-105">Permissions</span></span>

<span data-ttu-id="82b08-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82b08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82b08-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="82b08-108">Permission type</span></span>      | <span data-ttu-id="82b08-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="82b08-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="82b08-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="82b08-110">Delegated (work or school account)</span></span> | <span data-ttu-id="82b08-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82b08-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="82b08-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="82b08-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82b08-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82b08-113">Not supported.</span></span>    |
|<span data-ttu-id="82b08-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="82b08-114">Application</span></span> | <span data-ttu-id="82b08-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82b08-115">Not supported.</span></span> |

> <span data-ttu-id="82b08-116">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="82b08-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="82b08-117">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="82b08-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="82b08-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="82b08-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/shifts/{shiftId}
```

## <a name="request-headers"></a><span data-ttu-id="82b08-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="82b08-119">Request headers</span></span>

| <span data-ttu-id="82b08-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="82b08-120">Header</span></span>       | <span data-ttu-id="82b08-121">Значение</span><span class="sxs-lookup"><span data-stu-id="82b08-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="82b08-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="82b08-122">Authorization</span></span>  | <span data-ttu-id="82b08-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="82b08-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="82b08-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="82b08-125">Content-Type</span></span>  | <span data-ttu-id="82b08-126">application/json</span><span class="sxs-lookup"><span data-stu-id="82b08-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="82b08-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="82b08-127">Request body</span></span>
<span data-ttu-id="82b08-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="82b08-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="82b08-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="82b08-129">Response</span></span>

<span data-ttu-id="82b08-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [сдвига](../resources/shift.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="82b08-130">If successful, this method returns a `200 OK` response code and a [shift](../resources/shift.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82b08-131">Пример</span><span class="sxs-lookup"><span data-stu-id="82b08-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="82b08-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="82b08-132">Request</span></span>

<span data-ttu-id="82b08-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="82b08-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "shift-get"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/shifts/{shiftId}
```

#### <a name="response"></a><span data-ttu-id="82b08-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="82b08-134">Response</span></span>

<span data-ttu-id="82b08-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="82b08-135">The following is an example of the response.</span></span> 

><span data-ttu-id="82b08-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="82b08-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="82b08-138">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="82b08-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="82b08-139">Языках</span><span class="sxs-lookup"><span data-stu-id="82b08-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/shift-get-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="82b08-140">Язык</span><span class="sxs-lookup"><span data-stu-id="82b08-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/shift-get-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/shift-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/shift-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
