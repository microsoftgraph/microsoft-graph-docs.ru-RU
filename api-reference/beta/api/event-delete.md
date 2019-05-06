---
title: Удаление события
description: Удаление события.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 0467f421459cb349ab99a79ef00230de04dde172
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33587146"
---
# <a name="delete-event"></a><span data-ttu-id="8d7d5-103">Удаление события</span><span class="sxs-lookup"><span data-stu-id="8d7d5-103">Delete event</span></span>

<span data-ttu-id="8d7d5-104">Удаление события.</span><span class="sxs-lookup"><span data-stu-id="8d7d5-104">Delete event.</span></span>
## <a name="permissions"></a><span data-ttu-id="8d7d5-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8d7d5-105">Permissions</span></span>
<span data-ttu-id="8d7d5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d7d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d7d5-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8d7d5-108">Permission type</span></span>      | <span data-ttu-id="8d7d5-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8d7d5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d7d5-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8d7d5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8d7d5-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8d7d5-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="8d7d5-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8d7d5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d7d5-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8d7d5-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="8d7d5-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8d7d5-114">Application</span></span> | <span data-ttu-id="8d7d5-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8d7d5-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8d7d5-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8d7d5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/events/{id}
DELETE /users/{id | userPrincipalName}/events/{id}
DELETE /groups/{id}/events/{id}

DELETE /me/calendar/events/{id}
DELETE /users/{id | userPrincipalName}/calendar/events/{id}
DELETE /groups/{id}/calendar/events/{id}/

DELETE /me/calendars/{id}/events/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}/events/{id}

DELETE /me/calendargroup/calendars/{id}/events/{id}
DELETE /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}

DELETE /me/calendargroups/{id}/calendars/{id}/events/{id}
DELETE /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}
```
## <a name="request-headers"></a><span data-ttu-id="8d7d5-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8d7d5-117">Request headers</span></span>
| <span data-ttu-id="8d7d5-118">Имя</span><span class="sxs-lookup"><span data-stu-id="8d7d5-118">Name</span></span>       | <span data-ttu-id="8d7d5-119">Тип</span><span class="sxs-lookup"><span data-stu-id="8d7d5-119">Type</span></span> | <span data-ttu-id="8d7d5-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8d7d5-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8d7d5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d7d5-121">Authorization</span></span>  | <span data-ttu-id="8d7d5-122">string</span><span class="sxs-lookup"><span data-stu-id="8d7d5-122">string</span></span>  | <span data-ttu-id="8d7d5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8d7d5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8d7d5-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8d7d5-125">Request body</span></span>
<span data-ttu-id="8d7d5-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8d7d5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d7d5-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d7d5-127">Response</span></span>

<span data-ttu-id="8d7d5-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="8d7d5-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d7d5-130">Пример</span><span class="sxs-lookup"><span data-stu-id="8d7d5-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8d7d5-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d7d5-131">Request</span></span>
<span data-ttu-id="8d7d5-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8d7d5-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_event"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/events/{id}
```
##### <a name="response"></a><span data-ttu-id="8d7d5-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d7d5-133">Response</span></span>
<span data-ttu-id="8d7d5-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8d7d5-134">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="8d7d5-135">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="8d7d5-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8d7d5-136">Языках</span><span class="sxs-lookup"><span data-stu-id="8d7d5-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_event-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8d7d5-137">Язык</span><span class="sxs-lookup"><span data-stu-id="8d7d5-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_event-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/event-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/event-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
