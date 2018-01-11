# <a name="get-user-mailbox-settings"></a><span data-ttu-id="ee754-101">Получение параметров почтового ящика пользователя</span><span class="sxs-lookup"><span data-stu-id="ee754-101">Get user mailbox settings</span></span>

<span data-ttu-id="ee754-p101">Получение объекта [mailboxSettings](../resources/mailboxsettings.md) пользователя. Этот объект включает параметры автоматических ответов (автоматического уведомления пользователей при получении их почты), языкового стандарта (сведения о языке и стране или регионе) и часового пояса.</span><span class="sxs-lookup"><span data-stu-id="ee754-p101">Get the user's [mailboxSettings](../resources/mailboxsettings.md). This includes settings for automatic replies (notify people automatically upon receipt of their email), locale (language and country/region), and time zone.</span></span>

<span data-ttu-id="ee754-104">Вы можете просмотреть все параметры почтового ящика или получить определенные параметры.</span><span class="sxs-lookup"><span data-stu-id="ee754-104">You can view all mailbox settings, or, get specific settings.</span></span>

<span data-ttu-id="ee754-105">Часовой пояс относится к предпочтительным параметрам, настраиваемым пользователями.</span><span class="sxs-lookup"><span data-stu-id="ee754-105">Time zone is one of the preferred settings a user can set up for the user's mailbox.</span></span> <span data-ttu-id="ee754-106">Допустимые форматы часовых поясов включают в себя форматы Windows и [IANA, или Internet Assigned Numbers Authority]((http://www.iana.org/time-zones)) (последний еще зовется форматом часового пояса Олсона).</span><span class="sxs-lookup"><span data-stu-id="ee754-106">Valid time zone formats include the Windows time zone format and [Internet Assigned Numbers Authority (IANA) time zone]((http://www.iana.org/time-zones)) (also known as Olson time zone) format.</span></span> <span data-ttu-id="ee754-107">Формат Windows используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ee754-107">The Windows format is the default.</span></span> 

