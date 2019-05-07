---
title: Удаление календаря
description: Удаление календаря, отличного от календаря по умолчанию.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 03ee1f83f57b17e316a1663169bbdd112c55421f
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636074"
---
# <a name="delete-calendar"></a><span data-ttu-id="6406b-103">Удаление календаря</span><span class="sxs-lookup"><span data-stu-id="6406b-103">Delete calendar</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6406b-104">Удаление календаря, отличного от календаря по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="6406b-104">Delete a calendar other than the default calendar.</span></span>
## <a name="permissions"></a><span data-ttu-id="6406b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6406b-105">Permissions</span></span>
<span data-ttu-id="6406b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6406b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6406b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6406b-108">Permission type</span></span>      | <span data-ttu-id="6406b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6406b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6406b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6406b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6406b-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6406b-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="6406b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6406b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6406b-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6406b-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="6406b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6406b-114">Application</span></span> | <span data-ttu-id="6406b-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6406b-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="6406b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6406b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="6406b-117">[Календарь](../resources/calendar.md) пользователя, отличный от календаря по умолчанию, в группе [calendarGroup](../resources/calendargroup.md) по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="6406b-117">A user's [calendar](../resources/calendar.md) other than the default calendar in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}

DELETE /me/calendarGroup/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="6406b-118">[Календарь](../resources/calendar.md), отличный от календаря по умолчанию, в определенной группе [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="6406b-118">A [calendar](../resources/calendar.md) other than the default calendar, in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendarGroups/{id}/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="6406b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6406b-119">Request headers</span></span>
| <span data-ttu-id="6406b-120">Имя</span><span class="sxs-lookup"><span data-stu-id="6406b-120">Name</span></span>           |  <span data-ttu-id="6406b-121">Тип</span><span class="sxs-lookup"><span data-stu-id="6406b-121">Type</span></span>    | <span data-ttu-id="6406b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="6406b-122">Description</span></span>|
|:---------------|:---------|:----------|
| <span data-ttu-id="6406b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6406b-123">Authorization</span></span>  |  <span data-ttu-id="6406b-124">string</span><span class="sxs-lookup"><span data-stu-id="6406b-124">string</span></span>  | <span data-ttu-id="6406b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6406b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6406b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6406b-127">Request body</span></span>
<span data-ttu-id="6406b-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6406b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6406b-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="6406b-129">Response</span></span>

<span data-ttu-id="6406b-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="6406b-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6406b-132">Пример</span><span class="sxs-lookup"><span data-stu-id="6406b-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6406b-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="6406b-133">Request</span></span>
<span data-ttu-id="6406b-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6406b-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_calendar"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/calendar
```
##### <a name="response"></a><span data-ttu-id="6406b-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="6406b-135">Response</span></span>
<span data-ttu-id="6406b-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6406b-136">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="6406b-137">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="6406b-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6406b-138">Языках</span><span class="sxs-lookup"><span data-stu-id="6406b-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_calendar-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6406b-139">Язык</span><span class="sxs-lookup"><span data-stu-id="6406b-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_calendar-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/calendar-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/calendar-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
