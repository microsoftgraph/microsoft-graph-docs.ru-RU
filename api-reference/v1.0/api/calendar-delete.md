---
title: Удаление календаря
description: Удаление календаря, отличного от календаря по умолчанию.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: bd2947d3e39ae885e86af2a61a755148b68fc5b3
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36325367"
---
# <a name="delete-calendar"></a><span data-ttu-id="5d309-103">Удаление календаря</span><span class="sxs-lookup"><span data-stu-id="5d309-103">Delete calendar</span></span>

<span data-ttu-id="5d309-104">Удаление календаря, отличного от календаря по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5d309-104">Delete a calendar other than the default calendar.</span></span>
## <a name="permissions"></a><span data-ttu-id="5d309-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5d309-105">Permissions</span></span>
<span data-ttu-id="5d309-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d309-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d309-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5d309-108">Permission type</span></span>      | <span data-ttu-id="5d309-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5d309-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d309-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5d309-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5d309-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5d309-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="5d309-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5d309-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d309-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5d309-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="5d309-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5d309-114">Application</span></span> | <span data-ttu-id="5d309-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5d309-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d309-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5d309-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="5d309-117">[Календарь](../resources/calendar.md) пользователя, отличный от календаря по умолчанию, в группе [calendarGroup](../resources/calendargroup.md) по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5d309-117">A user's [calendar](../resources/calendar.md) other than the default calendar in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}

DELETE /me/calendarGroup/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="5d309-118">[Календарь](../resources/calendar.md), отличный от календаря по умолчанию, в определенной группе [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="5d309-118">A [calendar](../resources/calendar.md) other than the default calendar, in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendarGroups/{id}/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="5d309-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5d309-119">Request headers</span></span>
| <span data-ttu-id="5d309-120">Имя</span><span class="sxs-lookup"><span data-stu-id="5d309-120">Name</span></span>           |  <span data-ttu-id="5d309-121">Тип</span><span class="sxs-lookup"><span data-stu-id="5d309-121">Type</span></span>    | <span data-ttu-id="5d309-122">Описание</span><span class="sxs-lookup"><span data-stu-id="5d309-122">Description</span></span>|
|:---------------|:---------|:----------|
| <span data-ttu-id="5d309-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d309-123">Authorization</span></span>  |  <span data-ttu-id="5d309-124">string</span><span class="sxs-lookup"><span data-stu-id="5d309-124">string</span></span>  | <span data-ttu-id="5d309-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5d309-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5d309-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5d309-127">Request body</span></span>
<span data-ttu-id="5d309-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5d309-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5d309-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d309-129">Response</span></span>

<span data-ttu-id="5d309-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="5d309-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d309-132">Пример</span><span class="sxs-lookup"><span data-stu-id="5d309-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5d309-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="5d309-133">Request</span></span>
<span data-ttu-id="5d309-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5d309-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5d309-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="5d309-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_calendar"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/calendar
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5d309-136">C#</span><span class="sxs-lookup"><span data-stu-id="5d309-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-calendar-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5d309-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5d309-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-calendar-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5d309-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="5d309-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-calendar-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5d309-139">Java</span><span class="sxs-lookup"><span data-stu-id="5d309-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-calendar-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5d309-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d309-140">Response</span></span>
<span data-ttu-id="5d309-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5d309-141">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
