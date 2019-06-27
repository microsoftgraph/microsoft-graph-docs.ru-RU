---
title: Удаление календаря
description: Удаление календаря, отличного от календаря по умолчанию.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 9325308eb348c92a6352da3205c4bed230b02455
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262435"
---
# <a name="delete-calendar"></a><span data-ttu-id="b5069-103">Удаление календаря</span><span class="sxs-lookup"><span data-stu-id="b5069-103">Delete calendar</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5069-104">Удаление календаря, отличного от календаря по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b5069-104">Delete a calendar other than the default calendar.</span></span>
## <a name="permissions"></a><span data-ttu-id="b5069-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b5069-105">Permissions</span></span>
<span data-ttu-id="b5069-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5069-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5069-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b5069-108">Permission type</span></span>      | <span data-ttu-id="b5069-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b5069-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5069-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b5069-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b5069-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b5069-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="b5069-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b5069-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5069-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b5069-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="b5069-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b5069-114">Application</span></span> | <span data-ttu-id="b5069-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b5069-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b5069-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b5069-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="b5069-117">[Календарь](../resources/calendar.md) пользователя, отличный от календаря по умолчанию, в группе [calendarGroup](../resources/calendargroup.md) по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b5069-117">A user's [calendar](../resources/calendar.md) other than the default calendar in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}

DELETE /me/calendarGroup/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="b5069-118">[Календарь](../resources/calendar.md), отличный от календаря по умолчанию, в определенной группе [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="b5069-118">A [calendar](../resources/calendar.md) other than the default calendar, in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendarGroups/{id}/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b5069-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b5069-119">Request headers</span></span>
| <span data-ttu-id="b5069-120">Имя</span><span class="sxs-lookup"><span data-stu-id="b5069-120">Name</span></span>           |  <span data-ttu-id="b5069-121">Тип</span><span class="sxs-lookup"><span data-stu-id="b5069-121">Type</span></span>    | <span data-ttu-id="b5069-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b5069-122">Description</span></span>|
|:---------------|:---------|:----------|
| <span data-ttu-id="b5069-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5069-123">Authorization</span></span>  |  <span data-ttu-id="b5069-124">string</span><span class="sxs-lookup"><span data-stu-id="b5069-124">string</span></span>  | <span data-ttu-id="b5069-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b5069-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b5069-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b5069-127">Request body</span></span>
<span data-ttu-id="b5069-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b5069-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5069-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="b5069-129">Response</span></span>

<span data-ttu-id="b5069-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="b5069-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5069-132">Пример</span><span class="sxs-lookup"><span data-stu-id="b5069-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b5069-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5069-133">Request</span></span>
<span data-ttu-id="b5069-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b5069-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_calendar"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/calendar
```
##### <a name="response"></a><span data-ttu-id="b5069-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5069-135">Response</span></span>
<span data-ttu-id="b5069-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b5069-136">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="b5069-137">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="b5069-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b5069-138">C#</span><span class="sxs-lookup"><span data-stu-id="b5069-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_calendar-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b5069-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="b5069-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_calendar-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="b5069-140">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b5069-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_calendar-Objective-C-snippets.md)]
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
    "Error: /api-reference/beta/api/calendar-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/calendar-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/calendar-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
