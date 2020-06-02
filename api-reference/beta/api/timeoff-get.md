---
title: Получение Тимеофф
description: Получение Тимеофф по ИДЕНТИФИКАТОРу.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f4fc2fd04d6c9fef78294b0a99d586c32a17cc8e
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44154432"
---
# <a name="get-timeoff"></a><span data-ttu-id="fd9d8-103">Получение Тимеофф</span><span class="sxs-lookup"><span data-stu-id="fd9d8-103">Get timeOff</span></span>

<span data-ttu-id="fd9d8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd9d8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd9d8-105">Получение свойств и связей объекта [тимеофф](../resources/timeoff.md) по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="fd9d8-105">Retrieve the properties and relationships of a [timeOff](../resources/timeoff.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="fd9d8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fd9d8-106">Permissions</span></span>

<span data-ttu-id="fd9d8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd9d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd9d8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fd9d8-109">Permission type</span></span>      | <span data-ttu-id="fd9d8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fd9d8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd9d8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fd9d8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fd9d8-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd9d8-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="fd9d8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fd9d8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd9d8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd9d8-114">Not supported.</span></span>    |
|<span data-ttu-id="fd9d8-115">Сервер приложений</span><span class="sxs-lookup"><span data-stu-id="fd9d8-115">Application</span></span> | <span data-ttu-id="fd9d8-116">Schedule. Read. All *, Schedule. ReadWrite. ALL*</span><span class="sxs-lookup"><span data-stu-id="fd9d8-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span> |

><span data-ttu-id="fd9d8-117">\***Важно!** Разрешения на доступ к приложениям в настоящее время доступны только для частного просмотра и недоступны для использования в общедоступном режиме.</span><span class="sxs-lookup"><span data-stu-id="fd9d8-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="fd9d8-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="fd9d8-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="fd9d8-119">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="fd9d8-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="fd9d8-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fd9d8-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timesOff/{timeOffId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fd9d8-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fd9d8-121">Optional query parameters</span></span>

<span data-ttu-id="fd9d8-122">Этот метод не поддерживает параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="fd9d8-122">This method does not support OData query parameters to customize the response.</span></span>


## <a name="request-headers"></a><span data-ttu-id="fd9d8-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fd9d8-123">Request headers</span></span>

| <span data-ttu-id="fd9d8-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fd9d8-124">Header</span></span>       | <span data-ttu-id="fd9d8-125">Значение</span><span class="sxs-lookup"><span data-stu-id="fd9d8-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fd9d8-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fd9d8-126">Authorization</span></span>  | <span data-ttu-id="fd9d8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fd9d8-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fd9d8-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fd9d8-129">Request body</span></span>
<span data-ttu-id="fd9d8-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fd9d8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fd9d8-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd9d8-131">Response</span></span>

<span data-ttu-id="fd9d8-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [тимеофф](../resources/timeoff.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fd9d8-132">If successful, this method returns a `200 OK` response code and a [timeOff](../resources/timeoff.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd9d8-133">Пример</span><span class="sxs-lookup"><span data-stu-id="fd9d8-133">Example</span></span>

#### <a name="request"></a><span data-ttu-id="fd9d8-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="fd9d8-134">Request</span></span>

<span data-ttu-id="fd9d8-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fd9d8-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fd9d8-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="fd9d8-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoff-get"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/timesOff/{timeOffId}
```
# <a name="c"></a>[<span data-ttu-id="fd9d8-137">C#</span><span class="sxs-lookup"><span data-stu-id="fd9d8-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoff-get-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fd9d8-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fd9d8-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoff-get-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fd9d8-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fd9d8-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoff-get-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fd9d8-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd9d8-140">Response</span></span>

<span data-ttu-id="fd9d8-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fd9d8-141">The following is an example of the response.</span></span> 

><span data-ttu-id="fd9d8-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fd9d8-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
