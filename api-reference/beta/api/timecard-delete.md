---
title: Удаление timeCard
description: Удаление экземпляра timeCard в расписании.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: fc76b48ac1bac83435446d50e93a93ef256a49be
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869732"
---
# <a name="delete-timecard"></a><span data-ttu-id="c96d6-103">Удаление timeCard</span><span class="sxs-lookup"><span data-stu-id="c96d6-103">Delete timeCard</span></span>

<span data-ttu-id="c96d6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c96d6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c96d6-105">Удаление [экземпляра timeCard](../resources/timeCard.md) в [расписании.](../resources/schedule.md)</span><span class="sxs-lookup"><span data-stu-id="c96d6-105">Delete a [timeCard](../resources/timeCard.md) instance in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c96d6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c96d6-106">Permissions</span></span>

<span data-ttu-id="c96d6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c96d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c96d6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c96d6-109">Permission type</span></span>      | <span data-ttu-id="c96d6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c96d6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c96d6-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c96d6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c96d6-112">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c96d6-112">Schedule.ReadWrite.All</span></span>    |
|<span data-ttu-id="c96d6-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c96d6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c96d6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c96d6-114">Not supported.</span></span>    |
|<span data-ttu-id="c96d6-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="c96d6-115">Application</span></span> | <span data-ttu-id="c96d6-116">Schedule.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="c96d6-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="c96d6-117">\***Важно:** При использовании разрешений приложения необходимо включить в запрос `MS-APP-ACTS-AS` заготвую.</span><span class="sxs-lookup"><span data-stu-id="c96d6-117">\* **Important:** When you use application permissions, you must include the `MS-APP-ACTS-AS` header in the request.</span></span>

## <a name="http-request"></a><span data-ttu-id="c96d6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c96d6-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timecards/{timeCardID}
```

## <a name="request-headers"></a><span data-ttu-id="c96d6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c96d6-119">Request headers</span></span>

| <span data-ttu-id="c96d6-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c96d6-120">Header</span></span>       | <span data-ttu-id="c96d6-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c96d6-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c96d6-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c96d6-122">Authorization</span></span>  | <span data-ttu-id="c96d6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c96d6-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c96d6-125">MS-APP-ACTS-AS</span><span class="sxs-lookup"><span data-stu-id="c96d6-125">MS-APP-ACTS-AS</span></span> | <span data-ttu-id="c96d6-126">ID пользователя, от имени которого действует приложение.</span><span class="sxs-lookup"><span data-stu-id="c96d6-126">The ID of the user on behalf of whom the app is acting.</span></span> <span data-ttu-id="c96d6-127">Требуется при использовании области разрешений приложения.</span><span class="sxs-lookup"><span data-stu-id="c96d6-127">Required when you use the application permission scope.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c96d6-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c96d6-128">Request body</span></span>
<span data-ttu-id="c96d6-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c96d6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c96d6-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="c96d6-130">Response</span></span>

<span data-ttu-id="c96d6-131">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c96d6-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c96d6-132">Пример</span><span class="sxs-lookup"><span data-stu-id="c96d6-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="c96d6-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="c96d6-133">Request</span></span>
<span data-ttu-id="c96d6-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c96d6-134">The following is an example of the request.</span></span> 


# <a name="http"></a>[<span data-ttu-id="c96d6-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="c96d6-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timecard-delete"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/871dbd5c-3a6a-4392-bfe1-042452793a50/schedule/timecards/3895809b-a618-4c0d-86a0-d42b25b7d74f
```
# <a name="c"></a>[<span data-ttu-id="c96d6-136">C#</span><span class="sxs-lookup"><span data-stu-id="c96d6-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timecard-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c96d6-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c96d6-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timecard-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c96d6-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c96d6-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timecard-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c96d6-139">Java</span><span class="sxs-lookup"><span data-stu-id="c96d6-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timecard-delete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c96d6-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="c96d6-140">Response</span></span>

<span data-ttu-id="c96d6-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c96d6-141">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete timeCard",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
