---
title: Замена timeOff
description: Замените существующее время.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 535feee59c1f3992d9d78eea1380b50bd841987c
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787354"
---
# <a name="replace-timeoff"></a><span data-ttu-id="92ab1-103">Замена timeOff</span><span class="sxs-lookup"><span data-stu-id="92ab1-103">Replace timeOff</span></span>

<span data-ttu-id="92ab1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92ab1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92ab1-105">Замените [существующий timeOff](../resources/timeoff.md).</span><span class="sxs-lookup"><span data-stu-id="92ab1-105">Replace an existing [timeOff](../resources/timeoff.md).</span></span>

<span data-ttu-id="92ab1-106">Если указанного [timeOff](../resources/timeoff.md) не существует, этот метод `404 Not found` возвращается.</span><span class="sxs-lookup"><span data-stu-id="92ab1-106">If the specified [timeOff](../resources/timeoff.md) doesn't exist, this method returns `404 Not found`.</span></span>

## <a name="permissions"></a><span data-ttu-id="92ab1-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="92ab1-107">Permissions</span></span>

<span data-ttu-id="92ab1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92ab1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92ab1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="92ab1-110">Permission type</span></span>      | <span data-ttu-id="92ab1-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="92ab1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="92ab1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="92ab1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="92ab1-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92ab1-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="92ab1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="92ab1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92ab1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92ab1-115">Not supported.</span></span>    |
|<span data-ttu-id="92ab1-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="92ab1-116">Application</span></span> | <span data-ttu-id="92ab1-117">Schedule.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="92ab1-117">Schedule.ReadWrite.All\*</span></span>  |

><span data-ttu-id="92ab1-118">\***Важно:** Разрешения приложения в настоящее время доступны только в закрытом режиме и недоступны для общего пользования.</span><span class="sxs-lookup"><span data-stu-id="92ab1-118">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="92ab1-119">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="92ab1-119">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="92ab1-120">Глобальные администраторы могут получать доступ к группам, в которых они не являются членами.</span><span class="sxs-lookup"><span data-stu-id="92ab1-120">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="92ab1-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="92ab1-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/timesOff/{timeOffId}
```

## <a name="request-headers"></a><span data-ttu-id="92ab1-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="92ab1-122">Request headers</span></span>

| <span data-ttu-id="92ab1-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="92ab1-123">Header</span></span>       | <span data-ttu-id="92ab1-124">Значение</span><span class="sxs-lookup"><span data-stu-id="92ab1-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="92ab1-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="92ab1-125">Authorization</span></span>  | <span data-ttu-id="92ab1-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="92ab1-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="92ab1-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="92ab1-128">Content-Type</span></span>  | <span data-ttu-id="92ab1-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="92ab1-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="92ab1-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="92ab1-131">Request body</span></span>

<span data-ttu-id="92ab1-132">В теле запроса поставляем представление JSON объекта [timeOff.](../resources/timeoff.md)</span><span class="sxs-lookup"><span data-stu-id="92ab1-132">In the request body, supply a JSON representation of a [timeOff](../resources/timeoff.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="92ab1-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="92ab1-133">Response</span></span>

<span data-ttu-id="92ab1-134">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект timeOff](../resources/timeoff.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="92ab1-134">If successful, this method returns a `200 OK` response code and a [timeOff](../resources/timeoff.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92ab1-135">Пример</span><span class="sxs-lookup"><span data-stu-id="92ab1-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="92ab1-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="92ab1-136">Request</span></span>

<span data-ttu-id="92ab1-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="92ab1-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="92ab1-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="92ab1-138">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="92ab1-139">C#</span><span class="sxs-lookup"><span data-stu-id="92ab1-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoff-put-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="92ab1-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92ab1-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoff-put-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="92ab1-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="92ab1-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoff-put-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="92ab1-142">Java</span><span class="sxs-lookup"><span data-stu-id="92ab1-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timeoff-put-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="92ab1-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="92ab1-143">Response</span></span>

<span data-ttu-id="92ab1-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="92ab1-144">The following is an example of the response.</span></span> 

><span data-ttu-id="92ab1-145">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="92ab1-145">**Note:** The response object shown here might be shortened for readability.</span></span>
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


