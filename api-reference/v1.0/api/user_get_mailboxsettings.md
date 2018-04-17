# <a name="get-user-mailbox-settings"></a><span data-ttu-id="da09e-101">Получение параметров почтового ящика пользователя</span><span class="sxs-lookup"><span data-stu-id="da09e-101">Get user mailbox settings</span></span>

<span data-ttu-id="da09e-p101">Получение объекта [mailboxSettings](../resources/mailboxsettings.md) пользователя. Этот объект включает параметры автоматических ответов (автоматического уведомления пользователей при получении электронных сообщений от них), языкового стандарта (язык и страна или регион), часового пояса и рабочего времени.</span><span class="sxs-lookup"><span data-stu-id="da09e-p101">Get the user's [mailboxSettings](../resources/mailboxsettings.md). This includes settings for automatic replies (notify people automatically upon receipt of their email), locale (language and country/region), and time zone.</span></span>

<span data-ttu-id="da09e-104">Вы можете просмотреть все параметры почтового ящика или получить определенные параметры.</span><span class="sxs-lookup"><span data-stu-id="da09e-104">You can view all mailbox settings, or, get specific settings.</span></span>

<span data-ttu-id="da09e-105">Часовой пояс относится к предпочтительным параметрам, настраиваемым пользователями.</span><span class="sxs-lookup"><span data-stu-id="da09e-105">Time zone is one of the preferred settings a user can set up for the user's mailbox.</span></span> <span data-ttu-id="da09e-106">Допустимые форматы часовых поясов включают в себя форматы Windows и [IANA, или Internet Assigned Numbers Authority](http://www.iana.org/time-zones) (последний еще зовется форматом часового пояса Олсона).</span><span class="sxs-lookup"><span data-stu-id="da09e-106">Valid time zone formats include the Windows time zone format and [Internet Assigned Numbers Authority (IANA) time zone](http://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="da09e-107">Формат Windows используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="da09e-107">The Windows format is the default.</span></span> 

