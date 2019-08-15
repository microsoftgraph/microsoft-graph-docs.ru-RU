---
title: Обновление параметров почтового ящика пользователя
description: Обновление одного или нескольких параметров почтового ящика пользователя. Сюда входят параметры для автоматических ответов (уведомлять пользователей автоматически после получения их электронной почты), языковой стандарт (язык и страну или регион), часовой пояс и рабочие часы.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fe39d03850c9e3d006827593cb4151c0cdac376b
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36421801"
---
# <a name="update-user-mailbox-settings"></a><span data-ttu-id="b57a4-104">Обновление параметров почтового ящика пользователя</span><span class="sxs-lookup"><span data-stu-id="b57a4-104">Update user mailbox settings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b57a4-p102">Обновление одного или нескольких параметров почтового ящика пользователя. Это относится к параметрам [автоматических ответов](../resources/automaticrepliessetting.md) (автоматического уведомления пользователей после получения электронных сообщений от них), [языковых стандартов](../resources/localeinfo.md) (языка и страны или региона), часового пояса и [рабочего времени](../resources/workinghours.md).</span><span class="sxs-lookup"><span data-stu-id="b57a4-p102">Update one or more settings for the user's mailbox. This includes settings for [automatic replies](../resources/automaticrepliessetting.md) (notify people automatically upon receipt of their email), [locale](../resources/localeinfo.md) (language and country/region), time zone, and [working hours](../resources/workinghours.md).</span></span>

