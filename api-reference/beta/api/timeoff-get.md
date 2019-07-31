---
title: Получение Тимеофф
description: Получение Тимеофф по ИДЕНТИФИКАТОРу.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b186a963652748faaab37c18e23ed43d672f2c70
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35982405"
---
# <a name="get-timeoff"></a><span data-ttu-id="d2549-103">Получение Тимеофф</span><span class="sxs-lookup"><span data-stu-id="d2549-103">Get timeOff</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2549-104">Получение свойств и связей объекта [тимеофф](../resources/timeoff.md) по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="d2549-104">Retrieve the properties and relationships of a [timeOff](../resources/timeoff.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2549-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d2549-105">Permissions</span></span>

<span data-ttu-id="d2549-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2549-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2549-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2549-108">Permission type</span></span>      | <span data-ttu-id="d2549-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2549-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2549-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2549-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d2549-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2549-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d2549-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2549-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2549-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2549-113">Not supported.</span></span>    |
|<span data-ttu-id="d2549-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d2549-114">Application</span></span> | <span data-ttu-id="d2549-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2549-115">Not supported.</span></span> |

> <span data-ttu-id="d2549-116">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="d2549-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="d2549-117">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="d2549-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="d2549-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2549-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timesOff/{timeOffId}
```

## <a name="request-headers"></a><span data-ttu-id="d2549-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d2549-119">Request headers</span></span>

| <span data-ttu-id="d2549-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d2549-120">Header</span></span>       | <span data-ttu-id="d2549-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d2549-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d2549-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d2549-122">Authorization</span></span>  | <span data-ttu-id="d2549-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2549-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d2549-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d2549-125">Content-Type</span></span>  | <span data-ttu-id="d2549-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d2549-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d2549-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d2549-127">Request body</span></span>
<span data-ttu-id="d2549-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d2549-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2549-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2549-129">Response</span></span>

<span data-ttu-id="d2549-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [тимеофф](../resources/timeoff.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d2549-130">If successful, this method returns a `200 OK` response code and a [timeOff](../resources/timeoff.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2549-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d2549-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d2549-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2549-132">Request</span></span>

<span data-ttu-id="d2549-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d2549-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d2549-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="d2549-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoff-get"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/timesOff/{timeOffId}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d2549-135">C#</span><span class="sxs-lookup"><span data-stu-id="d2549-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoff-get-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d2549-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="d2549-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoff-get-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d2549-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d2549-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoff-get-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d2549-138">Java</span><span class="sxs-lookup"><span data-stu-id="d2549-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timeoff-get-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d2549-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2549-139">Response</span></span>

<span data-ttu-id="d2549-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d2549-140">The following is an example of the response.</span></span> 

><span data-ttu-id="d2549-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d2549-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get a timeOff by id",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
