# <a name="get-user-mailbox-settings"></a><span data-ttu-id="16d6b-101">Получение параметров почтового ящика пользователя</span><span class="sxs-lookup"><span data-stu-id="16d6b-101">Get user mailbox settings</span></span>

<span data-ttu-id="16d6b-p101">Получение объекта [mailboxSettings](../resources/mailboxsettings.md) пользователя. Этот объект включает параметры автоматических ответов (автоматического уведомления пользователей при получении их почты), языкового стандарта (сведения о языке и стране или регионе) и часового пояса.</span><span class="sxs-lookup"><span data-stu-id="16d6b-p101">Get the user's [mailboxSettings](../resources/mailboxsettings.md). This includes settings for automatic replies (notify people automatically upon receipt of their email), locale (language and country/region), and time zone.</span></span>

<span data-ttu-id="16d6b-104">Вы можете просмотреть все параметры почтового ящика или получить определенные параметры.</span><span class="sxs-lookup"><span data-stu-id="16d6b-104">You can view all mailbox settings, or, get specific settings.</span></span>

## <a name="permissions"></a><span data-ttu-id="16d6b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="16d6b-105">Permissions</span></span>
<span data-ttu-id="16d6b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="16d6b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="16d6b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16d6b-108">Permission type</span></span>      | <span data-ttu-id="16d6b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="16d6b-109">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="16d6b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16d6b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="16d6b-111">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="16d6b-111">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    | 
|<span data-ttu-id="16d6b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16d6b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16d6b-113">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="16d6b-113">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    | 
|<span data-ttu-id="16d6b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="16d6b-114">Application</span></span> | <span data-ttu-id="16d6b-115">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="16d6b-115">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="16d6b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16d6b-116">HTTP request</span></span>
<span data-ttu-id="16d6b-117">Чтобы получить все параметры почтового ящика, включающие параметры автоматических ответов, используйте указанные ниже команды.</span><span class="sxs-lookup"><span data-stu-id="16d6b-117">To get all mailbox settings which include automatic replies settings:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings
GET /users/{id|userPrincipalName}/mailboxSettings
```

<span data-ttu-id="16d6b-118">Чтобы получить определенные параметры, например только параметры автоматических ответов, сведения о языковом стандарте и часовом поясе, выполните указанные ниже команды.</span><span class="sxs-lookup"><span data-stu-id="16d6b-118">To get specific settings - for example, only the automatic replies settings, locale, or time zone:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings/automaticRepliesSetting
GET /users/{id|userPrincipalName}/mailboxSettings/automaticRepliesSetting

GET /me/mailboxSettings/language
GET /users/{id|userPrincipalName}/mailboxSettings/language

GET /me/mailboxSettings/timeZone
GET /users/{id|userPrincipalName}/mailboxSettings/timeZone
```
## <a name="optional-query-parameters"></a><span data-ttu-id="16d6b-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="16d6b-119">Optional query parameters</span></span>
<span data-ttu-id="16d6b-120">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="16d6b-120">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="16d6b-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="16d6b-121">Request headers</span></span>
| <span data-ttu-id="16d6b-122">Имя</span><span class="sxs-lookup"><span data-stu-id="16d6b-122">Name</span></span>       | <span data-ttu-id="16d6b-123">Тип</span><span class="sxs-lookup"><span data-stu-id="16d6b-123">Type</span></span> | <span data-ttu-id="16d6b-124">Описание</span><span class="sxs-lookup"><span data-stu-id="16d6b-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="16d6b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="16d6b-125">Authorization</span></span>  | <span data-ttu-id="16d6b-126">string</span><span class="sxs-lookup"><span data-stu-id="16d6b-126">string</span></span>  | <span data-ttu-id="16d6b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="16d6b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="16d6b-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="16d6b-129">Request body</span></span>
<span data-ttu-id="16d6b-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="16d6b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16d6b-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="16d6b-131">Response</span></span>

<span data-ttu-id="16d6b-132">При успешном выполнении этот метод возвращает код отклика `200 OK` и один из указанных ниже запрошенных объектов в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="16d6b-132">If successful, this method returns a `200 OK` response code and one of the following requested objects in the response body:</span></span>

- <span data-ttu-id="16d6b-133">Объект [mailboxSettings](../resources/mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="16d6b-133">[mailboxSettings](../resources/mailboxsettings.md) object</span></span>
- <span data-ttu-id="16d6b-134">Объект [automaticRepliesSetting](../resources/automaticRepliesSetting.md).</span><span class="sxs-lookup"><span data-stu-id="16d6b-134">[automaticRepliesSetting](../resources/automaticRepliesSetting.md) object</span></span>
- <span data-ttu-id="16d6b-135">Объект [localeInfo](../resources/localeinfo.md).</span><span class="sxs-lookup"><span data-stu-id="16d6b-135">[localeInfo](../resources/localeinfo.md) object</span></span>
- <span data-ttu-id="16d6b-136">Строка (для параметра **timeZone**).</span><span class="sxs-lookup"><span data-stu-id="16d6b-136">string (for **timeZone**)</span></span>

## <a name="example"></a><span data-ttu-id="16d6b-137">Пример</span><span class="sxs-lookup"><span data-stu-id="16d6b-137">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="16d6b-138">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="16d6b-138">Request 1</span></span>
<span data-ttu-id="16d6b-139">В первом примере показано, как получить все параметры почтового ящика пользователя, вошедшего в систему, в том числе параметры автоматических ответов, сведения о часовом поясе и параметры языка.</span><span class="sxs-lookup"><span data-stu-id="16d6b-139">The first example gets all the mailbox settings of the signed-in user's mailbox, which include automatic replies settings, time zone, and language settings.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailboxSettings
```
##### <a name="response-1"></a><span data-ttu-id="16d6b-140">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="16d6b-140">Response 1</span></span>
<span data-ttu-id="16d6b-p104">Отклик включает все параметры почтового ящика. Примечание. Показанный здесь объект отклика может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="16d6b-p104">The response includes all the mailbox settings. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request-2"></a><span data-ttu-id="16d6b-144">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="16d6b-144">Request 2</span></span>
<span data-ttu-id="16d6b-145">Во втором примере показано, как получить только параметры автоматических ответов почтового ящика пользователя, выполнившего вход в систему.</span><span class="sxs-lookup"><span data-stu-id="16d6b-145">The second example gets specifically the automatic replies settings of the signed-in user's mailbox.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_2"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailboxSettings/automaticRepliesSetting
```
##### <a name="response-2"></a><span data-ttu-id="16d6b-146">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="16d6b-146">Response 2</span></span>
<span data-ttu-id="16d6b-p105">Отклик включает только параметры автоматических ответов. Примечание. Показанный здесь объект отклика может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="16d6b-p105">The response includes only the automatic replies settings. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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