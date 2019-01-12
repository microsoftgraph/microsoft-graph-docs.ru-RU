---
title: Создание объекта Event
description: С помощью этого API можно создать объект Event в календаре по умолчанию или указанном календаре.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 2736810865a6a41570c61b3ec1f8be4f8075019b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961262"
---
# <a name="create-event"></a><span data-ttu-id="c5210-103">Создание события</span><span class="sxs-lookup"><span data-stu-id="c5210-103">Create Event</span></span>

> <span data-ttu-id="c5210-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c5210-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c5210-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5210-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c5210-106">С помощью этого API можно создать объект Event в календаре по умолчанию или указанном календаре.</span><span class="sxs-lookup"><span data-stu-id="c5210-106">Use this API to create a new Event in the default or the specified calendar.</span></span>
## <a name="permissions"></a><span data-ttu-id="c5210-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c5210-107">Permissions</span></span>
<span data-ttu-id="c5210-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5210-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5210-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c5210-110">Permission type</span></span>      | <span data-ttu-id="c5210-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c5210-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5210-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c5210-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c5210-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c5210-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="c5210-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c5210-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5210-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c5210-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="c5210-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c5210-116">Application</span></span> | <span data-ttu-id="c5210-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c5210-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c5210-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c5210-118">HTTP request</span></span>
<span data-ttu-id="c5210-119"><!-- { "blockType": "ignored" } -->Пользователя или группы по умолчанию [календаря](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="c5210-119"><!-- { "blockType": "ignored" } --> A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
POST /me/calendar/events
POST /users/{id | userPrincipalName}/calendar/events
POST /groups/{id}/calendar/events
```
<span data-ttu-id="c5210-120">Экземпляр [calendar](../resources/calendar.md) пользователя в экземпляре по умолчанию [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="c5210-120">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendars/{id}/events

POST /me/calendarGroup/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="c5210-121">[Календарь](../resources/calendar.md) пользователя в определенной группе [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="c5210-121">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendarGroups/{id}/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="request-headers"></a><span data-ttu-id="c5210-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c5210-122">Request headers</span></span>
| <span data-ttu-id="c5210-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c5210-123">Header</span></span>       | <span data-ttu-id="c5210-124">Значение</span><span class="sxs-lookup"><span data-stu-id="c5210-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c5210-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c5210-125">Authorization</span></span>  | <span data-ttu-id="c5210-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c5210-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c5210-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c5210-128">Content-Type</span></span>  | <span data-ttu-id="c5210-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c5210-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c5210-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c5210-131">Request body</span></span>
<span data-ttu-id="c5210-132">Предоставьте в тексте запроса описание объекта [Event](../resources/event.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c5210-132">In the request body, supply a JSON representation of [Event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c5210-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5210-133">Response</span></span>

<span data-ttu-id="c5210-134">В случае успеха этот метод возвращает код отклика `201 Created` и объект [Event](../resources/event.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c5210-134">If successful, this method returns `201 Created` response code and [Event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5210-135">Пример</span><span class="sxs-lookup"><span data-stu-id="c5210-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c5210-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5210-136">Request</span></span>
<span data-ttu-id="c5210-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c5210-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_event_from_calendar"
}-->
```http
POST https://graph.microsoft.com/beta/me/calendar/events
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "2016-10-19T10:37:00Z"
  },
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```
<span data-ttu-id="c5210-138">Предоставьте в тексте запроса описание объекта [event](../resources/event.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c5210-138">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="c5210-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="c5210-139">Response</span></span>
<span data-ttu-id="c5210-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c5210-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "2016-10-19T10:37:00Z"
  },
  "uid": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
