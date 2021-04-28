---
title: Создание timeOff
description: Создание нового timeOff.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 14cda6031e07ecf694ce771ad3a08a014057c25e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52039050"
---
# <a name="create-timeoff"></a><span data-ttu-id="e07f7-103">Создание timeOff</span><span class="sxs-lookup"><span data-stu-id="e07f7-103">Create timeOff</span></span>

<span data-ttu-id="e07f7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e07f7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e07f7-105">Создание нового [экземпляра timeOff](../resources/timeoff.md) в расписании. [](../resources/schedule.md)</span><span class="sxs-lookup"><span data-stu-id="e07f7-105">Create a new [timeOff](../resources/timeoff.md) instance in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e07f7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e07f7-106">Permissions</span></span>

<span data-ttu-id="e07f7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e07f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e07f7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e07f7-109">Permission type</span></span>      | <span data-ttu-id="e07f7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e07f7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e07f7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e07f7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e07f7-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e07f7-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e07f7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e07f7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e07f7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e07f7-114">Not supported.</span></span>    |
|<span data-ttu-id="e07f7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e07f7-115">Application</span></span> | <span data-ttu-id="e07f7-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e07f7-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="e07f7-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="e07f7-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="e07f7-118">Глобальные администраторы могут получать доступ к группам, в которых они не являются членами.</span><span class="sxs-lookup"><span data-stu-id="e07f7-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="e07f7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e07f7-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timesOff
```

## <a name="request-headers"></a><span data-ttu-id="e07f7-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e07f7-120">Request headers</span></span>

| <span data-ttu-id="e07f7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e07f7-121">Header</span></span>       | <span data-ttu-id="e07f7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e07f7-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e07f7-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e07f7-123">Authorization</span></span>  | <span data-ttu-id="e07f7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e07f7-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e07f7-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e07f7-126">Content-Type</span></span>  | <span data-ttu-id="e07f7-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e07f7-p104">application/json. Required.</span></span>  |

## <a name="response"></a><span data-ttu-id="e07f7-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e07f7-129">Response</span></span>

<span data-ttu-id="e07f7-130">В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект timeOff](../resources/timeoff.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e07f7-130">If successful, this method returns a `201 Created` response code and a [timeOff](../resources/timeoff.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e07f7-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e07f7-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e07f7-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e07f7-132">Request</span></span>

<span data-ttu-id="e07f7-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e07f7-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e07f7-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="e07f7-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e07f7-135">C#</span><span class="sxs-lookup"><span data-stu-id="e07f7-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoff-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e07f7-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e07f7-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoff-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e07f7-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e07f7-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoff-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e07f7-138">Java</span><span class="sxs-lookup"><span data-stu-id="e07f7-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timeoff-post-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="e07f7-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="e07f7-139">Response</span></span>

<span data-ttu-id="e07f7-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e07f7-140">The following is an example of the response.</span></span> 

><span data-ttu-id="e07f7-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e07f7-141">**Note:** The response object shown here might be shortened for readability.</span></span>
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

