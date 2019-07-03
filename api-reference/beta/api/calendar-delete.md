---
title: Удаление календаря
description: Удаление календаря, отличного от календаря по умолчанию.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 84d2b38b0e403425f9f552108338afdac0dee124
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35438939"
---
# <a name="delete-calendar"></a><span data-ttu-id="233ac-103">Удаление календаря</span><span class="sxs-lookup"><span data-stu-id="233ac-103">Delete calendar</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="233ac-104">Удаление календаря, отличного от календаря по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="233ac-104">Delete a calendar other than the default calendar.</span></span>
## <a name="permissions"></a><span data-ttu-id="233ac-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="233ac-105">Permissions</span></span>
<span data-ttu-id="233ac-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="233ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="233ac-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="233ac-108">Permission type</span></span>      | <span data-ttu-id="233ac-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="233ac-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="233ac-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="233ac-110">Delegated (work or school account)</span></span> | <span data-ttu-id="233ac-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="233ac-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="233ac-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="233ac-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="233ac-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="233ac-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="233ac-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="233ac-114">Application</span></span> | <span data-ttu-id="233ac-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="233ac-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="233ac-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="233ac-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="233ac-117">[Календарь](../resources/calendar.md) пользователя, отличный от календаря по умолчанию, в группе [calendarGroup](../resources/calendargroup.md) по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="233ac-117">A user's [calendar](../resources/calendar.md) other than the default calendar in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}

DELETE /me/calendarGroup/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="233ac-118">[Календарь](../resources/calendar.md), отличный от календаря по умолчанию, в определенной группе [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="233ac-118">A [calendar](../resources/calendar.md) other than the default calendar, in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendarGroups/{id}/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="233ac-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="233ac-119">Request headers</span></span>
| <span data-ttu-id="233ac-120">Имя</span><span class="sxs-lookup"><span data-stu-id="233ac-120">Name</span></span>           |  <span data-ttu-id="233ac-121">Тип</span><span class="sxs-lookup"><span data-stu-id="233ac-121">Type</span></span>    | <span data-ttu-id="233ac-122">Описание</span><span class="sxs-lookup"><span data-stu-id="233ac-122">Description</span></span>|
|:---------------|:---------|:----------|
| <span data-ttu-id="233ac-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="233ac-123">Authorization</span></span>  |  <span data-ttu-id="233ac-124">string</span><span class="sxs-lookup"><span data-stu-id="233ac-124">string</span></span>  | <span data-ttu-id="233ac-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="233ac-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="233ac-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="233ac-127">Request body</span></span>
<span data-ttu-id="233ac-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="233ac-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="233ac-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="233ac-129">Response</span></span>

<span data-ttu-id="233ac-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="233ac-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="233ac-132">Пример</span><span class="sxs-lookup"><span data-stu-id="233ac-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="233ac-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="233ac-133">Request</span></span>
<span data-ttu-id="233ac-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="233ac-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="233ac-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="233ac-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_calendar"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/calendar
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="233ac-136">C#</span><span class="sxs-lookup"><span data-stu-id="233ac-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-calendar-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="233ac-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="233ac-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-calendar-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="233ac-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="233ac-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-calendar-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="233ac-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="233ac-139">Response</span></span>
<span data-ttu-id="233ac-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="233ac-140">Here is an example of the response.</span></span> 
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