<span data-ttu-id="ee754-108">Когда вы получаете предпочтительный часовой пояс пользователя, часовой пояс возвращается в том формате, который был настроен.</span><span class="sxs-lookup"><span data-stu-id="ee754-108">When you get a user's preferred time zone, the time zone is returned in the format that it was set up.</span></span> <span data-ttu-id="ee754-109">Чтобы задать определенный формат часового пояса (Windows или IANA), сначала [обновите предпочтительный часовой пояс в этом формате как параметр почтового ящика](user_update_mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="ee754-109">If you want that time zone to be in a specific format (Windows or IANA), you can first [update the preferred time zone in that format as a mailbox setting](user_update_mailboxsettings.md).</span></span> <span data-ttu-id="ee754-110">Затем вы сможете получить часовой пояс в этом формате.</span><span class="sxs-lookup"><span data-stu-id="ee754-110">Subsequently you will be able to get the time zone in that format.</span></span> <span data-ttu-id="ee754-111">Кроме того, вы можете управлять преобразованием форматов в своем приложении.</span><span class="sxs-lookup"><span data-stu-id="ee754-111">Alternatively, you can manage the format conversion separately in your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="ee754-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ee754-112">Permissions</span></span>
<span data-ttu-id="ee754-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ee754-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ee754-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ee754-115">Permission type</span></span>      | <span data-ttu-id="ee754-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ee754-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee754-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ee754-117">Delegated (work or school account)</span></span> | <span data-ttu-id="ee754-118">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ee754-118">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="ee754-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ee754-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee754-120">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ee754-120">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="ee754-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ee754-121">Application</span></span> | <span data-ttu-id="ee754-122">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ee754-122">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ee754-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ee754-123">HTTP request</span></span>
<span data-ttu-id="ee754-124">Чтобы получить все параметры почтового ящика, включающие параметры автоматических ответов, используйте указанные ниже команды.</span><span class="sxs-lookup"><span data-stu-id="ee754-124">To get all mailbox settings which include automatic replies settings:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings
GET /users/{id|userPrincipalName}/mailboxSettings
```

<span data-ttu-id="ee754-125">Чтобы получить определенные параметры, например только параметры автоматических ответов, сведения о языковом стандарте и часовом поясе, выполните указанные ниже команды.</span><span class="sxs-lookup"><span data-stu-id="ee754-125">To get specific settings - for example, only the automatic replies settings, locale, or time zone:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings/automaticRepliesSetting
GET /users/{id|userPrincipalName}/mailboxSettings/automaticRepliesSetting

GET /me/mailboxSettings/language
GET /users/{id|userPrincipalName}/mailboxSettings/language

GET /me/mailboxSettings/timeZone
GET /users/{id|userPrincipalName}/mailboxSettings/timeZone
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ee754-126">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ee754-126">Optional query parameters</span></span>
<span data-ttu-id="ee754-127">Этот метод поддерживает [параметры запросов OData]((http://developer.microsoft.com/ru-RU/graph/docs/overview/query_parameters)) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ee754-127">This method supports the [OData Query Parameters]((http://developer.microsoft.com/ru-RU/graph/docs/overview/query_parameters)) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ee754-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ee754-128">Request headers</span></span>
| <span data-ttu-id="ee754-129">Имя</span><span class="sxs-lookup"><span data-stu-id="ee754-129">Name</span></span>       | <span data-ttu-id="ee754-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ee754-130">Type</span></span> | <span data-ttu-id="ee754-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ee754-131">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ee754-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee754-132">Authorization</span></span>  | <span data-ttu-id="ee754-133">string</span><span class="sxs-lookup"><span data-stu-id="ee754-133">string</span></span>  | <span data-ttu-id="ee754-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ee754-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ee754-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ee754-136">Request body</span></span>
<span data-ttu-id="ee754-137">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ee754-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee754-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee754-138">Response</span></span>

<span data-ttu-id="ee754-139">При успешном выполнении этот метод возвращает код отклика `200 OK` и один из указанных ниже запрошенных объектов в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ee754-139">If successful, this method returns a `200 OK` response code and one of the following requested objects in the response body:</span></span>

- <span data-ttu-id="ee754-140">Объект [mailboxSettings](../resources/mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="ee754-140">[mailboxSettings](../resources/mailboxsettings.md) object</span></span>
- <span data-ttu-id="ee754-141">Объект [automaticRepliesSetting](../resources/automaticRepliesSetting.md).</span><span class="sxs-lookup"><span data-stu-id="ee754-141">[automaticRepliesSetting](../resources/automaticRepliesSetting.md) object</span></span>
- <span data-ttu-id="ee754-142">Объект [localeInfo](../resources/localeinfo.md).</span><span class="sxs-lookup"><span data-stu-id="ee754-142">[localeInfo](../resources/localeinfo.md) object</span></span>
- <span data-ttu-id="ee754-143">Строка (для параметра **timeZone**).</span><span class="sxs-lookup"><span data-stu-id="ee754-143">string (for **timeZone**)</span></span>

## <a name="example"></a><span data-ttu-id="ee754-144">Пример</span><span class="sxs-lookup"><span data-stu-id="ee754-144">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="ee754-145">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="ee754-145">Request 1</span></span>
<span data-ttu-id="ee754-146">В первом примере показано, как получить все параметры почтового ящика пользователя, вошедшего в систему, в том числе параметры автоматических ответов, сведения о часовом поясе и параметры языка.</span><span class="sxs-lookup"><span data-stu-id="ee754-146">The first example gets all the mailbox settings of the signed-in user's mailbox, which include automatic replies settings, time zone, and language settings.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailboxSettings
```
##### <a name="response-1"></a><span data-ttu-id="ee754-147">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="ee754-147">Response 1</span></span>
<span data-ttu-id="ee754-p106">Отклик включает все параметры почтового ящика. Примечание. Показанный здесь объект отклика может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ee754-p106">The response includes all the mailbox settings. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    }
}
```

##### <a name="request-2"></a><span data-ttu-id="ee754-151">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="ee754-151">Request 2</span></span>
<span data-ttu-id="ee754-152">Во втором примере показано, как получить только параметры автоматических ответов почтового ящика пользователя, выполнившего вход в систему.</span><span class="sxs-lookup"><span data-stu-id="ee754-152">The second example gets specifically the automatic replies settings of the signed-in user's mailbox.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_2"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailboxSettings/automaticRepliesSetting
```
##### <a name="response-2"></a><span data-ttu-id="ee754-153">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="ee754-153">Response 2</span></span>
<span data-ttu-id="ee754-p107">Отклик включает только параметры автоматических ответов. Примечание. Показанный здесь объект отклика может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ee754-p107">The response includes only the automatic replies settings. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get mailbox settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->