---
title: 'user: reminderView'
description: 'Возвращает список напоминаний календаря за указанный период времени. '
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 5def572e5d3a76b6d919cf5b5c13edb72bb6d12d
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2020
ms.locfileid: "43108258"
---
# <a name="user-reminderview"></a><span data-ttu-id="839a7-103">user: reminderView</span><span class="sxs-lookup"><span data-stu-id="839a7-103">user: reminderView</span></span>

<span data-ttu-id="839a7-104">Пространство имен: Microsoft. Graph возвращает список напоминаний о событиях в календаре пользователя в пределах указанного времени начала и окончания.</span><span class="sxs-lookup"><span data-stu-id="839a7-104">Namespace: microsoft.graph Return a list of event reminders in a user calendar within the specified start and end times.</span></span> 

## <a name="permissions"></a><span data-ttu-id="839a7-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="839a7-105">Permissions</span></span>
<span data-ttu-id="839a7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="839a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="839a7-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="839a7-108">Permission type</span></span>      | <span data-ttu-id="839a7-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="839a7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="839a7-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="839a7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="839a7-111">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="839a7-111">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="839a7-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="839a7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="839a7-113">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="839a7-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="839a7-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="839a7-114">Application</span></span> | <span data-ttu-id="839a7-115">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="839a7-115">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="839a7-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="839a7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/reminderView(startDateTime=startDateTime-value,endDateTime=endDateTime-value)
```

## <a name="function-parameters"></a><span data-ttu-id="839a7-117">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="839a7-117">Function parameters</span></span>
<span data-ttu-id="839a7-118">В URL-адресе запроса укажите перечисленные ниже параметры функции и их значения.</span><span class="sxs-lookup"><span data-stu-id="839a7-118">In the request URL, provide the following function parameters with values.</span></span>

| <span data-ttu-id="839a7-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="839a7-119">Parameter</span></span>    | <span data-ttu-id="839a7-120">Тип</span><span class="sxs-lookup"><span data-stu-id="839a7-120">Type</span></span>   |<span data-ttu-id="839a7-121">Описание</span><span class="sxs-lookup"><span data-stu-id="839a7-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="839a7-122">startDateTime</span><span class="sxs-lookup"><span data-stu-id="839a7-122">startDateTime</span></span>|<span data-ttu-id="839a7-123">String</span><span class="sxs-lookup"><span data-stu-id="839a7-123">String</span></span>|<span data-ttu-id="839a7-p102">Дата и время начала события, для которого настроено напоминание. Значение представлено в формате ISO 8601, например "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="839a7-p102">The start date and time of the event for which the reminder is set up. The value is represented in ISO 8601 format, for example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="839a7-126">endDateTime</span><span class="sxs-lookup"><span data-stu-id="839a7-126">endDateTime</span></span>|<span data-ttu-id="839a7-127">String</span><span class="sxs-lookup"><span data-stu-id="839a7-127">String</span></span>|<span data-ttu-id="839a7-p103">Дата и время окончания события, для которого настроено напоминание. Значение представлено в формате ISO 8601, например "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="839a7-p103">The end date and time of the event for which the reminder is set up. The value is represented in ISO 8601 format, for example, "2015-11-08T20:00:00.0000000".</span></span>|

## <a name="request-headers"></a><span data-ttu-id="839a7-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="839a7-130">Request headers</span></span>
| <span data-ttu-id="839a7-131">Заголовок</span><span class="sxs-lookup"><span data-stu-id="839a7-131">Header</span></span>       | <span data-ttu-id="839a7-132">Значение</span><span class="sxs-lookup"><span data-stu-id="839a7-132">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="839a7-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="839a7-133">Authorization</span></span>  | <span data-ttu-id="839a7-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="839a7-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="839a7-136">Content-Type</span><span class="sxs-lookup"><span data-stu-id="839a7-136">Content-Type</span></span>   | <span data-ttu-id="839a7-137">application/json</span><span class="sxs-lookup"><span data-stu-id="839a7-137">application/json</span></span> |
| <span data-ttu-id="839a7-138">Prefer</span><span class="sxs-lookup"><span data-stu-id="839a7-138">Prefer</span></span> | <span data-ttu-id="839a7-p105">{Часовой пояс}. Необязательный. Если параметр не указан, по умолчанию используется формат UTC.</span><span class="sxs-lookup"><span data-stu-id="839a7-p105">{Time-zone}. Optional, UTC assumed if absent.</span></span>|

## <a name="request-body"></a><span data-ttu-id="839a7-141">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="839a7-141">Request body</span></span>
<span data-ttu-id="839a7-142">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="839a7-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="839a7-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="839a7-143">Response</span></span>

<span data-ttu-id="839a7-144">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции [reminder](../resources/reminder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="839a7-144">If successful, this method returns `200 OK` response code and [reminder](../resources/reminder.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="839a7-145">Пример</span><span class="sxs-lookup"><span data-stu-id="839a7-145">Example</span></span>
<span data-ttu-id="839a7-146">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="839a7-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="839a7-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="839a7-147">Request</span></span>
<span data-ttu-id="839a7-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="839a7-148">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="839a7-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="839a7-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_reminderview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/reminderView(startDateTime='2017-06-05T10:00:00.0000000',endDateTime='2017-06-11T11:00:00.0000000')
```
# <a name="c"></a>[<span data-ttu-id="839a7-150">C#</span><span class="sxs-lookup"><span data-stu-id="839a7-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-reminderview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="839a7-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="839a7-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-reminderview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="839a7-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="839a7-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-reminderview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="839a7-153">Java</span><span class="sxs-lookup"><span data-stu-id="839a7-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-reminderview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="839a7-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="839a7-154">Response</span></span>
<span data-ttu-id="839a7-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="839a7-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.reminder)",
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
