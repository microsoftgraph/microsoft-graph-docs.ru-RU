---
title: Замена Тимеофф
description: Замена существующего Тимеофф.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 69730353bfea2ec150aba7b861241eb359e35033
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637516"
---
# <a name="replace-timeoff"></a><span data-ttu-id="bf9d5-103">Замена Тимеофф</span><span class="sxs-lookup"><span data-stu-id="bf9d5-103">Replace timeOff</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf9d5-104">Замена существующего [тимеофф](../resources/timeoff.md).</span><span class="sxs-lookup"><span data-stu-id="bf9d5-104">Replace an existing [timeOff](../resources/timeoff.md).</span></span>

<span data-ttu-id="bf9d5-105">Если указанный [тимеофф](../resources/timeoff.md) не существует, этот метод возвращает значение `404 Not found`.</span><span class="sxs-lookup"><span data-stu-id="bf9d5-105">If the specified [timeOff](../resources/timeoff.md) doesn't exist, this method returns `404 Not found`.</span></span>

## <a name="permissions"></a><span data-ttu-id="bf9d5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bf9d5-106">Permissions</span></span>

<span data-ttu-id="bf9d5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf9d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf9d5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bf9d5-109">Permission type</span></span>      | <span data-ttu-id="bf9d5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bf9d5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bf9d5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bf9d5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bf9d5-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf9d5-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="bf9d5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bf9d5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf9d5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf9d5-114">Not supported.</span></span>    |
|<span data-ttu-id="bf9d5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bf9d5-115">Application</span></span> | <span data-ttu-id="bf9d5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf9d5-116">Not supported.</span></span> |

> <span data-ttu-id="bf9d5-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="bf9d5-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="bf9d5-118">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="bf9d5-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="bf9d5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bf9d5-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/timesOff/{timeOffId}
```

## <a name="request-headers"></a><span data-ttu-id="bf9d5-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bf9d5-120">Request headers</span></span>

| <span data-ttu-id="bf9d5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bf9d5-121">Header</span></span>       | <span data-ttu-id="bf9d5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bf9d5-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bf9d5-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bf9d5-123">Authorization</span></span>  | <span data-ttu-id="bf9d5-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bf9d5-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bf9d5-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bf9d5-126">Content-Type</span></span>  | <span data-ttu-id="bf9d5-127">application/json</span><span class="sxs-lookup"><span data-stu-id="bf9d5-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bf9d5-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bf9d5-128">Request body</span></span>

<span data-ttu-id="bf9d5-129">В тексте запроса добавьте представление объекта [Тимеофф](../resources/timeoff.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bf9d5-129">In the request body, supply a JSON representation of a [timeOff](../resources/timeoff.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="bf9d5-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf9d5-130">Response</span></span>

<span data-ttu-id="bf9d5-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [тимеофф](../resources/timeoff.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bf9d5-131">If successful, this method returns a `200 OK` response code and a [timeOff](../resources/timeoff.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf9d5-132">Пример</span><span class="sxs-lookup"><span data-stu-id="bf9d5-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="bf9d5-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="bf9d5-133">Request</span></span>

<span data-ttu-id="bf9d5-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bf9d5-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "timeoff-put"
}-->
```http
PUT https://graph.microsoft.com/beta/teams/{teamId}/schedule/timesOff/{timeOffId}
Content-type: application/json
Prefer: return=representation

{
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "sharedTimeOff": {
    "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    "startDateTime": "2019-03-11T07:00:00Z",
    "endDateTime": "2019-03-12T07:00:00Z",
    "theme": "white"
  },
  "draftTimeOff": {
    "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    "startDateTime": "2019-03-11T07:00:00Z",
    "endDateTime": "2019-03-12T07:00:00Z",
    "theme": "pink"
  }
}
```

#### <a name="response"></a><span data-ttu-id="bf9d5-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf9d5-135">Response</span></span>

<span data-ttu-id="bf9d5-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bf9d5-136">The following is an example of the response.</span></span> 

><span data-ttu-id="bf9d5-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bf9d5-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeOff"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "createdDateTime": "2019-03-14T05:35:57.755Z",
  "lastModifiedDateTime": "2019-03-14T05:36:08.381Z",
  "lastModifiedBy": {
    "@odata.type":"microsoft.graph.identitySet",
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  },
  "sharedTimeOff": {
    "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    "startDateTime": "2019-03-11T07:00:00Z",
    "endDateTime": "2019-03-12T07:00:00Z",
    "theme": "white"
  },
  "draftTimeOff": {
    "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    "startDateTime": "2019-03-11T07:00:00Z",
    "endDateTime": "2019-03-12T07:00:00Z",
    "theme": "pink"
  }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="bf9d5-139">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="bf9d5-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="bf9d5-140">Языках</span><span class="sxs-lookup"><span data-stu-id="bf9d5-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/timeoff-put-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bf9d5-141">Язык</span><span class="sxs-lookup"><span data-stu-id="bf9d5-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/timeoff-put-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Replace an existing timeOff",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/timeoff-put.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/timeoff-put.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
