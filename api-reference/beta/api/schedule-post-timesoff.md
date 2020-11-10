---
title: Создание Тимеофф
description: Создание нового Тимеофф.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 34e64c600b8e25c15784ce0d5ecbf636f8b59755
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48972089"
---
# <a name="create-timeoff"></a><span data-ttu-id="b3807-103">Создание Тимеофф</span><span class="sxs-lookup"><span data-stu-id="b3807-103">Create timeOff</span></span>

<span data-ttu-id="b3807-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3807-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3807-105">Создайте новый экземпляр [тимеофф](../resources/timeoff.md) в [расписании](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="b3807-105">Create a new [timeOff](../resources/timeoff.md) instance in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b3807-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b3807-106">Permissions</span></span>

<span data-ttu-id="b3807-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3807-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3807-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b3807-109">Permission type</span></span>      | <span data-ttu-id="b3807-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b3807-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b3807-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b3807-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b3807-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3807-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b3807-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b3807-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3807-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3807-114">Not supported.</span></span>    |
|<span data-ttu-id="b3807-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="b3807-115">Application</span></span> | <span data-ttu-id="b3807-116">Schedule. ReadWrite. ALL \*</span><span class="sxs-lookup"><span data-stu-id="b3807-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="b3807-117">\***Важно!** Разрешения на доступ к приложениям в настоящее время доступны только для частного просмотра и недоступны для использования в общедоступном режиме.</span><span class="sxs-lookup"><span data-stu-id="b3807-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="b3807-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="b3807-118">**Note** : This API supports admin permissions.</span></span> <span data-ttu-id="b3807-119">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="b3807-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="b3807-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b3807-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timesOff
```

## <a name="request-headers"></a><span data-ttu-id="b3807-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b3807-121">Request headers</span></span>

| <span data-ttu-id="b3807-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b3807-122">Header</span></span>       | <span data-ttu-id="b3807-123">Значение</span><span class="sxs-lookup"><span data-stu-id="b3807-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b3807-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b3807-124">Authorization</span></span>  | <span data-ttu-id="b3807-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b3807-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b3807-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b3807-127">Content-Type</span></span>  | <span data-ttu-id="b3807-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b3807-p104">application/json. Required.</span></span>  |

## <a name="response"></a><span data-ttu-id="b3807-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3807-130">Response</span></span>

<span data-ttu-id="b3807-131">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [тимеофф](../resources/timeoff.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b3807-131">If successful, this method returns a `201 Created` response code and a [timeOff](../resources/timeoff.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3807-132">Пример</span><span class="sxs-lookup"><span data-stu-id="b3807-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b3807-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3807-133">Request</span></span>

<span data-ttu-id="b3807-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b3807-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b3807-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="b3807-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoff-post"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{teamId}/schedule/timesOff
Content-type: application/json

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
# <a name="c"></a>[<span data-ttu-id="b3807-136">C#</span><span class="sxs-lookup"><span data-stu-id="b3807-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoff-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b3807-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b3807-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoff-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b3807-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b3807-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoff-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b3807-139">Java</span><span class="sxs-lookup"><span data-stu-id="b3807-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timeoff-post-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="b3807-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3807-140">Response</span></span>

<span data-ttu-id="b3807-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b3807-141">The following is an example of the response.</span></span> 

><span data-ttu-id="b3807-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b3807-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type":"microsoft.graph.timeOff"
} -->

```http
HTTP/1.1 201 Created
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
  "description": "Creates a new timeOff",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


