---
title: Удаление календаря
description: Удаление календаря, отличного от календаря по умолчанию.
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 1ea1fa81b7917864d7d794bf66a10cdf507fa79a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434911"
---
# <a name="delete-calendar"></a><span data-ttu-id="b284f-103">Удаление календаря</span><span class="sxs-lookup"><span data-stu-id="b284f-103">Delete calendar</span></span>

<span data-ttu-id="b284f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b284f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b284f-105">Удаление календаря, отличного от календаря по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b284f-105">Delete a calendar other than the default calendar.</span></span>
## <a name="permissions"></a><span data-ttu-id="b284f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b284f-106">Permissions</span></span>
<span data-ttu-id="b284f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b284f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b284f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b284f-109">Permission type</span></span>      | <span data-ttu-id="b284f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b284f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b284f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b284f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b284f-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b284f-112">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="b284f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b284f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b284f-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b284f-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="b284f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b284f-115">Application</span></span> | <span data-ttu-id="b284f-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b284f-116">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b284f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b284f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="b284f-118">[Календарь](../resources/calendar.md) пользователя, отличный от календаря по умолчанию, в группе [calendarGroup](../resources/calendargroup.md) по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b284f-118">A user's [calendar](../resources/calendar.md) other than the default calendar in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}
```
<span data-ttu-id="b284f-119">[Календарь](../resources/calendar.md), отличный от календаря по умолчанию, в определенной группе [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="b284f-119">A [calendar](../resources/calendar.md) other than the default calendar, in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendarGroups/{id}/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b284f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b284f-120">Request headers</span></span>
| <span data-ttu-id="b284f-121">Имя</span><span class="sxs-lookup"><span data-stu-id="b284f-121">Name</span></span>           |  <span data-ttu-id="b284f-122">Тип</span><span class="sxs-lookup"><span data-stu-id="b284f-122">Type</span></span>    | <span data-ttu-id="b284f-123">Описание</span><span class="sxs-lookup"><span data-stu-id="b284f-123">Description</span></span>|
|:---------------|:---------|:----------|
| <span data-ttu-id="b284f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b284f-124">Authorization</span></span>  |  <span data-ttu-id="b284f-125">string</span><span class="sxs-lookup"><span data-stu-id="b284f-125">string</span></span>  | <span data-ttu-id="b284f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b284f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b284f-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b284f-128">Request body</span></span>
<span data-ttu-id="b284f-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b284f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b284f-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="b284f-130">Response</span></span>

<span data-ttu-id="b284f-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="b284f-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b284f-133">Пример</span><span class="sxs-lookup"><span data-stu-id="b284f-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b284f-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="b284f-134">Request</span></span>
<span data-ttu-id="b284f-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b284f-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b284f-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="b284f-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_calendar"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/calendar
```
# <a name="c"></a>[<span data-ttu-id="b284f-137">C#</span><span class="sxs-lookup"><span data-stu-id="b284f-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-calendar-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b284f-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b284f-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-calendar-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b284f-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b284f-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-calendar-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b284f-140">Java</span><span class="sxs-lookup"><span data-stu-id="b284f-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-calendar-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b284f-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="b284f-141">Response</span></span>
<span data-ttu-id="b284f-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b284f-142">Here is an example of the response.</span></span> 
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

