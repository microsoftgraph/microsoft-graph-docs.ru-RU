---
title: Удаление календаря
description: Удаление календаря, отличного от календаря по умолчанию.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a42f3c8c4350f4c239a779cc27133a2201b5f3ef
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441006"
---
# <a name="delete-calendar"></a><span data-ttu-id="bb9b9-103">Удаление календаря</span><span class="sxs-lookup"><span data-stu-id="bb9b9-103">Delete calendar</span></span>

<span data-ttu-id="bb9b9-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="bb9b9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb9b9-105">Удаление календаря, отличного от календаря по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="bb9b9-105">Delete a calendar other than the default calendar.</span></span>
## <a name="permissions"></a><span data-ttu-id="bb9b9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bb9b9-106">Permissions</span></span>
<span data-ttu-id="bb9b9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb9b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb9b9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bb9b9-109">Permission type</span></span>      | <span data-ttu-id="bb9b9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bb9b9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bb9b9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bb9b9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bb9b9-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bb9b9-112">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="bb9b9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bb9b9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb9b9-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bb9b9-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="bb9b9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bb9b9-115">Application</span></span> | <span data-ttu-id="bb9b9-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bb9b9-116">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="bb9b9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bb9b9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="bb9b9-118">[Календарь](../resources/calendar.md) пользователя, отличный от календаря по умолчанию, в группе [calendarGroup](../resources/calendargroup.md) по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="bb9b9-118">A user's [calendar](../resources/calendar.md) other than the default calendar in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}

DELETE /me/calendarGroup/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="bb9b9-119">[Календарь](../resources/calendar.md), отличный от календаря по умолчанию, в определенной группе [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="bb9b9-119">A [calendar](../resources/calendar.md) other than the default calendar, in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendarGroups/{id}/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="bb9b9-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bb9b9-120">Request headers</span></span>
| <span data-ttu-id="bb9b9-121">Имя</span><span class="sxs-lookup"><span data-stu-id="bb9b9-121">Name</span></span>           |  <span data-ttu-id="bb9b9-122">Тип</span><span class="sxs-lookup"><span data-stu-id="bb9b9-122">Type</span></span>    | <span data-ttu-id="bb9b9-123">Описание</span><span class="sxs-lookup"><span data-stu-id="bb9b9-123">Description</span></span>|
|:---------------|:---------|:----------|
| <span data-ttu-id="bb9b9-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb9b9-124">Authorization</span></span>  |  <span data-ttu-id="bb9b9-125">string</span><span class="sxs-lookup"><span data-stu-id="bb9b9-125">string</span></span>  | <span data-ttu-id="bb9b9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb9b9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bb9b9-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bb9b9-128">Request body</span></span>
<span data-ttu-id="bb9b9-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bb9b9-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb9b9-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="bb9b9-130">Response</span></span>

<span data-ttu-id="bb9b9-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="bb9b9-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb9b9-133">Пример</span><span class="sxs-lookup"><span data-stu-id="bb9b9-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bb9b9-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="bb9b9-134">Request</span></span>
<span data-ttu-id="bb9b9-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bb9b9-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bb9b9-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="bb9b9-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_calendar"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/calendar
```
# <a name="c"></a>[<span data-ttu-id="bb9b9-137">C#</span><span class="sxs-lookup"><span data-stu-id="bb9b9-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-calendar-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bb9b9-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bb9b9-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-calendar-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bb9b9-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bb9b9-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-calendar-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="bb9b9-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb9b9-140">Response</span></span>
<span data-ttu-id="bb9b9-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bb9b9-141">Here is an example of the response.</span></span> 
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
  "description": "Delete calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