<span data-ttu-id="da09e-108">Когда вы получаете предпочтительный часовой пояс пользователя, часовой пояс возвращается в том формате, который был настроен.</span><span class="sxs-lookup"><span data-stu-id="da09e-108">When you get a user's preferred time zone, the time zone is returned in the format that it was set up.</span></span> <span data-ttu-id="da09e-109">Чтобы задать определенный формат часового пояса (Windows или IANA), сначала [обновите предпочтительный часовой пояс в этом формате как параметр почтового ящика](user_update_mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="da09e-109">If you want that time zone to be in a specific format (Windows or IANA), you can first [update the preferred time zone in that format as a mailbox setting](user_update_mailboxsettings.md).</span></span> <span data-ttu-id="da09e-110">Затем вы сможете получить часовой пояс в этом формате.</span><span class="sxs-lookup"><span data-stu-id="da09e-110">Subsequently you will be able to get the time zone in that format.</span></span> <span data-ttu-id="da09e-111">Кроме того, вы можете управлять преобразованием форматов в своем приложении.</span><span class="sxs-lookup"><span data-stu-id="da09e-111">Alternatively, you can manage the format conversion separately in your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="da09e-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="da09e-112">Permissions</span></span>
<span data-ttu-id="da09e-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="da09e-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="da09e-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="da09e-115">Permission type</span></span>      | <span data-ttu-id="da09e-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="da09e-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da09e-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="da09e-117">Delegated (work or school account)</span></span> | <span data-ttu-id="da09e-118">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="da09e-118">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="da09e-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="da09e-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da09e-120">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="da09e-120">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="da09e-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="da09e-121">Application</span></span> | <span data-ttu-id="da09e-122">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="da09e-122">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="da09e-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="da09e-123">HTTP request</span></span>
<span data-ttu-id="da09e-124">Получение всех параметров почтового ящика пользователя:</span><span class="sxs-lookup"><span data-stu-id="da09e-124">To get all mailbox settings for a user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings
GET /users/{id|userPrincipalName}/mailboxSettings
```

<span data-ttu-id="da09e-125">Получение определенных параметров, например только параметров автоматических ответов, языкового стандарта, часового пояса или рабочего времени:</span><span class="sxs-lookup"><span data-stu-id="da09e-125">To get specific settings - for example, only the automatic replies settings, locale, or time zone:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings/automaticRepliesSetting
GET /users/{id|userPrincipalName}/mailboxSettings/automaticRepliesSetting

GET /me/mailboxSettings/language
GET /users/{id|userPrincipalName}/mailboxSettings/language

GET /me/mailboxSettings/timeZone
GET /users/{id|userPrincipalName}/mailboxSettings/timeZone

GET /me/mailboxSettings/workingHours
GET /users/{id|userPrincipalName}/mailboxSettings/workingHours
```
## <a name="optional-query-parameters"></a><span data-ttu-id="da09e-126">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="da09e-126">Optional query parameters</span></span>
<span data-ttu-id="da09e-127">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/ru-RU/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="da09e-127">This method supports the [OData Query Parameters](http://developer.microsoft.com/ru-RU/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="da09e-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="da09e-128">Request headers</span></span>
| <span data-ttu-id="da09e-129">Имя</span><span class="sxs-lookup"><span data-stu-id="da09e-129">Name</span></span>       | <span data-ttu-id="da09e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="da09e-130">Type</span></span> | <span data-ttu-id="da09e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="da09e-131">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="da09e-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="da09e-132">Authorization</span></span>  | <span data-ttu-id="da09e-133">string</span><span class="sxs-lookup"><span data-stu-id="da09e-133">string</span></span>  | <span data-ttu-id="da09e-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="da09e-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="da09e-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="da09e-136">Request body</span></span>
<span data-ttu-id="da09e-137">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="da09e-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da09e-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="da09e-138">Response</span></span>

<span data-ttu-id="da09e-139">При успешном выполнении этот метод возвращает код отклика `200 OK` и один из указанных ниже запрошенных объектов в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="da09e-139">If successful, this method returns a `200 OK` response code and one of the following requested objects in the response body:</span></span>

- <span data-ttu-id="da09e-140">Объект [mailboxSettings](../resources/mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="da09e-140">[mailboxSettings](../resources/mailboxsettings.md) object</span></span>
- <span data-ttu-id="da09e-141">Объект [automaticRepliesSetting](../resources/automaticRepliesSetting.md).</span><span class="sxs-lookup"><span data-stu-id="da09e-141">[automaticRepliesSetting](../resources/automaticRepliesSetting.md) object</span></span>
- <span data-ttu-id="da09e-142">Объект [localeInfo](../resources/localeinfo.md).</span><span class="sxs-lookup"><span data-stu-id="da09e-142">[localeInfo](../resources/localeinfo.md) object</span></span>
- <span data-ttu-id="da09e-143">Строка (для параметра **timeZone**).</span><span class="sxs-lookup"><span data-stu-id="da09e-143">string (for **timeZone**)</span></span>
- [<span data-ttu-id="da09e-144">workingHours</span><span class="sxs-lookup"><span data-stu-id="da09e-144">workingHours</span></span>](../resources/workinghours.md)

## <a name="example"></a><span data-ttu-id="da09e-145">Пример</span><span class="sxs-lookup"><span data-stu-id="da09e-145">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="da09e-146">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="da09e-146">Request 1</span></span>
<span data-ttu-id="da09e-147">В первом примере считываются все параметры часового пояса для почтового ящика вошедшего пользователя, в том числе параметры часового пояса, автоматических ответов, языкового стандарта (язык и страна или регион) и рабочего времени.</span><span class="sxs-lookup"><span data-stu-id="da09e-147">The first example gets all the mailbox settings of the signed-in user's mailbox, which include automatic replies settings, time zone, and language settings.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailboxSettings
```
##### <a name="response-1"></a><span data-ttu-id="da09e-148">Ответ 1</span><span class="sxs-lookup"><span data-stu-id="da09e-148">Response 1</span></span>
<span data-ttu-id="da09e-p106">Отклик включает все параметры почтового ящика. Примечание. Показанный здесь объект отклика может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="da09e-p106">The response includes all the mailbox settings. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxSettings"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/mailboxSettings",
    "automaticRepliesSetting": {
        "status": "Scheduled",
        "externalAudience": "All",
        "scheduledStartDateTime": {
            "dateTime": "2016-03-14T07:00:00.0000000",
            "timeZone": "UTC"
        },
        "scheduledEndDateTime": {
            "dateTime": "2016-03-28T07:00:00.0000000",
            "timeZone": "UTC"
        },
        "internalReplyMessage": "<html>\n<body>\n<p>I'm at our company's worldwide reunion and will respond to your message as soon as I return.<br>\n</p></body>\n</html>\n",
        "externalReplyMessage": "<html>\n<body>\n<p>I'm at the Contoso worldwide reunion and will respond to your message as soon as I return.<br>\n</p></body>\n</html>\n"
    },
    "timeZone":"UTC",
    "language":{
      "locale":"en-US",
      "displayName":"English (United States)"
    },
    "workingHours":{
        "daysOfWeek":[
            "monday",
            "tuesday",
            "wednesday",
            "thursday",
            "friday"
        ],
        "startTime":"08:00:00.0000000",
        "endTime":"17:00:00.0000000",
        "timeZone":{
            "name":"Pacific Standard Time"
        }
    }
}
```

##### <a name="request-2"></a><span data-ttu-id="da09e-152">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="da09e-152">Request 2</span></span>
<span data-ttu-id="da09e-153">Во втором примере показано, как получить только параметры автоматических ответов почтового ящика пользователя, выполнившего вход в систему.</span><span class="sxs-lookup"><span data-stu-id="da09e-153">The second example gets specifically the automatic replies settings of the signed-in user's mailbox.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_2"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailboxSettings/automaticRepliesSetting
```
##### <a name="response-2"></a><span data-ttu-id="da09e-154">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="da09e-154">Response 2</span></span>
<span data-ttu-id="da09e-p107">Отклик включает только параметры автоматических ответов. Примечание. Показанный здесь объект отклика может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="da09e-p107">The response includes only the automatic replies settings. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.automaticRepliesSetting"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/api/v1.0/$metadata#Me/mailboxSettings/automaticRepliesSetting",
    "status": "alwaysEnabled",
    "externalAudience": "None",
    "scheduledStartDateTime": {
        "dateTime": "2016-03-19T02:00:00.0000000",
        "timeZone": "UTC"
    },
    "scheduledEndDateTime": {
        "dateTime": "2016-03-20T02:00:00.0000000",
        "timeZone": "UTC"
    },
    "internalReplyMessage": "<html>\n<body>\n<p>I'm at our company's worldwide reunion and will respond to your message as soon as I return.<br>\n</p></body>\n</html>\n",
    "externalReplyMessage": "<html>\n<body>\n<p>I'm at the Contoso worldwide reunion and will respond to your message as soon as I return.<br>\n</p></body>\n</html>\n"
}
```


##### <a name="request-3"></a><span data-ttu-id="da09e-158">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="da09e-158">Request 3</span></span>
<span data-ttu-id="da09e-159">В третьем примере показано, как получить только параметры рабочего времени для почтового ящика пользователя, выполнившего вход в систему.</span><span class="sxs-lookup"><span data-stu-id="da09e-159">The second example gets specifically the automatic replies settings of the signed-in user's mailbox.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_mailboxsettings_3"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailboxSettings/workingHours
```
##### <a name="response-3"></a><span data-ttu-id="da09e-160">Ответ 3</span><span class="sxs-lookup"><span data-stu-id="da09e-160">Response 3</span></span>
<span data-ttu-id="da09e-161">Ответ включает только параметры рабочего времени.</span><span class="sxs-lookup"><span data-stu-id="da09e-161">The response includes only the working hours settings.</span></span> <span data-ttu-id="da09e-162">Обратите внимание, что рабочее время пользователя относится к [пользовательскому часовому поясу](../resources/customtimezone.md).</span><span class="sxs-lookup"><span data-stu-id="da09e-162">Notice that the user's work hours are in a [custom time zone](../resources/customtimezone.md).</span></span> <span data-ttu-id="da09e-163">Примечание. Представленный здесь объект ответа может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="da09e-163">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="da09e-164">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="da09e-164">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_mailboxsettings_3",
  "truncated": true,
  "@odata.type": "microsoft.graph.workingHours"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('94447c6e-ea4c-494c-a9ed-d905e366c5cb')/mailboxSettings/workingHours",
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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get mailbox settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->