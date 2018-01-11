# <a name="update-user-mailbox-settings"></a><span data-ttu-id="0e497-101">Обновление параметров почтового ящика пользователя</span><span class="sxs-lookup"><span data-stu-id="0e497-101">Update user mailbox settings</span></span>

<span data-ttu-id="0e497-p101">Обновление одного или нескольких параметров почтового ящика пользователя. Этот объект включает параметры автоматических ответов (автоматического уведомления пользователей при получении их почты), языкового стандарта или часового пояса.</span><span class="sxs-lookup"><span data-stu-id="0e497-p101">Update one or more settings for the user's mailbox. This includes settings for automatic replies (notify people automatically upon receipt of their email), locale, or time zone.</span></span>

<span data-ttu-id="0e497-104">Вы можете включить, настроить или отключить один или несколько этих параметров в составе объекта [mailboxSettings](../resources/mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="0e497-104">You can enable, configure, or disable one or more of these settings as part of [mailboxSettings](../resources/mailboxsettings.md).</span></span>

<span data-ttu-id="0e497-105">**Примечание.** Невозможно создать или удалить какие-либо параметры почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="0e497-105">**Note** You cannot create or delete any mailbox settings.</span></span>

<span data-ttu-id="0e497-106">Обновляя предпочтительный часовой пояс для пользователя, можете указать его в формате Windows или [часового пояса IANA]((http://www.iana.org/time-zones)) (также известен как часовой пояс Олсона).</span><span class="sxs-lookup"><span data-stu-id="0e497-106">When you update the preferred time zone for a user, you can specify it in the Windows or  [Internet Assigned Numbers Authority (IANA) time zone]((http://www.iana.org/time-zones)) (also known as Olson time zone) format.</span></span>

## <a name="permissions"></a><span data-ttu-id="0e497-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0e497-107">Permissions</span></span>
<span data-ttu-id="0e497-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0e497-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0e497-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0e497-110">Permission type</span></span>      | <span data-ttu-id="0e497-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0e497-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0e497-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0e497-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0e497-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0e497-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="0e497-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0e497-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e497-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0e497-115">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="0e497-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0e497-116">Application</span></span> | <span data-ttu-id="0e497-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0e497-117">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0e497-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0e497-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailboxSettings
PATCH /users/{id|userPrincipalName}/mailboxSettings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0e497-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0e497-119">Optional query parameters</span></span>
<span data-ttu-id="0e497-120">Этот метод поддерживает [параметры запросов OData]((http://developer.microsoft.com/ru-RU/graph/docs/overview/query_parameters)) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0e497-120">This method supports the [OData Query Parameters]((http://developer.microsoft.com/ru-RU/graph/docs/overview/query_parameters)) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="0e497-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0e497-121">Request headers</span></span>
| <span data-ttu-id="0e497-122">Имя</span><span class="sxs-lookup"><span data-stu-id="0e497-122">Name</span></span>       | <span data-ttu-id="0e497-123">Тип</span><span class="sxs-lookup"><span data-stu-id="0e497-123">Type</span></span> | <span data-ttu-id="0e497-124">Описание</span><span class="sxs-lookup"><span data-stu-id="0e497-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0e497-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e497-125">Authorization</span></span>  | <span data-ttu-id="0e497-126">string</span><span class="sxs-lookup"><span data-stu-id="0e497-126">string</span></span>  | <span data-ttu-id="0e497-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0e497-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0e497-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0e497-129">Request body</span></span>
<span data-ttu-id="0e497-p104">В тексте запроса укажите значения для соответствующих свойств, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом изменений других значений свойств. Чтобы обеспечить максимальную производительность, не включайте существующие значения, которые не изменились, в запрос. Ниже перечислены свойства, значения которых можно записать или обновить.</span><span class="sxs-lookup"><span data-stu-id="0e497-p104">In the request body, supply the values for the relevant properties that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. The following are the writable/updatable properties:</span></span>

| <span data-ttu-id="0e497-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="0e497-134">Property</span></span>     | <span data-ttu-id="0e497-135">Тип</span><span class="sxs-lookup"><span data-stu-id="0e497-135">Type</span></span>   |<span data-ttu-id="0e497-136">Описание</span><span class="sxs-lookup"><span data-stu-id="0e497-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0e497-137">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="0e497-137">automaticRepliesSetting</span></span>|[<span data-ttu-id="0e497-138">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="0e497-138">automaticRepliesSetting</span></span>](../resources/automaticrepliessetting.md)|<span data-ttu-id="0e497-139">Параметры конфигурации для автоматического уведомления отправителя о входящем письме с помощью сообщения от пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="0e497-139">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span>|
|<span data-ttu-id="0e497-140">language</span><span class="sxs-lookup"><span data-stu-id="0e497-140">language</span></span>|[<span data-ttu-id="0e497-141">localeInfo</span><span class="sxs-lookup"><span data-stu-id="0e497-141">localeInfo</span></span>](../resources/localeinfo.md)|<span data-ttu-id="0e497-142">Сведения о языковом стандарте пользователя, в том числе о предпочитаемом языке и стране или регионе.</span><span class="sxs-lookup"><span data-stu-id="0e497-142">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="0e497-143">timeZone</span><span class="sxs-lookup"><span data-stu-id="0e497-143">timeZone</span></span>|<span data-ttu-id="0e497-144">string</span><span class="sxs-lookup"><span data-stu-id="0e497-144">string</span></span>|<span data-ttu-id="0e497-145">Часовой пояс, используемый по умолчанию, для почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="0e497-145">The default time zone for the user's mailbox.</span></span>|

## <a name="response"></a><span data-ttu-id="0e497-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e497-146">Response</span></span>

<span data-ttu-id="0e497-147">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [mailboxSettings](../resources/mailboxSettings.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0e497-147">If successful, this method returns a `200 OK` response code and [mailboxSettings](../resources/mailboxSettings.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0e497-148">Пример</span><span class="sxs-lookup"><span data-stu-id="0e497-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0e497-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="0e497-149">Request</span></span>
<span data-ttu-id="0e497-150">В примере ниже показано, как включить автоматические ответы для диапазона дат, настроив для свойства **automaticRepliesSetting** следующие свойства: **status**, **scheduledStartDateTime** и **scheduledEndDateTime**.</span><span class="sxs-lookup"><span data-stu-id="0e497-150">The following example enables automatic replies for a date range, by setting the following properties of the **automaticRepliesSetting** property: **status**, **scheduledStartDateTime** and **scheduledEndDateTime**.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_mailboxsettings"
}-->
```http
PATCH https://graph.microsoft.com/api/v1.0/me/mailboxSettings
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/api/v1.0/$metadata#Me/mailboxSettings",
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
##### <a name="response"></a><span data-ttu-id="0e497-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e497-151">Response</span></span>
<span data-ttu-id="0e497-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0e497-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxSettings"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/api/v1.0/$metadata#Me/mailboxSettings",
    "automaticRepliesSetting": {
        "status": "scheduled",
        "externalAudience": "none",
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
    },
    "timeZone":"UTC",
    "language":{
      "locale":"en-US",
      "displayName":"English (United States)"
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
  "tocPath": ""
}-->