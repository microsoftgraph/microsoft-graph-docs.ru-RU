---
title: 'user: reminderView'
description: 'Возвращает список напоминаний календаря за указанный период времени. '
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 34c2f1a55b6dea1daff36c5ce98d1959fd78b301
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510472"
---
# <a name="user-reminderview"></a><span data-ttu-id="c6f1a-103">user: reminderView</span><span class="sxs-lookup"><span data-stu-id="c6f1a-103">user: reminderView</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6f1a-104">Возвращает список событий напоминания в календаре пользователя в рамках указанного время начала и окончания.</span><span class="sxs-lookup"><span data-stu-id="c6f1a-104">Return a list of event reminders in a user calendar within the specified start and end times.</span></span> 

## <a name="permissions"></a><span data-ttu-id="c6f1a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c6f1a-105">Permissions</span></span>
<span data-ttu-id="c6f1a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6f1a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6f1a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c6f1a-108">Permission type</span></span>      | <span data-ttu-id="c6f1a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c6f1a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6f1a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c6f1a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c6f1a-111">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6f1a-111">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="c6f1a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c6f1a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6f1a-113">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6f1a-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="c6f1a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c6f1a-114">Application</span></span> | <span data-ttu-id="c6f1a-115">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6f1a-115">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c6f1a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c6f1a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/reminderView(startDateTime=startDateTime-value,endDateTime=endDateTime-value)
```

## <a name="function-parameters"></a><span data-ttu-id="c6f1a-117">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="c6f1a-117">Function parameters</span></span>
<span data-ttu-id="c6f1a-118">В URL-адресе запроса укажите перечисленные ниже параметры функции и их значения.</span><span class="sxs-lookup"><span data-stu-id="c6f1a-118">In the request URL, provide the following function parameters with values.</span></span>

| <span data-ttu-id="c6f1a-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="c6f1a-119">Parameter</span></span>    | <span data-ttu-id="c6f1a-120">Тип</span><span class="sxs-lookup"><span data-stu-id="c6f1a-120">Type</span></span>   |<span data-ttu-id="c6f1a-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c6f1a-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c6f1a-122">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c6f1a-122">startDateTime</span></span>|<span data-ttu-id="c6f1a-123">String</span><span class="sxs-lookup"><span data-stu-id="c6f1a-123">String</span></span>|<span data-ttu-id="c6f1a-p102">Дата и время начала события, для которого настроено напоминание. Значение представлено в формате ISO 8601, например "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="c6f1a-p102">The start date and time of the event for which the reminder is set up. The value is represented in ISO 8601 format, for example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="c6f1a-126">endDateTime</span><span class="sxs-lookup"><span data-stu-id="c6f1a-126">endDateTime</span></span>|<span data-ttu-id="c6f1a-127">String</span><span class="sxs-lookup"><span data-stu-id="c6f1a-127">String</span></span>|<span data-ttu-id="c6f1a-p103">Дата и время окончания события, для которого настроено напоминание. Значение представлено в формате ISO 8601, например "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="c6f1a-p103">The end date and time of the event for which the reminder is set up. The value is represented in ISO 8601 format, for example, "2015-11-08T20:00:00.0000000".</span></span>|

## <a name="request-headers"></a><span data-ttu-id="c6f1a-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c6f1a-130">Request headers</span></span>
| <span data-ttu-id="c6f1a-131">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c6f1a-131">Header</span></span>       | <span data-ttu-id="c6f1a-132">Значение</span><span class="sxs-lookup"><span data-stu-id="c6f1a-132">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="c6f1a-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c6f1a-133">Authorization</span></span>  | <span data-ttu-id="c6f1a-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c6f1a-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c6f1a-136">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c6f1a-136">Content-Type</span></span>   | <span data-ttu-id="c6f1a-137">application/json</span><span class="sxs-lookup"><span data-stu-id="c6f1a-137">application/json</span></span> |
| <span data-ttu-id="c6f1a-138">Prefer</span><span class="sxs-lookup"><span data-stu-id="c6f1a-138">Prefer</span></span> | <span data-ttu-id="c6f1a-p105">{Часовой пояс}. Необязательный. Если параметр не указан, по умолчанию используется формат UTC.</span><span class="sxs-lookup"><span data-stu-id="c6f1a-p105">{Time-zone}. Optional, UTC assumed if absent.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6f1a-141">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c6f1a-141">Request body</span></span>
<span data-ttu-id="c6f1a-142">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c6f1a-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c6f1a-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6f1a-143">Response</span></span>

<span data-ttu-id="c6f1a-144">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции [reminder](../resources/reminder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c6f1a-144">If successful, this method returns `200 OK` response code and [reminder](../resources/reminder.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6f1a-145">Пример</span><span class="sxs-lookup"><span data-stu-id="c6f1a-145">Example</span></span>
<span data-ttu-id="c6f1a-146">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="c6f1a-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c6f1a-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="c6f1a-147">Request</span></span>
<span data-ttu-id="c6f1a-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c6f1a-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_reminderview"
}-->
```http
GET https://graph.microsoft.com/beta/me/reminderView(startDateTime='2017-06-05T10:00:00.0000000',endDateTime='2017-06-11T11:00:00.0000000')
```

##### <a name="response"></a><span data-ttu-id="c6f1a-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="c6f1a-149">Response</span></span>
<span data-ttu-id="c6f1a-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="c6f1a-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "user: reminderView",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-reminderview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
