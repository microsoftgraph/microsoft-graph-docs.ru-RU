---
title: 'user: reminderView'
description: 'Возвращает список напоминаний календаря за указанный период времени. '
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3fb0283aaae4f814f06b59a8a6ad6183cc18fec1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918212"
---
# <a name="user-reminderview"></a><span data-ttu-id="44cc7-103">user: reminderView</span><span class="sxs-lookup"><span data-stu-id="44cc7-103">user: reminderView</span></span>

> <span data-ttu-id="44cc7-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="44cc7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="44cc7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44cc7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="44cc7-106">Возвращает список событий напоминания в календаре пользователя в рамках указанного время начала и окончания.</span><span class="sxs-lookup"><span data-stu-id="44cc7-106">Return a list of event reminders in a user calendar within the specified start and end times.</span></span> 

## <a name="permissions"></a><span data-ttu-id="44cc7-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="44cc7-107">Permissions</span></span>
<span data-ttu-id="44cc7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44cc7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44cc7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="44cc7-110">Permission type</span></span>      | <span data-ttu-id="44cc7-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="44cc7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="44cc7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="44cc7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="44cc7-113">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="44cc7-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="44cc7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="44cc7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44cc7-115">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="44cc7-115">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="44cc7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="44cc7-116">Application</span></span> | <span data-ttu-id="44cc7-117">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="44cc7-117">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="44cc7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="44cc7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/reminderView(startDateTime=startDateTime-value,endDateTime=endDateTime-value)
```

## <a name="function-parameters"></a><span data-ttu-id="44cc7-119">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="44cc7-119">Function parameters</span></span>
<span data-ttu-id="44cc7-120">В URL-адресе запроса укажите перечисленные ниже параметры функции и их значения.</span><span class="sxs-lookup"><span data-stu-id="44cc7-120">In the request URL, provide the following function parameters with values.</span></span>

| <span data-ttu-id="44cc7-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="44cc7-121">Parameter</span></span>    | <span data-ttu-id="44cc7-122">Тип</span><span class="sxs-lookup"><span data-stu-id="44cc7-122">Type</span></span>   |<span data-ttu-id="44cc7-123">Описание</span><span class="sxs-lookup"><span data-stu-id="44cc7-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="44cc7-124">startDateTime</span><span class="sxs-lookup"><span data-stu-id="44cc7-124">startDateTime</span></span>|<span data-ttu-id="44cc7-125">String</span><span class="sxs-lookup"><span data-stu-id="44cc7-125">String</span></span>|<span data-ttu-id="44cc7-p103">Дата и время начала события, для которого настроено напоминание. Значение представлено в формате ISO 8601, например "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="44cc7-p103">The start date and time of the event for which the reminder is set up. The value is represented in ISO 8601 format, for example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="44cc7-128">endDateTime</span><span class="sxs-lookup"><span data-stu-id="44cc7-128">endDateTime</span></span>|<span data-ttu-id="44cc7-129">String</span><span class="sxs-lookup"><span data-stu-id="44cc7-129">String</span></span>|<span data-ttu-id="44cc7-p104">Дата и время окончания события, для которого настроено напоминание. Значение представлено в формате ISO 8601, например "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="44cc7-p104">The end date and time of the event for which the reminder is set up. The value is represented in ISO 8601 format, for example, "2015-11-08T20:00:00.0000000".</span></span>|

## <a name="request-headers"></a><span data-ttu-id="44cc7-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="44cc7-132">Request headers</span></span>
| <span data-ttu-id="44cc7-133">Заголовок</span><span class="sxs-lookup"><span data-stu-id="44cc7-133">Header</span></span>       | <span data-ttu-id="44cc7-134">Значение</span><span class="sxs-lookup"><span data-stu-id="44cc7-134">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="44cc7-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="44cc7-135">Authorization</span></span>  | <span data-ttu-id="44cc7-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="44cc7-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="44cc7-138">Content-Type</span><span class="sxs-lookup"><span data-stu-id="44cc7-138">Content-Type</span></span>   | <span data-ttu-id="44cc7-139">application/json</span><span class="sxs-lookup"><span data-stu-id="44cc7-139">application/json</span></span> |
| <span data-ttu-id="44cc7-140">Prefer</span><span class="sxs-lookup"><span data-stu-id="44cc7-140">Prefer</span></span> | <span data-ttu-id="44cc7-p106">{Часовой пояс}. Необязательный. Если параметр не указан, по умолчанию используется формат UTC.</span><span class="sxs-lookup"><span data-stu-id="44cc7-p106">{Time-zone}. Optional, UTC assumed if absent.</span></span>|

## <a name="request-body"></a><span data-ttu-id="44cc7-143">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="44cc7-143">Request body</span></span>
<span data-ttu-id="44cc7-144">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="44cc7-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="44cc7-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="44cc7-145">Response</span></span>

<span data-ttu-id="44cc7-146">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции [reminder](../resources/reminder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="44cc7-146">If successful, this method returns `200 OK` response code and [reminder](../resources/reminder.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44cc7-147">Пример</span><span class="sxs-lookup"><span data-stu-id="44cc7-147">Example</span></span>
<span data-ttu-id="44cc7-148">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="44cc7-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="44cc7-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="44cc7-149">Request</span></span>
<span data-ttu-id="44cc7-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="44cc7-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_reminderview"
}-->
```http
GET https://graph.microsoft.com/beta/me/reminderView(startDateTime='2017-06-05T10:00:00.0000000',endDateTime='2017-06-11T11:00:00.0000000')
```

##### <a name="response"></a><span data-ttu-id="44cc7-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="44cc7-151">Response</span></span>
<span data-ttu-id="44cc7-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="44cc7-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.reminder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 673

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.reminder)",
    "value": [
        {
            "eventId": "AAMkADNsvAAA=",
            "changeKey": "SuFHwDRP1EeXJUopWbSLlgAAmBvk2g==",
            "eventSubject": "Plan summer company picnic",
            "eventWebLink": "https://outlook.office365.com/owa/?itemid=AAMkADNsvAAA%3D&exvsurl=1&path=/calendar/item",
            "eventStartTime": {
                "dateTime": "2017-06-09T18:00:00.0000000",
                "timeZone": "UTC"
            },
            "eventEndTime": {
                "dateTime": "2017-06-09T19:00:00.0000000",
                "timeZone": "UTC"
            },
            "eventLocation": {
                "displayName": "Conf Room 3"
            },
            "reminderFireTime": {
                "dateTime": "2017-06-09T17:45:00.0000000",
                "timeZone": "UTC"
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: reminderView",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
