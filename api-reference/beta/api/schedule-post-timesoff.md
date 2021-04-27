---
title: Создание timeOff
description: Создание нового timeOff.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b9e57f24ff16c9140e012328f7fda8917fcb4dbe
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052714"
---
# <a name="create-timeoff"></a><span data-ttu-id="11b44-103">Создание timeOff</span><span class="sxs-lookup"><span data-stu-id="11b44-103">Create timeOff</span></span>

<span data-ttu-id="11b44-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11b44-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11b44-105">Создание нового [экземпляра timeOff](../resources/timeoff.md) в расписании. [](../resources/schedule.md)</span><span class="sxs-lookup"><span data-stu-id="11b44-105">Create a new [timeOff](../resources/timeoff.md) instance in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="11b44-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="11b44-106">Permissions</span></span>

<span data-ttu-id="11b44-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11b44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11b44-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="11b44-109">Permission type</span></span>      | <span data-ttu-id="11b44-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="11b44-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="11b44-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="11b44-111">Delegated (work or school account)</span></span> | <span data-ttu-id="11b44-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11b44-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="11b44-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="11b44-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11b44-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11b44-114">Not supported.</span></span>    |
|<span data-ttu-id="11b44-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="11b44-115">Application</span></span> | <span data-ttu-id="11b44-116">Schedule.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="11b44-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="11b44-117">\***Важно:** Разрешения приложения в настоящее время доступны только в закрытом режиме и недоступны для общего пользования.</span><span class="sxs-lookup"><span data-stu-id="11b44-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="11b44-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="11b44-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="11b44-119">Глобальные администраторы могут получать доступ к группам, в которых они не являются членами.</span><span class="sxs-lookup"><span data-stu-id="11b44-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="11b44-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="11b44-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timesOff
```

## <a name="request-headers"></a><span data-ttu-id="11b44-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="11b44-121">Request headers</span></span>

| <span data-ttu-id="11b44-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="11b44-122">Header</span></span>       | <span data-ttu-id="11b44-123">Значение</span><span class="sxs-lookup"><span data-stu-id="11b44-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="11b44-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="11b44-124">Authorization</span></span>  | <span data-ttu-id="11b44-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="11b44-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="11b44-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="11b44-127">Content-Type</span></span>  | <span data-ttu-id="11b44-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="11b44-p104">application/json. Required.</span></span>  |

## <a name="response"></a><span data-ttu-id="11b44-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="11b44-130">Response</span></span>

<span data-ttu-id="11b44-131">В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект timeOff](../resources/timeoff.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="11b44-131">If successful, this method returns a `201 Created` response code and a [timeOff](../resources/timeoff.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11b44-132">Пример</span><span class="sxs-lookup"><span data-stu-id="11b44-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="11b44-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="11b44-133">Request</span></span>

<span data-ttu-id="11b44-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="11b44-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="11b44-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="11b44-135">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="11b44-136">C#</span><span class="sxs-lookup"><span data-stu-id="11b44-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoff-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="11b44-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="11b44-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoff-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="11b44-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="11b44-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoff-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="11b44-139">Java</span><span class="sxs-lookup"><span data-stu-id="11b44-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timeoff-post-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="11b44-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="11b44-140">Response</span></span>

<span data-ttu-id="11b44-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="11b44-141">The following is an example of the response.</span></span> 

><span data-ttu-id="11b44-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="11b44-142">**Note:** The response object shown here might be shortened for readability.</span></span>
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


