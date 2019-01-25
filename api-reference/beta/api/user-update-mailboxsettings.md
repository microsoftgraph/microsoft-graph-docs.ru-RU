---
title: Обновление параметров почтового ящика пользователя
description: Обновление одного или нескольких параметров почтового ящика пользователя. Это относится к параметрам автоматических ответов (автоматического уведомления пользователей после получения электронных сообщений от них), языковых стандартов (языка и страны или региона), часового пояса и рабочего времени.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 90140a5c6f7822730b172dbc5a424c97b2fafc39
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516226"
---
# <a name="update-user-mailbox-settings"></a><span data-ttu-id="59d27-104">Обновление параметров почтового ящика пользователя</span><span class="sxs-lookup"><span data-stu-id="59d27-104">Update user mailbox settings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59d27-p102">Обновление одного или нескольких параметров почтового ящика пользователя. Это относится к параметрам [автоматических ответов](../resources/automaticrepliessetting.md) (автоматического уведомления пользователей после получения электронных сообщений от них), [языковых стандартов](../resources/localeinfo.md) (языка и страны или региона), часового пояса и [рабочего времени](../resources/workinghours.md).</span><span class="sxs-lookup"><span data-stu-id="59d27-p102">Update one or more settings for the user's mailbox. This includes settings for [automatic replies](../resources/automaticrepliessetting.md) (notify people automatically upon receipt of their email), [locale](../resources/localeinfo.md) (language and country/region), time zone, and [working hours](../resources/workinghours.md).</span></span>

