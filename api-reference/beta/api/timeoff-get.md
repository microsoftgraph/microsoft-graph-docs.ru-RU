---
title: Получение Тимеофф
description: Получение Тимеофф по ИДЕНТИФИКАТОРу.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4a26b0e1048a4a43a0dad833c07d901367cf40f9
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981452"
---
# <a name="get-timeoff"></a><span data-ttu-id="3e1ba-103">Получение Тимеофф</span><span class="sxs-lookup"><span data-stu-id="3e1ba-103">Get timeOff</span></span>

<span data-ttu-id="3e1ba-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e1ba-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e1ba-105">Получение свойств и связей объекта [тимеофф](../resources/timeoff.md) по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="3e1ba-105">Retrieve the properties and relationships of a [timeOff](../resources/timeoff.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="3e1ba-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3e1ba-106">Permissions</span></span>

<span data-ttu-id="3e1ba-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e1ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e1ba-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3e1ba-109">Permission type</span></span>      | <span data-ttu-id="3e1ba-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3e1ba-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e1ba-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3e1ba-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3e1ba-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e1ba-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3e1ba-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3e1ba-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e1ba-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e1ba-114">Not supported.</span></span>    |
|<span data-ttu-id="3e1ba-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="3e1ba-115">Application</span></span> | <span data-ttu-id="3e1ba-116">Schedule. Read. All *, Schedule. ReadWrite. ALL*</span><span class="sxs-lookup"><span data-stu-id="3e1ba-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span> |

><span data-ttu-id="3e1ba-117">\***Важно!** Разрешения на доступ к приложениям в настоящее время доступны только для частного просмотра и недоступны для использования в общедоступном режиме.</span><span class="sxs-lookup"><span data-stu-id="3e1ba-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="3e1ba-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="3e1ba-118">**Note** : This API supports admin permissions.</span></span> <span data-ttu-id="3e1ba-119">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="3e1ba-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="3e1ba-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3e1ba-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timesOff/{timeOffId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3e1ba-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3e1ba-121">Optional query parameters</span></span>

<span data-ttu-id="3e1ba-122">Этот метод не поддерживает параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="3e1ba-122">This method does not support OData query parameters to customize the response.</span></span>


## <a name="request-headers"></a><span data-ttu-id="3e1ba-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3e1ba-123">Request headers</span></span>

| <span data-ttu-id="3e1ba-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3e1ba-124">Header</span></span>       | <span data-ttu-id="3e1ba-125">Значение</span><span class="sxs-lookup"><span data-stu-id="3e1ba-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3e1ba-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3e1ba-126">Authorization</span></span>  | <span data-ttu-id="3e1ba-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3e1ba-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3e1ba-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3e1ba-129">Request body</span></span>
<span data-ttu-id="3e1ba-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3e1ba-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3e1ba-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e1ba-131">Response</span></span>

<span data-ttu-id="3e1ba-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [тимеофф](../resources/timeoff.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3e1ba-132">If successful, this method returns a `200 OK` response code and a [timeOff](../resources/timeoff.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e1ba-133">Пример</span><span class="sxs-lookup"><span data-stu-id="3e1ba-133">Example</span></span>

#### <a name="request"></a><span data-ttu-id="3e1ba-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="3e1ba-134">Request</span></span>

<span data-ttu-id="3e1ba-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3e1ba-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3e1ba-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="3e1ba-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoff-get"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/timesOff/{timeOffId}
```
# <a name="c"></a>[<span data-ttu-id="3e1ba-137">C#</span><span class="sxs-lookup"><span data-stu-id="3e1ba-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoff-get-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3e1ba-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3e1ba-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoff-get-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3e1ba-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3e1ba-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoff-get-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3e1ba-140">Java</span><span class="sxs-lookup"><span data-stu-id="3e1ba-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timeoff-get-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3e1ba-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e1ba-141">Response</span></span>

<span data-ttu-id="3e1ba-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3e1ba-142">The following is an example of the response.</span></span> 

><span data-ttu-id="3e1ba-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3e1ba-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


