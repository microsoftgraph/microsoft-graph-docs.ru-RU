---
title: Получение Тимеофф
description: Получение Тимеофф по ИДЕНТИФИКАТОРу.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e6b70967be4de1d067cf09965a0a98802abb99a2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452332"
---
# <a name="get-timeoff"></a><span data-ttu-id="c9e99-103">Получение Тимеофф</span><span class="sxs-lookup"><span data-stu-id="c9e99-103">Get timeOff</span></span>

<span data-ttu-id="c9e99-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9e99-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9e99-105">Получение свойств и связей объекта [тимеофф](../resources/timeoff.md) по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="c9e99-105">Retrieve the properties and relationships of a [timeOff](../resources/timeoff.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="c9e99-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c9e99-106">Permissions</span></span>

<span data-ttu-id="c9e99-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9e99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9e99-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c9e99-109">Permission type</span></span>      | <span data-ttu-id="c9e99-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c9e99-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c9e99-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c9e99-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c9e99-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9e99-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c9e99-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c9e99-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9e99-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9e99-114">Not supported.</span></span>    |
|<span data-ttu-id="c9e99-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c9e99-115">Application</span></span> | <span data-ttu-id="c9e99-116">Schedule. Read. All *, Schedule. ReadWrite. ALL*</span><span class="sxs-lookup"><span data-stu-id="c9e99-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span> |

><span data-ttu-id="c9e99-117">\***Важно!** Разрешения на доступ к приложениям в настоящее время доступны только для частного просмотра и недоступны для использования в общедоступном режиме.</span><span class="sxs-lookup"><span data-stu-id="c9e99-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="c9e99-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="c9e99-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="c9e99-119">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="c9e99-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="c9e99-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c9e99-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timesOff/{timeOffId}
```

## <a name="request-headers"></a><span data-ttu-id="c9e99-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c9e99-121">Request headers</span></span>

| <span data-ttu-id="c9e99-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c9e99-122">Header</span></span>       | <span data-ttu-id="c9e99-123">Значение</span><span class="sxs-lookup"><span data-stu-id="c9e99-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c9e99-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c9e99-124">Authorization</span></span>  | <span data-ttu-id="c9e99-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c9e99-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c9e99-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c9e99-127">Request body</span></span>
<span data-ttu-id="c9e99-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c9e99-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9e99-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="c9e99-129">Response</span></span>

<span data-ttu-id="c9e99-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [тимеофф](../resources/timeoff.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c9e99-130">If successful, this method returns a `200 OK` response code and a [timeOff](../resources/timeoff.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9e99-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c9e99-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c9e99-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9e99-132">Request</span></span>

<span data-ttu-id="c9e99-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c9e99-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c9e99-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c9e99-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoff-get"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/timesOff/{timeOffId}
```
# <a name="c"></a>[<span data-ttu-id="c9e99-135">C#</span><span class="sxs-lookup"><span data-stu-id="c9e99-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoff-get-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c9e99-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c9e99-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoff-get-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c9e99-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c9e99-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoff-get-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c9e99-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9e99-138">Response</span></span>

<span data-ttu-id="c9e99-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c9e99-139">The following is an example of the response.</span></span> 

><span data-ttu-id="c9e99-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c9e99-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
