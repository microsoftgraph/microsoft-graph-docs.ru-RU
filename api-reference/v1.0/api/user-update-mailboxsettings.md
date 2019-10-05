---
title: Обновление параметров почтового ящика пользователя
description: Обновление одного или нескольких параметров почтового ящика пользователя. Сюда входят параметры для автоматических ответов (уведомлять пользователей автоматически после получения их электронной почты), языковой стандарт (язык и страну или регион), часовой пояс и рабочие часы.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 0a224df7acdc0396d13743433d2cb407eb500d06
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402832"
---
# <a name="update-user-mailbox-settings"></a><span data-ttu-id="67932-104">Обновление параметров почтового ящика пользователя</span><span class="sxs-lookup"><span data-stu-id="67932-104">Update user mailbox settings</span></span>

<span data-ttu-id="67932-105">Включить, настроить или отключить один или несколько из следующих параметров в составе [mailboxSettings](../resources/mailboxsettings.md)пользователя:</span><span class="sxs-lookup"><span data-stu-id="67932-105">Enable, configure, or disable one or more of the following settings as part of a user's [mailboxSettings](../resources/mailboxsettings.md):</span></span>

- <span data-ttu-id="67932-106">[автоматические ответы](../resources/automaticrepliessetting.md) (уведомлять пользователей автоматически после получения их электронной почты)</span><span class="sxs-lookup"><span data-stu-id="67932-106">[automatic replies](../resources/automaticrepliessetting.md) (notify people automatically upon receipt of their email)</span></span>
- <span data-ttu-id="67932-107">dateFormat</span><span class="sxs-lookup"><span data-stu-id="67932-107">dateFormat</span></span>
- <span data-ttu-id="67932-108">[языковой стандарт](../resources/localeinfo.md) (язык и страна/регион)</span><span class="sxs-lookup"><span data-stu-id="67932-108">[locale](../resources/localeinfo.md) (language and country/region)</span></span>
- <span data-ttu-id="67932-109">тимеформат</span><span class="sxs-lookup"><span data-stu-id="67932-109">timeFormat</span></span>
- <span data-ttu-id="67932-110">часовой пояс</span><span class="sxs-lookup"><span data-stu-id="67932-110">time zone</span></span>
- [<span data-ttu-id="67932-111">рабочие часы</span><span class="sxs-lookup"><span data-stu-id="67932-111">working hours</span></span>](../resources/workinghours.md)

