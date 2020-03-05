---
title: 'user: reminderView'
description: 'Возвращает список напоминаний календаря за указанный период времени. '
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fb947dd0b7e08167b109d1a38baa537b74015f37
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451660"
---
# <a name="user-reminderview"></a><span data-ttu-id="d921b-103">user: reminderView</span><span class="sxs-lookup"><span data-stu-id="d921b-103">user: reminderView</span></span>

<span data-ttu-id="d921b-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d921b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d921b-105">Возвращает список напоминаний о событиях в календаре пользователя в заданных время начала и окончания.</span><span class="sxs-lookup"><span data-stu-id="d921b-105">Return a list of event reminders in a user calendar within the specified start and end times.</span></span> 

## <a name="permissions"></a><span data-ttu-id="d921b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d921b-106">Permissions</span></span>
<span data-ttu-id="d921b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d921b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d921b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d921b-109">Permission type</span></span>      | <span data-ttu-id="d921b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d921b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d921b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d921b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d921b-112">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d921b-112">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="d921b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d921b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d921b-114">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d921b-114">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="d921b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d921b-115">Application</span></span> | <span data-ttu-id="d921b-116">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d921b-116">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d921b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d921b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/reminderView(startDateTime=startDateTime-value,endDateTime=endDateTime-value)
```

## <a name="function-parameters"></a><span data-ttu-id="d921b-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="d921b-118">Function parameters</span></span>
<span data-ttu-id="d921b-119">В URL-адресе запроса укажите перечисленные ниже параметры функции и их значения.</span><span class="sxs-lookup"><span data-stu-id="d921b-119">In the request URL, provide the following function parameters with values.</span></span>

| <span data-ttu-id="d921b-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="d921b-120">Parameter</span></span>    | <span data-ttu-id="d921b-121">Тип</span><span class="sxs-lookup"><span data-stu-id="d921b-121">Type</span></span>   |<span data-ttu-id="d921b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d921b-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d921b-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d921b-123">startDateTime</span></span>|<span data-ttu-id="d921b-124">String</span><span class="sxs-lookup"><span data-stu-id="d921b-124">String</span></span>|<span data-ttu-id="d921b-p102">Дата и время начала события, для которого настроено напоминание. Значение представлено в формате ISO 8601, например "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="d921b-p102">The start date and time of the event for which the reminder is set up. The value is represented in ISO 8601 format, for example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="d921b-127">endDateTime</span><span class="sxs-lookup"><span data-stu-id="d921b-127">endDateTime</span></span>|<span data-ttu-id="d921b-128">String</span><span class="sxs-lookup"><span data-stu-id="d921b-128">String</span></span>|<span data-ttu-id="d921b-p103">Дата и время окончания события, для которого настроено напоминание. Значение представлено в формате ISO 8601, например "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="d921b-p103">The end date and time of the event for which the reminder is set up. The value is represented in ISO 8601 format, for example, "2015-11-08T20:00:00.0000000".</span></span>|

## <a name="request-headers"></a><span data-ttu-id="d921b-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d921b-131">Request headers</span></span>
| <span data-ttu-id="d921b-132">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d921b-132">Header</span></span>       | <span data-ttu-id="d921b-133">Значение</span><span class="sxs-lookup"><span data-stu-id="d921b-133">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="d921b-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d921b-134">Authorization</span></span>  | <span data-ttu-id="d921b-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d921b-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d921b-137">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d921b-137">Content-Type</span></span>   | <span data-ttu-id="d921b-138">application/json</span><span class="sxs-lookup"><span data-stu-id="d921b-138">application/json</span></span> |
| <span data-ttu-id="d921b-139">Prefer</span><span class="sxs-lookup"><span data-stu-id="d921b-139">Prefer</span></span> | <span data-ttu-id="d921b-p105">{Часовой пояс}. Необязательный. Если параметр не указан, по умолчанию используется формат UTC.</span><span class="sxs-lookup"><span data-stu-id="d921b-p105">{Time-zone}. Optional, UTC assumed if absent.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d921b-142">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d921b-142">Request body</span></span>
<span data-ttu-id="d921b-143">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d921b-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d921b-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="d921b-144">Response</span></span>

<span data-ttu-id="d921b-145">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции [reminder](../resources/reminder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d921b-145">If successful, this method returns `200 OK` response code and [reminder](../resources/reminder.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d921b-146">Пример</span><span class="sxs-lookup"><span data-stu-id="d921b-146">Example</span></span>
<span data-ttu-id="d921b-147">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="d921b-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d921b-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="d921b-148">Request</span></span>
<span data-ttu-id="d921b-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d921b-149">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d921b-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="d921b-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_reminderview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/reminderView(startDateTime='2017-06-05T10:00:00.0000000',endDateTime='2017-06-11T11:00:00.0000000')
```
# <a name="c"></a>[<span data-ttu-id="d921b-151">C#</span><span class="sxs-lookup"><span data-stu-id="d921b-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-reminderview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d921b-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d921b-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-reminderview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d921b-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d921b-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-reminderview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d921b-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="d921b-154">Response</span></span>
<span data-ttu-id="d921b-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d921b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
