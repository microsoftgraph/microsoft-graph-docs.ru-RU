---
title: Замена timeOff
description: Замените существующий объект timeOff.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b05916566f366793e683e413b3dd44076f2f76a5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051216"
---
# <a name="replace-timeoff"></a><span data-ttu-id="04ccc-103">Замена timeOff</span><span class="sxs-lookup"><span data-stu-id="04ccc-103">Replace timeOff</span></span>

<span data-ttu-id="04ccc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04ccc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="04ccc-105">Замените [существующий объект timeOff.](../resources/timeoff.md)</span><span class="sxs-lookup"><span data-stu-id="04ccc-105">Replace an existing [timeOff](../resources/timeoff.md) object.</span></span>

<span data-ttu-id="04ccc-106">Если указанного [объекта timeOff](../resources/timeoff.md) не существует, этот метод `404 Not found` возвращается.</span><span class="sxs-lookup"><span data-stu-id="04ccc-106">If the specified [timeOff](../resources/timeoff.md) object doesn't exist, this method returns `404 Not found`.</span></span>

## <a name="permissions"></a><span data-ttu-id="04ccc-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="04ccc-107">Permissions</span></span>

<span data-ttu-id="04ccc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04ccc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04ccc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="04ccc-110">Permission type</span></span>      | <span data-ttu-id="04ccc-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="04ccc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="04ccc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="04ccc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="04ccc-113">Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04ccc-113">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="04ccc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="04ccc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04ccc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04ccc-115">Not supported.</span></span>    |
|<span data-ttu-id="04ccc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="04ccc-116">Application</span></span> | <span data-ttu-id="04ccc-117">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04ccc-117">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="04ccc-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="04ccc-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="04ccc-119">Глобальные администраторы могут получать доступ к группам, в которых они не являются членами.</span><span class="sxs-lookup"><span data-stu-id="04ccc-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="04ccc-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="04ccc-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/timesOff/{timeOffId}
```

## <a name="request-headers"></a><span data-ttu-id="04ccc-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="04ccc-121">Request headers</span></span>

| <span data-ttu-id="04ccc-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="04ccc-122">Header</span></span>       | <span data-ttu-id="04ccc-123">Значение</span><span class="sxs-lookup"><span data-stu-id="04ccc-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="04ccc-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="04ccc-124">Authorization</span></span>  | <span data-ttu-id="04ccc-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="04ccc-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="04ccc-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="04ccc-127">Content-Type</span></span>  | <span data-ttu-id="04ccc-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="04ccc-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="04ccc-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="04ccc-130">Request body</span></span>

<span data-ttu-id="04ccc-131">В теле запроса поставляем представление JSON объекта [timeOff.](../resources/timeoff.md)</span><span class="sxs-lookup"><span data-stu-id="04ccc-131">In the request body, supply a JSON representation of a [timeOff](../resources/timeoff.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="04ccc-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="04ccc-132">Response</span></span>

<span data-ttu-id="04ccc-133">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект timeOff](../resources/timeoff.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="04ccc-133">If successful, this method returns a `200 OK` response code and a [timeOff](../resources/timeoff.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04ccc-134">Пример</span><span class="sxs-lookup"><span data-stu-id="04ccc-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="04ccc-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="04ccc-135">Request</span></span>

<span data-ttu-id="04ccc-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="04ccc-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="04ccc-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="04ccc-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoff-put"
}-->
```http
PUT https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/timesOff/{timeOffId}
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
# <a name="c"></a>[<span data-ttu-id="04ccc-138">C#</span><span class="sxs-lookup"><span data-stu-id="04ccc-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoff-put-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="04ccc-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="04ccc-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoff-put-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="04ccc-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="04ccc-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoff-put-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="04ccc-141">Java</span><span class="sxs-lookup"><span data-stu-id="04ccc-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timeoff-put-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


#### <a name="response"></a><span data-ttu-id="04ccc-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="04ccc-142">Response</span></span>

<span data-ttu-id="04ccc-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="04ccc-143">The following is an example of the response.</span></span> 

><span data-ttu-id="04ccc-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="04ccc-144">**Note:** The response object shown here might be shortened for readability.</span></span>
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

