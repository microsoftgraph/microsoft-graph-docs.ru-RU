---
title: Замена Тимеофф
description: Замена существующего Тимеофф.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7234fc4f630064acf1934079a4ed485a2c3b1524
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2020
ms.locfileid: "42452311"
---
# <a name="replace-timeoff"></a><span data-ttu-id="b1736-103">Замена Тимеофф</span><span class="sxs-lookup"><span data-stu-id="b1736-103">Replace timeOff</span></span>

<span data-ttu-id="b1736-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1736-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1736-105">Замена существующего [тимеофф](../resources/timeoff.md).</span><span class="sxs-lookup"><span data-stu-id="b1736-105">Replace an existing [timeOff](../resources/timeoff.md).</span></span>

<span data-ttu-id="b1736-106">Если указанный [тимеофф](../resources/timeoff.md) не существует, этот метод возвращает значение `404 Not found` .</span><span class="sxs-lookup"><span data-stu-id="b1736-106">If the specified [timeOff](../resources/timeoff.md) doesn't exist, this method returns `404 Not found`.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1736-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b1736-107">Permissions</span></span>

<span data-ttu-id="b1736-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1736-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1736-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b1736-110">Permission type</span></span>      | <span data-ttu-id="b1736-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b1736-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b1736-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b1736-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b1736-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1736-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b1736-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b1736-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1736-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1736-115">Not supported.</span></span>    |
|<span data-ttu-id="b1736-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b1736-116">Application</span></span> | <span data-ttu-id="b1736-117">Schedule. ReadWrite. ALL \*</span><span class="sxs-lookup"><span data-stu-id="b1736-117">Schedule.ReadWrite.All\*</span></span>  |

><span data-ttu-id="b1736-118">\***Важно!** Разрешения на доступ к приложениям в настоящее время доступны только для частного просмотра и недоступны для использования в общедоступном режиме.</span><span class="sxs-lookup"><span data-stu-id="b1736-118">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="b1736-119">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="b1736-119">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="b1736-120">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="b1736-120">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="b1736-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b1736-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/timesOff/{timeOffId}
```

## <a name="request-headers"></a><span data-ttu-id="b1736-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b1736-122">Request headers</span></span>

| <span data-ttu-id="b1736-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b1736-123">Header</span></span>       | <span data-ttu-id="b1736-124">Значение</span><span class="sxs-lookup"><span data-stu-id="b1736-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b1736-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b1736-125">Authorization</span></span>  | <span data-ttu-id="b1736-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1736-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b1736-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b1736-128">Content-Type</span></span>  | <span data-ttu-id="b1736-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1736-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b1736-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b1736-131">Request body</span></span>

<span data-ttu-id="b1736-132">В тексте запроса добавьте представление объекта [тимеофф](../resources/timeoff.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b1736-132">In the request body, supply a JSON representation of a [timeOff](../resources/timeoff.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b1736-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="b1736-133">Response</span></span>

<span data-ttu-id="b1736-134">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [тимеофф](../resources/timeoff.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b1736-134">If successful, this method returns a `200 OK` response code and a [timeOff](../resources/timeoff.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1736-135">Пример</span><span class="sxs-lookup"><span data-stu-id="b1736-135">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b1736-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1736-136">Request</span></span>

<span data-ttu-id="b1736-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b1736-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b1736-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="b1736-138">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b1736-139">C#</span><span class="sxs-lookup"><span data-stu-id="b1736-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoff-put-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b1736-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b1736-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoff-put-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b1736-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b1736-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoff-put-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b1736-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1736-142">Response</span></span>

<span data-ttu-id="b1736-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b1736-143">The following is an example of the response.</span></span> 

><span data-ttu-id="b1736-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b1736-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