<span data-ttu-id="b57a4-107">Вы можете включить, настроить или отключить один или несколько этих параметров в составе объекта [mailboxSettings](../resources/mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="b57a4-107">You can enable, configure, or disable one or more of these settings as part of [mailboxSettings](../resources/mailboxsettings.md).</span></span>

<span data-ttu-id="b57a4-108">**Примечание.** Невозможно создать или удалить какие-либо параметры почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="b57a4-108">**Note** You cannot create or delete any mailbox settings.</span></span>

<span data-ttu-id="b57a4-109">Обновляя предпочтительный часовой пояс для пользователя, можете указать его в формате Windows или [часового пояса IANA](https://www.iana.org/time-zones) (также известен как часовой пояс Олсона).</span><span class="sxs-lookup"><span data-stu-id="b57a4-109">When you update the preferred time zone for a user, you can specify it in the Windows or  [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="b57a4-110">Кроме того, можно настроить часовой пояс, как показано в [примере 2](#request-2) ниже.</span><span class="sxs-lookup"><span data-stu-id="b57a4-110">You can also further customize the time zone as shown in [example 2](#request-2) below.</span></span>

## <a name="permissions"></a><span data-ttu-id="b57a4-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b57a4-111">Permissions</span></span>
<span data-ttu-id="b57a4-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b57a4-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b57a4-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b57a4-114">Permission type</span></span>      | <span data-ttu-id="b57a4-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b57a4-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b57a4-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b57a4-116">Delegated (work or school account)</span></span> | <span data-ttu-id="b57a4-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b57a4-117">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="b57a4-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b57a4-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b57a4-119">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b57a4-119">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="b57a4-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b57a4-120">Application</span></span> | <span data-ttu-id="b57a4-121">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b57a4-121">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b57a4-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b57a4-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailboxSettings
PATCH /users/{id|userPrincipalName}/mailboxSettings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b57a4-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b57a4-123">Optional query parameters</span></span>
<span data-ttu-id="b57a4-124">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b57a4-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b57a4-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b57a4-125">Request headers</span></span>
| <span data-ttu-id="b57a4-126">Имя</span><span class="sxs-lookup"><span data-stu-id="b57a4-126">Name</span></span>       | <span data-ttu-id="b57a4-127">Тип</span><span class="sxs-lookup"><span data-stu-id="b57a4-127">Type</span></span> | <span data-ttu-id="b57a4-128">Описание</span><span class="sxs-lookup"><span data-stu-id="b57a4-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b57a4-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="b57a4-129">Authorization</span></span>  | <span data-ttu-id="b57a4-130">string</span><span class="sxs-lookup"><span data-stu-id="b57a4-130">string</span></span>  | <span data-ttu-id="b57a4-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b57a4-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b57a4-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b57a4-133">Request body</span></span>
<span data-ttu-id="b57a4-p106">В тексте запроса укажите значения для соответствующих свойств, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом изменений других значений свойств. Чтобы обеспечить максимальную производительность, не включайте существующие значения, которые не изменились, в запрос. Ниже перечислены свойства, значения которых можно записать или обновить.</span><span class="sxs-lookup"><span data-stu-id="b57a4-p106">In the request body, supply the values for the relevant properties that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. The following are the writable/updatable properties:</span></span>

| <span data-ttu-id="b57a4-138">Свойство</span><span class="sxs-lookup"><span data-stu-id="b57a4-138">Property</span></span>     | <span data-ttu-id="b57a4-139">Тип</span><span class="sxs-lookup"><span data-stu-id="b57a4-139">Type</span></span>   |<span data-ttu-id="b57a4-140">Описание</span><span class="sxs-lookup"><span data-stu-id="b57a4-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b57a4-141">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="b57a4-141">automaticRepliesSetting</span></span>|[<span data-ttu-id="b57a4-142">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="b57a4-142">automaticRepliesSetting</span></span>](../resources/automaticrepliessetting.md)|<span data-ttu-id="b57a4-143">Параметры конфигурации для автоматического уведомления отправителя о входящем письме с помощью сообщения от пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="b57a4-143">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span> <span data-ttu-id="b57a4-144">Вы можете настроить такие уведомления только для диапазона дат в будущем.</span><span class="sxs-lookup"><span data-stu-id="b57a4-144">You can set such notifications for only a future date range.</span></span>|
|<span data-ttu-id="b57a4-145">language</span><span class="sxs-lookup"><span data-stu-id="b57a4-145">language</span></span>|[<span data-ttu-id="b57a4-146">localeInfo</span><span class="sxs-lookup"><span data-stu-id="b57a4-146">localeInfo</span></span>](../resources/localeinfo.md)|<span data-ttu-id="b57a4-147">Сведения о языковом стандарте пользователя, в том числе о предпочитаемом языке и стране или регионе.</span><span class="sxs-lookup"><span data-stu-id="b57a4-147">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="b57a4-148">timeZone</span><span class="sxs-lookup"><span data-stu-id="b57a4-148">timeZone</span></span>|<span data-ttu-id="b57a4-149">string</span><span class="sxs-lookup"><span data-stu-id="b57a4-149">string</span></span>|<span data-ttu-id="b57a4-150">Часовой пояс, используемый по умолчанию, для почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="b57a4-150">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="b57a4-151">workingHours</span><span class="sxs-lookup"><span data-stu-id="b57a4-151">workingHours</span></span>|[<span data-ttu-id="b57a4-152">workingHours</span><span class="sxs-lookup"><span data-stu-id="b57a4-152">workingHours</span></span>](../resources/workinghours.md)|<span data-ttu-id="b57a4-153">Часы, дни недели и часовой пояс работы пользователя.</span><span class="sxs-lookup"><span data-stu-id="b57a4-153">The hours, days of a week, and time zone that the user works.</span></span>|

## <a name="response"></a><span data-ttu-id="b57a4-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="b57a4-154">Response</span></span>

<span data-ttu-id="b57a4-155">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [mailboxSettings](../resources/mailboxsettings.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b57a4-155">If successful, this method returns a `200 OK` response code and [mailboxSettings](../resources/mailboxsettings.md) object in the response body.</span></span>

## <a name="errors"></a><span data-ttu-id="b57a4-156">Ошибки</span><span class="sxs-lookup"><span data-stu-id="b57a4-156">Errors</span></span>

<span data-ttu-id="b57a4-157">Если заданы недопустимые значения рабочего времени, могут возникать указанные ниже ошибки.</span><span class="sxs-lookup"><span data-stu-id="b57a4-157">Setting working hours with inappropriate values may return the following errors.</span></span>

| <span data-ttu-id="b57a4-158">Сценарий</span><span class="sxs-lookup"><span data-stu-id="b57a4-158">Scenario</span></span>   | <span data-ttu-id="b57a4-159">Код состояния HTTP</span><span class="sxs-lookup"><span data-stu-id="b57a4-159">HTTP status code</span></span> | <span data-ttu-id="b57a4-160">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="b57a4-160">Error code</span></span> | <span data-ttu-id="b57a4-161">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="b57a4-161">Error message</span></span> |
|:-----------|:------|:----------|:----------|
| <span data-ttu-id="b57a4-162">Недопустимое значение **startTime** или **endTime**</span><span class="sxs-lookup"><span data-stu-id="b57a4-162">Invalid **startTime** or **endTime**</span></span> | <span data-ttu-id="b57a4-163">400</span><span class="sxs-lookup"><span data-stu-id="b57a4-163">400</span></span> | <span data-ttu-id="b57a4-164">RequestBodyRead</span><span class="sxs-lookup"><span data-stu-id="b57a4-164">RequestBodyRead</span></span> | <span data-ttu-id="b57a4-165">Не удается преобразовать литерал "08" в ожидаемый тип Edm.TimeOfDay.</span><span class="sxs-lookup"><span data-stu-id="b57a4-165">Cannot convert the literal '08' to the expected type 'Edm.TimeOfDay'.</span></span>|
| <span data-ttu-id="b57a4-166">Время начала больше времени окончания</span><span class="sxs-lookup"><span data-stu-id="b57a4-166">Start time is greater than end time</span></span> | <span data-ttu-id="b57a4-167">400</span><span class="sxs-lookup"><span data-stu-id="b57a4-167">400</span></span> | <span data-ttu-id="b57a4-168">ErrorInvalidTimeSettings</span><span class="sxs-lookup"><span data-stu-id="b57a4-168">ErrorInvalidTimeSettings</span></span> | <span data-ttu-id="b57a4-169">Время начало должно быть раньше, чем время окончания.</span><span class="sxs-lookup"><span data-stu-id="b57a4-169">Start Time should occur before End Time.</span></span> |
| <span data-ttu-id="b57a4-170">Недопустимый день в свойстве **daysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="b57a4-170">Invalid day in **daysOfWeek**</span></span> | <span data-ttu-id="b57a4-171">400</span><span class="sxs-lookup"><span data-stu-id="b57a4-171">400</span></span> | <span data-ttu-id="b57a4-172">InvalidArguments</span><span class="sxs-lookup"><span data-stu-id="b57a4-172">InvalidArguments</span></span> | <span data-ttu-id="b57a4-173">Запрашиваемое значение RandomDay не найдено.</span><span class="sxs-lookup"><span data-stu-id="b57a4-173">Requested value 'RandomDay' was not found.</span></span>|
| <span data-ttu-id="b57a4-174">Недопустимое значение **timeZone**</span><span class="sxs-lookup"><span data-stu-id="b57a4-174">Invalid **timeZone**</span></span> | <span data-ttu-id="b57a4-175">400</span><span class="sxs-lookup"><span data-stu-id="b57a4-175">400</span></span> | <span data-ttu-id="b57a4-176">InvalidTimeZone</span><span class="sxs-lookup"><span data-stu-id="b57a4-176">InvalidTimeZone</span></span> | <span data-ttu-id="b57a4-177">Указаны недопустимые параметры часового пояса.</span><span class="sxs-lookup"><span data-stu-id="b57a4-177">Time Zone settings provided are invalid.</span></span>|


## <a name="example"></a><span data-ttu-id="b57a4-178">Пример</span><span class="sxs-lookup"><span data-stu-id="b57a4-178">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="b57a4-179">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="b57a4-179">Request 1</span></span>
<span data-ttu-id="b57a4-180">В первом примере показано, как включить автоматические ответы для диапазона дат, настроив для свойства **automaticRepliesSetting** следующие свойства: **status**, **scheduledStartDateTime** и **scheduledEndDateTime**.</span><span class="sxs-lookup"><span data-stu-id="b57a4-180">The first example enables automatic replies for a date range, by setting the following properties of the **automaticRepliesSetting** property: **status**, **scheduledStartDateTime** and **scheduledEndDateTime**.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b57a4-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="b57a4-181">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="b57a4-182">C#</span><span class="sxs-lookup"><span data-stu-id="b57a4-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-mailboxsettings-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b57a4-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b57a4-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-mailboxsettings-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b57a4-184">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b57a4-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-mailboxsettings-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-1"></a><span data-ttu-id="b57a4-185">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="b57a4-185">Response 1</span></span>
<span data-ttu-id="b57a4-186">Ответ включает обновленные параметры автоматических ответов.</span><span class="sxs-lookup"><span data-stu-id="b57a4-186">The response includes the updated settings for automatic replies.</span></span> <span data-ttu-id="b57a4-187">Примечание. Представленный здесь объект ответа может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="b57a4-187">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b57a4-188">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b57a4-188">All of the properties will be returned from an actual call.</span></span>
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


##### <a name="request-2"></a><span data-ttu-id="b57a4-189">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="b57a4-189">Request 2</span></span>
<span data-ttu-id="b57a4-190">Во втором примере настраивается часовой пояс для рабочего времени вошедшего пользователя. Для этого в свойстве **timeZone** указывается [пользовательский часовой пояс](../resources/customtimezone.md).</span><span class="sxs-lookup"><span data-stu-id="b57a4-190">The second example customizes the time zone for the working hours of the signed-in user, by setting the **timeZone** property to a [custom time zone](../resources/customtimezone.md).</span></span>

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
##### <a name="response-2"></a><span data-ttu-id="b57a4-191">Ответ 2</span><span class="sxs-lookup"><span data-stu-id="b57a4-191">Response 2</span></span>
<span data-ttu-id="b57a4-p109">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b57a4-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