<span data-ttu-id="67932-112">При обновлении предпочтительного формата даты или времени для пользователя укажите его соответственно в [кратком формате даты](https://docs.microsoft.com/en-us/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortDate) или [коротком формате времени](https://docs.microsoft.com/en-us/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortTime) .</span><span class="sxs-lookup"><span data-stu-id="67932-112">When updating the preferred date or time format for a user, specify it in respectively, the [short date](https://docs.microsoft.com/en-us/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortDate) or [short time](https://docs.microsoft.com/en-us/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortTime) format.</span></span> 

<span data-ttu-id="67932-113">При обновлении предпочтительного часового пояса для пользователя укажите его в формате [часового пояса Windows или Internet Assigned Numbers Authority (IANA)](https://www.iana.org/time-zones) (также известного как часовой пояс Олсона).</span><span class="sxs-lookup"><span data-stu-id="67932-113">When updating the preferred time zone for a user, specify it in the Windows or [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="67932-114">Кроме того, можно настроить часовой пояс, как показано в [примере 2](#example-2) ниже.</span><span class="sxs-lookup"><span data-stu-id="67932-114">You can also further customize the time zone as shown in [example 2](#example-2) below.</span></span>

> [!TIP] 
> <span data-ttu-id="67932-115">Вы не можете создавать или удалять параметры почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="67932-115">You cannot create or delete any mailbox settings.</span></span>

## <a name="permissions"></a><span data-ttu-id="67932-116">Разрешения</span><span class="sxs-lookup"><span data-stu-id="67932-116">Permissions</span></span>
<span data-ttu-id="67932-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67932-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67932-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="67932-119">Permission type</span></span>      | <span data-ttu-id="67932-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="67932-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="67932-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="67932-121">Delegated (work or school account)</span></span> | <span data-ttu-id="67932-122">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="67932-122">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="67932-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="67932-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67932-124">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="67932-124">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="67932-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="67932-125">Application</span></span> | <span data-ttu-id="67932-126">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="67932-126">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="67932-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="67932-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailboxSettings
PATCH /users/{id|userPrincipalName}/mailboxSettings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="67932-128">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="67932-128">Optional query parameters</span></span>
<span data-ttu-id="67932-129">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="67932-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="67932-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="67932-130">Request headers</span></span>
| <span data-ttu-id="67932-131">Имя</span><span class="sxs-lookup"><span data-stu-id="67932-131">Name</span></span>       | <span data-ttu-id="67932-132">Тип</span><span class="sxs-lookup"><span data-stu-id="67932-132">Type</span></span> | <span data-ttu-id="67932-133">Описание</span><span class="sxs-lookup"><span data-stu-id="67932-133">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="67932-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="67932-134">Authorization</span></span>  | <span data-ttu-id="67932-135">string</span><span class="sxs-lookup"><span data-stu-id="67932-135">string</span></span>  | <span data-ttu-id="67932-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="67932-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="67932-138">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="67932-138">Request body</span></span>
<span data-ttu-id="67932-p105">В тексте запроса укажите значения для соответствующих свойств, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом изменений других значений свойств. Чтобы обеспечить максимальную производительность, не включайте существующие значения, которые не изменились, в запрос. Ниже перечислены свойства, значения которых можно записать или обновить.</span><span class="sxs-lookup"><span data-stu-id="67932-p105">In the request body, supply the values for the relevant properties that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. The following are the writable/updatable properties:</span></span>

| <span data-ttu-id="67932-143">Свойство</span><span class="sxs-lookup"><span data-stu-id="67932-143">Property</span></span>     | <span data-ttu-id="67932-144">Тип</span><span class="sxs-lookup"><span data-stu-id="67932-144">Type</span></span>   |<span data-ttu-id="67932-145">Описание</span><span class="sxs-lookup"><span data-stu-id="67932-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="67932-146">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="67932-146">automaticRepliesSetting</span></span>|[<span data-ttu-id="67932-147">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="67932-147">automaticRepliesSetting</span></span>](../resources/automaticrepliessetting.md)|<span data-ttu-id="67932-148">Параметры конфигурации для автоматического уведомления отправителя о входящем письме с помощью сообщения от пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="67932-148">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span> <span data-ttu-id="67932-149">Вы можете настроить такие уведомления только для диапазона дат в будущем.</span><span class="sxs-lookup"><span data-stu-id="67932-149">You can set such notifications for only a future date range.</span></span>|
|<span data-ttu-id="67932-150">dateFormat</span><span class="sxs-lookup"><span data-stu-id="67932-150">dateFormat</span></span>|<span data-ttu-id="67932-151">string</span><span class="sxs-lookup"><span data-stu-id="67932-151">string</span></span>|<span data-ttu-id="67932-152">Формат даты для почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="67932-152">The date format for the user's mailbox.</span></span>|
|<span data-ttu-id="67932-153">language</span><span class="sxs-lookup"><span data-stu-id="67932-153">language</span></span>|[<span data-ttu-id="67932-154">localeInfo</span><span class="sxs-lookup"><span data-stu-id="67932-154">localeInfo</span></span>](../resources/localeinfo.md)|<span data-ttu-id="67932-155">Сведения о языковом стандарте пользователя, в том числе о предпочитаемом языке и стране или регионе.</span><span class="sxs-lookup"><span data-stu-id="67932-155">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="67932-156">тимеформат</span><span class="sxs-lookup"><span data-stu-id="67932-156">timeFormat</span></span>|<span data-ttu-id="67932-157">string</span><span class="sxs-lookup"><span data-stu-id="67932-157">string</span></span>|<span data-ttu-id="67932-158">Формат времени для почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="67932-158">The time format for the user's mailbox.</span></span>|
|<span data-ttu-id="67932-159">timeZone</span><span class="sxs-lookup"><span data-stu-id="67932-159">timeZone</span></span>|<span data-ttu-id="67932-160">string</span><span class="sxs-lookup"><span data-stu-id="67932-160">string</span></span>|<span data-ttu-id="67932-161">Часовой пояс, используемый по умолчанию, для почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="67932-161">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="67932-162">workingHours</span><span class="sxs-lookup"><span data-stu-id="67932-162">workingHours</span></span>|[<span data-ttu-id="67932-163">workingHours</span><span class="sxs-lookup"><span data-stu-id="67932-163">workingHours</span></span>](../resources/workinghours.md)|<span data-ttu-id="67932-164">Часы, дни недели и часовой пояс работы пользователя.</span><span class="sxs-lookup"><span data-stu-id="67932-164">The hours, days of a week, and time zone that the user works.</span></span>|

## <a name="response"></a><span data-ttu-id="67932-165">Ответ</span><span class="sxs-lookup"><span data-stu-id="67932-165">Response</span></span>

<span data-ttu-id="67932-166">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленные свойства объекта [mailboxSettings](../resources/mailboxsettings.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="67932-166">If successful, this method returns a `200 OK` response code and the updated properties of a [mailboxSettings](../resources/mailboxsettings.md) object in the response body.</span></span>

## <a name="errors"></a><span data-ttu-id="67932-167">Ошибки</span><span class="sxs-lookup"><span data-stu-id="67932-167">Errors</span></span>

<span data-ttu-id="67932-168">Если заданы недопустимые значения рабочего времени, могут возникать указанные ниже ошибки.</span><span class="sxs-lookup"><span data-stu-id="67932-168">Setting working hours with inappropriate values may return the following errors.</span></span>

| <span data-ttu-id="67932-169">Сценарий</span><span class="sxs-lookup"><span data-stu-id="67932-169">Scenario</span></span>   | <span data-ttu-id="67932-170">Код состояния HTTP</span><span class="sxs-lookup"><span data-stu-id="67932-170">HTTP status code</span></span> | <span data-ttu-id="67932-171">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="67932-171">Error code</span></span> | <span data-ttu-id="67932-172">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="67932-172">Error message</span></span> |
|:-----------|:------|:----------|:----------|
| <span data-ttu-id="67932-173">Недопустимое значение **startTime** или **endTime**</span><span class="sxs-lookup"><span data-stu-id="67932-173">Invalid **startTime** or **endTime**</span></span> | <span data-ttu-id="67932-174">400</span><span class="sxs-lookup"><span data-stu-id="67932-174">400</span></span> | <span data-ttu-id="67932-175">RequestBodyRead</span><span class="sxs-lookup"><span data-stu-id="67932-175">RequestBodyRead</span></span> | <span data-ttu-id="67932-176">Не удается преобразовать литерал "08" в ожидаемый тип Edm.TimeOfDay.</span><span class="sxs-lookup"><span data-stu-id="67932-176">Cannot convert the literal '08' to the expected type 'Edm.TimeOfDay'.</span></span>|
| <span data-ttu-id="67932-177">Время начала больше времени окончания</span><span class="sxs-lookup"><span data-stu-id="67932-177">Start time is greater than end time</span></span> | <span data-ttu-id="67932-178">400</span><span class="sxs-lookup"><span data-stu-id="67932-178">400</span></span> | <span data-ttu-id="67932-179">ErrorInvalidTimeSettings</span><span class="sxs-lookup"><span data-stu-id="67932-179">ErrorInvalidTimeSettings</span></span> | <span data-ttu-id="67932-180">Время начало должно быть раньше, чем время окончания.</span><span class="sxs-lookup"><span data-stu-id="67932-180">Start Time should occur before End Time.</span></span> |
| <span data-ttu-id="67932-181">Недопустимый день в свойстве **daysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="67932-181">Invalid day in **daysOfWeek**</span></span> | <span data-ttu-id="67932-182">400</span><span class="sxs-lookup"><span data-stu-id="67932-182">400</span></span> | <span data-ttu-id="67932-183">InvalidArguments</span><span class="sxs-lookup"><span data-stu-id="67932-183">InvalidArguments</span></span> | <span data-ttu-id="67932-184">Запрашиваемое значение RandomDay не найдено.</span><span class="sxs-lookup"><span data-stu-id="67932-184">Requested value 'RandomDay' was not found.</span></span>|
| <span data-ttu-id="67932-185">Недопустимое значение **timeZone**</span><span class="sxs-lookup"><span data-stu-id="67932-185">Invalid **timeZone**</span></span> | <span data-ttu-id="67932-186">400</span><span class="sxs-lookup"><span data-stu-id="67932-186">400</span></span> | <span data-ttu-id="67932-187">InvalidTimeZone</span><span class="sxs-lookup"><span data-stu-id="67932-187">InvalidTimeZone</span></span> | <span data-ttu-id="67932-188">Указаны недопустимые параметры часового пояса.</span><span class="sxs-lookup"><span data-stu-id="67932-188">Time Zone settings provided are invalid.</span></span>|


## <a name="examples"></a><span data-ttu-id="67932-189">Примеры</span><span class="sxs-lookup"><span data-stu-id="67932-189">Examples</span></span>
### <a name="example-1"></a><span data-ttu-id="67932-190">Пример 1</span><span class="sxs-lookup"><span data-stu-id="67932-190">Example 1</span></span>
#### <a name="request"></a><span data-ttu-id="67932-191">Запрос</span><span class="sxs-lookup"><span data-stu-id="67932-191">Request</span></span> 
<span data-ttu-id="67932-192">В первом примере показано, как включить автоматические ответы для диапазона дат, настроив для свойства **automaticRepliesSetting** следующие свойства: **status**, **scheduledStartDateTime** и **scheduledEndDateTime**.</span><span class="sxs-lookup"><span data-stu-id="67932-192">The first example enables automatic replies for a date range, by setting the following properties of the **automaticRepliesSetting** property: **status**, **scheduledStartDateTime** and **scheduledEndDateTime**.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="67932-193">HTTP</span><span class="sxs-lookup"><span data-stu-id="67932-193">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_mailboxsettings_1"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/mailboxSettings
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/mailboxSettings",
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

#### <a name="response"></a><span data-ttu-id="67932-194">Ответ</span><span class="sxs-lookup"><span data-stu-id="67932-194">Response</span></span>
<span data-ttu-id="67932-195">Ответ включает обновленные параметры автоматических ответов.</span><span class="sxs-lookup"><span data-stu-id="67932-195">The response includes the updated settings for automatic replies.</span></span> <span data-ttu-id="67932-196">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="67932-196">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="67932-197">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="67932-197">All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/mailboxSettings",
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

### <a name="example-2"></a><span data-ttu-id="67932-198">Пример 2</span><span class="sxs-lookup"><span data-stu-id="67932-198">Example 2</span></span>
#### <a name="request"></a><span data-ttu-id="67932-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="67932-199">Request</span></span>
<span data-ttu-id="67932-200">Во втором примере настраивается часовой пояс для рабочего времени вошедшего пользователя. Для этого в свойстве **timeZone** указывается [пользовательский часовой пояс](../resources/customtimezone.md).</span><span class="sxs-lookup"><span data-stu-id="67932-200">The second example customizes the time zone for the working hours of the signed-in user, by setting the **timeZone** property to a [custom time zone](../resources/customtimezone.md).</span></span>

<!-- {
  "blockType": "ignored",
  "name": "update_mailboxsettings_2"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/mailboxSettings
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
#### <a name="response"></a><span data-ttu-id="67932-201">Отклик</span><span class="sxs-lookup"><span data-stu-id="67932-201">Response</span></span>
<span data-ttu-id="67932-p108">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="67932-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('94447c6e-ea4c-494c-a9ed-d905e366c5cb')/mailboxSettings",
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
<!-- {
  "type": "#page.annotation",
  "description": "Update mailbox settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
