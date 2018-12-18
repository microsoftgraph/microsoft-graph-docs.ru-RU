---
title: Удаление календаря
description: Удаление календаря, отличного от календаря по умолчанию.
author: angelgolfer-ms
ms.openlocfilehash: d8e2a7aaaff9f4489d5ef1cbcae97bcdbceb8f17
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348792"
---
# <a name="delete-calendar"></a><span data-ttu-id="8701e-103">Удаление календаря</span><span class="sxs-lookup"><span data-stu-id="8701e-103">Delete calendar</span></span>

> <span data-ttu-id="8701e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8701e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8701e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8701e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8701e-106">Удаление календаря, отличного от календаря по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8701e-106">Delete a calendar other than the default calendar.</span></span>
## <a name="permissions"></a><span data-ttu-id="8701e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8701e-107">Permissions</span></span>
<span data-ttu-id="8701e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8701e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8701e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8701e-110">Permission type</span></span>      | <span data-ttu-id="8701e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8701e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8701e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8701e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8701e-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8701e-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="8701e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8701e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8701e-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8701e-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="8701e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8701e-116">Application</span></span> | <span data-ttu-id="8701e-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8701e-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8701e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8701e-118">HTTP request</span></span>
<span data-ttu-id="8701e-119"><!-- { "blockType": "ignored" } -->Пользователя [календаря](../resources/calendar.md) , отличный от календаря по умолчанию в [calendarGroup](../resources/calendargroup.md)по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8701e-119"><!-- { "blockType": "ignored" } --> A user's [calendar](../resources/calendar.md) other than the default calendar in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendars/{id}

DELETE /me/calendarGroup/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="8701e-120">[Календарь](../resources/calendar.md), отличный от календаря по умолчанию, в определенной группе [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="8701e-120">A [calendar](../resources/calendar.md) other than the default calendar, in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
DELETE /me/calendarGroups/{id}/calendars/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="request-headers"></a><span data-ttu-id="8701e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8701e-121">Request headers</span></span>
| <span data-ttu-id="8701e-122">Имя</span><span class="sxs-lookup"><span data-stu-id="8701e-122">Name</span></span>           |  <span data-ttu-id="8701e-123">Тип</span><span class="sxs-lookup"><span data-stu-id="8701e-123">Type</span></span>    | <span data-ttu-id="8701e-124">Описание</span><span class="sxs-lookup"><span data-stu-id="8701e-124">Description</span></span>|
|:---------------|:---------|:----------|
| <span data-ttu-id="8701e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="8701e-125">Authorization</span></span>  |  <span data-ttu-id="8701e-126">string</span><span class="sxs-lookup"><span data-stu-id="8701e-126">string</span></span>  | <span data-ttu-id="8701e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8701e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8701e-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8701e-129">Request body</span></span>
<span data-ttu-id="8701e-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8701e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8701e-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="8701e-131">Response</span></span>

<span data-ttu-id="8701e-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="8701e-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8701e-134">Пример</span><span class="sxs-lookup"><span data-stu-id="8701e-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8701e-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="8701e-135">Request</span></span>
<span data-ttu-id="8701e-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8701e-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_calendar"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/calendar
```
##### <a name="response"></a><span data-ttu-id="8701e-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="8701e-137">Response</span></span>
<span data-ttu-id="8701e-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8701e-138">Here is an example of the response.</span></span> 
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
  "tocPath": ""
}-->
