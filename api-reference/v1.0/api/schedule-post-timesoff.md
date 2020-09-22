---
title: Создание Тимеофф
description: Создание нового Тимеофф.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c9c4f3d95e828e1886e1cc3d474830059de1349a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48083185"
---
# <a name="create-timeoff"></a><span data-ttu-id="8501a-103">Создание Тимеофф</span><span class="sxs-lookup"><span data-stu-id="8501a-103">Create timeOff</span></span>

<span data-ttu-id="8501a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8501a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8501a-105">Создайте новый экземпляр [тимеофф](../resources/timeoff.md) в [расписании](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="8501a-105">Create a new [timeOff](../resources/timeoff.md) instance in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8501a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8501a-106">Permissions</span></span>

<span data-ttu-id="8501a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8501a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8501a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8501a-109">Permission type</span></span>      | <span data-ttu-id="8501a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8501a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8501a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8501a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8501a-112">Запланируйте. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="8501a-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8501a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8501a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8501a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8501a-114">Not supported.</span></span>    |
|<span data-ttu-id="8501a-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="8501a-115">Application</span></span> | <span data-ttu-id="8501a-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8501a-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="8501a-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="8501a-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="8501a-118">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="8501a-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="8501a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8501a-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timesOff
```

## <a name="request-headers"></a><span data-ttu-id="8501a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8501a-120">Request headers</span></span>

| <span data-ttu-id="8501a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8501a-121">Header</span></span>       | <span data-ttu-id="8501a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8501a-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8501a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8501a-123">Authorization</span></span>  | <span data-ttu-id="8501a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8501a-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8501a-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8501a-126">Content-Type</span></span>  | <span data-ttu-id="8501a-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8501a-p104">application/json. Required.</span></span>  |

## <a name="response"></a><span data-ttu-id="8501a-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="8501a-129">Response</span></span>

<span data-ttu-id="8501a-130">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [тимеофф](../resources/timeoff.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8501a-130">If successful, this method returns a `201 Created` response code and a [timeOff](../resources/timeoff.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8501a-131">Пример</span><span class="sxs-lookup"><span data-stu-id="8501a-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="8501a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8501a-132">Request</span></span>

<span data-ttu-id="8501a-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8501a-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8501a-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="8501a-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoff-post"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/timesOff
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
# <a name="c"></a>[<span data-ttu-id="8501a-135">C#</span><span class="sxs-lookup"><span data-stu-id="8501a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoff-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8501a-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8501a-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoff-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8501a-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8501a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoff-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8501a-138">Java</span><span class="sxs-lookup"><span data-stu-id="8501a-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timeoff-post-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="8501a-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="8501a-139">Response</span></span>

<span data-ttu-id="8501a-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8501a-140">The following is an example of the response.</span></span> 

><span data-ttu-id="8501a-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8501a-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