<span data-ttu-id="59d27-107">Вы можете включить, настроить или отключить один или несколько этих параметров в составе объекта [mailboxSettings](../resources/mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="59d27-107">You can enable, configure, or disable one or more of these settings as part of [mailboxSettings](../resources/mailboxsettings.md).</span></span>

<span data-ttu-id="59d27-108">**Примечание.** Невозможно создать или удалить какие-либо параметры почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="59d27-108">**Note** You cannot create or delete any mailbox settings.</span></span>

<span data-ttu-id="59d27-109">Обновляя предпочтительный часовой пояс для пользователя, можете указать его в формате Windows или [часового пояса IANA](https://www.iana.org/time-zones) (также известен как часовой пояс Олсона).</span><span class="sxs-lookup"><span data-stu-id="59d27-109">When you update the preferred time zone for a user, you can specify it in the Windows or  [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="59d27-110">Можно также настроить часовой пояс как показано в следующем [примере 2](#request-2) .</span><span class="sxs-lookup"><span data-stu-id="59d27-110">You can also further customize the time zone as shown in [example 2](#request-2) below.</span></span>

## <a name="permissions"></a><span data-ttu-id="59d27-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="59d27-111">Permissions</span></span>
<span data-ttu-id="59d27-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59d27-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59d27-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="59d27-114">Permission type</span></span>      | <span data-ttu-id="59d27-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="59d27-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59d27-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="59d27-116">Delegated (work or school account)</span></span> | <span data-ttu-id="59d27-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59d27-117">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="59d27-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="59d27-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59d27-119">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59d27-119">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="59d27-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="59d27-120">Application</span></span> | <span data-ttu-id="59d27-121">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59d27-121">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="59d27-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="59d27-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailboxSettings
PATCH /users/{id|userPrincipalName}/mailboxSettings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="59d27-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="59d27-123">Optional query parameters</span></span>
<span data-ttu-id="59d27-124">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="59d27-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="59d27-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="59d27-125">Request headers</span></span>
| <span data-ttu-id="59d27-126">Имя</span><span class="sxs-lookup"><span data-stu-id="59d27-126">Name</span></span>       | <span data-ttu-id="59d27-127">Тип</span><span class="sxs-lookup"><span data-stu-id="59d27-127">Type</span></span> | <span data-ttu-id="59d27-128">Описание</span><span class="sxs-lookup"><span data-stu-id="59d27-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="59d27-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="59d27-129">Authorization</span></span>  | <span data-ttu-id="59d27-130">string</span><span class="sxs-lookup"><span data-stu-id="59d27-130">string</span></span>  | <span data-ttu-id="59d27-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="59d27-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="59d27-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="59d27-133">Request body</span></span>
<span data-ttu-id="59d27-p106">В тексте запроса укажите значения для соответствующих свойств, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом изменений других значений свойств. Чтобы обеспечить максимальную производительность, не включайте существующие значения, которые не изменились, в запрос. Ниже перечислены свойства, значения которых можно записать или обновить.</span><span class="sxs-lookup"><span data-stu-id="59d27-p106">In the request body, supply the values for the relevant properties that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. The following are the writable/updatable properties:</span></span>

| <span data-ttu-id="59d27-138">Свойство</span><span class="sxs-lookup"><span data-stu-id="59d27-138">Property</span></span>     | <span data-ttu-id="59d27-139">Тип</span><span class="sxs-lookup"><span data-stu-id="59d27-139">Type</span></span>   |<span data-ttu-id="59d27-140">Описание</span><span class="sxs-lookup"><span data-stu-id="59d27-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="59d27-141">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="59d27-141">automaticRepliesSetting</span></span>|[<span data-ttu-id="59d27-142">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="59d27-142">automaticRepliesSetting</span></span>](../resources/automaticrepliessetting.md)|<span data-ttu-id="59d27-143">Параметры конфигурации для автоматического уведомления отправителя о входящем письме с помощью сообщения от пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="59d27-143">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span> <span data-ttu-id="59d27-144">Можно настроить такие уведомления для диапазон дат в будущем.</span><span class="sxs-lookup"><span data-stu-id="59d27-144">You can set such notifications for only a future date range.</span></span>|
|<span data-ttu-id="59d27-145">language</span><span class="sxs-lookup"><span data-stu-id="59d27-145">language</span></span>|[<span data-ttu-id="59d27-146">localeInfo</span><span class="sxs-lookup"><span data-stu-id="59d27-146">localeInfo</span></span>](../resources/localeinfo.md)|<span data-ttu-id="59d27-147">Сведения о языковом стандарте пользователя, в том числе о предпочитаемом языке и стране или регионе.</span><span class="sxs-lookup"><span data-stu-id="59d27-147">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="59d27-148">timeZone</span><span class="sxs-lookup"><span data-stu-id="59d27-148">timeZone</span></span>|<span data-ttu-id="59d27-149">string</span><span class="sxs-lookup"><span data-stu-id="59d27-149">string</span></span>|<span data-ttu-id="59d27-150">Часовой пояс почтового ящика пользователя по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="59d27-150">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="59d27-151">workingHours</span><span class="sxs-lookup"><span data-stu-id="59d27-151">workingHours</span></span>|[<span data-ttu-id="59d27-152">workingHours</span><span class="sxs-lookup"><span data-stu-id="59d27-152">workingHours</span></span>](../resources/workinghours.md)|<span data-ttu-id="59d27-153">Часы, дни недели и часовой пояс работы пользователя.</span><span class="sxs-lookup"><span data-stu-id="59d27-153">The hours, days of a week, and time zone that the user works.</span></span>|

## <a name="response"></a><span data-ttu-id="59d27-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="59d27-154">Response</span></span>

<span data-ttu-id="59d27-155">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [mailboxSettings](../resources/mailboxsettings.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="59d27-155">If successful, this method returns a `200 OK` response code and [mailboxSettings](../resources/mailboxsettings.md) object in the response body.</span></span>

## <a name="errors"></a><span data-ttu-id="59d27-156">Ошибки</span><span class="sxs-lookup"><span data-stu-id="59d27-156">Errors</span></span>

<span data-ttu-id="59d27-157">Если заданы недопустимые значения рабочего времени, могут возникать указанные ниже ошибки.</span><span class="sxs-lookup"><span data-stu-id="59d27-157">Setting working hours with inappropriate values may return the following errors.</span></span>

| <span data-ttu-id="59d27-158">Сценарий</span><span class="sxs-lookup"><span data-stu-id="59d27-158">Scenario</span></span>   | <span data-ttu-id="59d27-159">Код состояния HTTP</span><span class="sxs-lookup"><span data-stu-id="59d27-159">HTTP status code</span></span> | <span data-ttu-id="59d27-160">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="59d27-160">Error code</span></span> | <span data-ttu-id="59d27-161">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="59d27-161">Error message</span></span> |
|:-----------|:------|:----------|:----------|
| <span data-ttu-id="59d27-162">Недопустимое значение **startTime** или **endTime**</span><span class="sxs-lookup"><span data-stu-id="59d27-162">Invalid **startTime** or **endTime**</span></span> | <span data-ttu-id="59d27-163">400</span><span class="sxs-lookup"><span data-stu-id="59d27-163">400</span></span> | <span data-ttu-id="59d27-164">RequestBodyRead</span><span class="sxs-lookup"><span data-stu-id="59d27-164">RequestBodyRead</span></span> | <span data-ttu-id="59d27-165">Не удается преобразовать литерал "08" в ожидаемый тип Edm.TimeOfDay.</span><span class="sxs-lookup"><span data-stu-id="59d27-165">Cannot convert the literal '08' to the expected type 'Edm.TimeOfDay'.</span></span>|
| <span data-ttu-id="59d27-166">Время начала больше времени окончания</span><span class="sxs-lookup"><span data-stu-id="59d27-166">Start time is greater than end time</span></span> | <span data-ttu-id="59d27-167">400</span><span class="sxs-lookup"><span data-stu-id="59d27-167">400</span></span> | <span data-ttu-id="59d27-168">ErrorInvalidTimeSettings</span><span class="sxs-lookup"><span data-stu-id="59d27-168">ErrorInvalidTimeSettings</span></span> | <span data-ttu-id="59d27-169">Время начало должно быть раньше, чем время окончания.</span><span class="sxs-lookup"><span data-stu-id="59d27-169">Start Time should occur before End Time.</span></span> |
| <span data-ttu-id="59d27-170">Недопустимый день в свойстве **daysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="59d27-170">Invalid day in **daysOfWeek**</span></span> | <span data-ttu-id="59d27-171">400</span><span class="sxs-lookup"><span data-stu-id="59d27-171">400</span></span> | <span data-ttu-id="59d27-172">InvalidArguments</span><span class="sxs-lookup"><span data-stu-id="59d27-172">InvalidArguments</span></span> | <span data-ttu-id="59d27-173">Запрашиваемое значение RandomDay не найдено.</span><span class="sxs-lookup"><span data-stu-id="59d27-173">Requested value 'RandomDay' was not found.</span></span>|
| <span data-ttu-id="59d27-174">Недопустимое значение **timeZone**</span><span class="sxs-lookup"><span data-stu-id="59d27-174">Invalid **timeZone**</span></span> | <span data-ttu-id="59d27-175">400</span><span class="sxs-lookup"><span data-stu-id="59d27-175">400</span></span> | <span data-ttu-id="59d27-176">InvalidTimeZone</span><span class="sxs-lookup"><span data-stu-id="59d27-176">InvalidTimeZone</span></span> | <span data-ttu-id="59d27-177">Указаны недопустимые параметры часового пояса.</span><span class="sxs-lookup"><span data-stu-id="59d27-177">Time Zone settings provided are invalid.</span></span>|


## <a name="example"></a><span data-ttu-id="59d27-178">Пример</span><span class="sxs-lookup"><span data-stu-id="59d27-178">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="59d27-179">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="59d27-179">Request 1</span></span>
<span data-ttu-id="59d27-180">В первом примере показано, как включить автоматические ответы для диапазона дат, настроив для свойства **automaticRepliesSetting** следующие свойства: **status**, **scheduledStartDateTime** и **scheduledEndDateTime**.</span><span class="sxs-lookup"><span data-stu-id="59d27-180">The first example enables automatic replies for a date range, by setting the following properties of the **automaticRepliesSetting** property: **status**, **scheduledStartDateTime** and **scheduledEndDateTime**.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_mailboxsettings_1"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/mailboxSettings
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/mailboxSettings",
    "automaticRepliesSetting": {
        "status": "Scheduled",
        "scheduledStartDateTime": {
          "dateTime": "2016-03-20T18:00:00.0000000",
          "timeZone": "UTC"
        },
        "scheduledEndDateTime": {
          "dateTime": "2016-03-28T18:00:00.0000000",
          "timeZone": "UTC"
        }
    }
}
```
##### <a name="response-1"></a><span data-ttu-id="59d27-181">Ответ 1</span><span class="sxs-lookup"><span data-stu-id="59d27-181">Response 1</span></span>
<span data-ttu-id="59d27-182">Ответ включает обновленные параметры автоматических ответов.</span><span class="sxs-lookup"><span data-stu-id="59d27-182">The response includes the updated settings for automatic replies.</span></span> <span data-ttu-id="59d27-183">Примечание. Представленный здесь объект ответа может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="59d27-183">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="59d27-184">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="59d27-184">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "update_mailboxsettings_1",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxSettings"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/mailboxSettings",
    "automaticRepliesSetting": {
        "status": "scheduled",
        "externalAudience": "all",
        "scheduledStartDateTime": {
            "dateTime": "2016-03-20T02:00:00.0000000",
            "timeZone": "UTC"
        },
        "scheduledEndDateTime": {
            "dateTime": "2016-03-28T02:00:00.0000000",
            "timeZone": "UTC"
        },
    "internalReplyMessage": "<html>\n<body>\n<p>I'm at our company's worldwide reunion and will respond to your message as soon as I return.<br>\n</p></body>\n</html>\n",
    "externalReplyMessage": "<html>\n<body>\n<p>I'm at the Contoso worldwide reunion and will respond to your message as soon as I return.<br>\n</p></body>\n</html>\n"
    }
}
```


##### <a name="request-2"></a><span data-ttu-id="59d27-185">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="59d27-185">Request 2</span></span>
<span data-ttu-id="59d27-186">Во втором примере настраивается часовой пояс для рабочего времени вошедшего пользователя. Для этого в свойстве **timeZone** указывается [пользовательский часовой пояс](../resources/customtimezone.md).</span><span class="sxs-lookup"><span data-stu-id="59d27-186">The second example customizes the time zone for the working hours of the signed-in user, by setting the **timeZone** property to a [custom time zone](../resources/customtimezone.md).</span></span>

<!-- {
  "blockType": "ignored",
  "name": "update_mailboxsettings_2"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/mailboxSettings
Content-Type: application/json

{
  "workingHours": {
      "endTime" : "18:30:00.0000000", 
      "daysOfWeek": [ 
          "Monday", 
          "Tuesday", 
          "Wednesday", 
          "Thursday", 
          "Friday", 
          "Saturday" 
      ], 
      "timeZone" : { 
         "@odata.type": "#microsoft.graph.customTimeZone", 
         "bias":-300, 
         "name": "Customized Time Zone",
         "standardOffset":{   
           "time":"02:00:00.0000000", 
           "dayOccurrence":2, 
           "dayOfWeek":"Sunday", 
           "month":10, 
           "year":0 
         }, 
         "daylightOffset":{   
           "daylightBias":100, 
           "time":"02:00:00.0000000", 
           "dayOccurrence":4, 
           "dayOfWeek":"Sunday", 
           "month":5, 
           "year":0 
         } 
      } 
  }
} 
```
##### <a name="response-2"></a><span data-ttu-id="59d27-187">Ответ 2</span><span class="sxs-lookup"><span data-stu-id="59d27-187">Response 2</span></span>
<span data-ttu-id="59d27-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="59d27-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "update_mailboxsettings_2",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxSettings"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('94447c6e-ea4c-494c-a9ed-d905e366c5cb')/mailboxSettings",
    "workingHours":{
        "daysOfWeek":[
            "monday",
            "tuesday",
            "wednesday",
            "thursday",
            "friday",
            "saturday"
        ],
        "startTime":"09:00:00.0000000",
        "endTime":"18:30:00.0000000",
        "timeZone":{
            "@odata.type":"#microsoft.graph.customTimeZone",
            "bias":-200,
            "name":"Customized Time Zone",
            "standardOffset":{
                "time":"02:00:00.0000000",
                "dayOccurrence":4,
                "dayOfWeek":"sunday",
                "month":5,
                "year":0
            },
            "daylightOffset":{
                "daylightBias":-100,
                "time":"02:00:00.0000000",
                "dayOccurrence":2,
                "dayOfWeek":"sunday",
                "month":10,
                "year":0
            }
        }
    }
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update mailbox settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-update-mailboxsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
