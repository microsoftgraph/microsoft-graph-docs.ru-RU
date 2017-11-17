# <a name="update-user-mailbox-settings"></a><span data-ttu-id="432d6-101">Обновление параметров почтового ящика пользователя</span><span class="sxs-lookup"><span data-stu-id="432d6-101">Update user mailbox settings</span></span>

<span data-ttu-id="432d6-p101">Обновление одного или нескольких параметров почтового ящика пользователя. Этот объект включает параметры автоматических ответов (автоматического уведомления пользователей при получении их почты), языкового стандарта или часового пояса.</span><span class="sxs-lookup"><span data-stu-id="432d6-p101">Update one or more settings for the user's mailbox. This includes settings for automatic replies (notify people automatically upon receipt of their email), locale, or time zone.</span></span>

<span data-ttu-id="432d6-104">Вы можете включить, настроить или отключить один или несколько этих параметров в составе объекта [mailboxSettings](../resources/mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="432d6-104">You can enable, configure, or disable one or more of these settings as part of [mailboxSettings](../resources/mailboxsettings.md).</span></span>

<span data-ttu-id="432d6-105">**Примечание.** Невозможно создать или удалить какие-либо параметры почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="432d6-105">**Note** You cannot create or delete any mailbox settings.</span></span>

## <a name="permissions"></a><span data-ttu-id="432d6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="432d6-106">Permissions</span></span>
<span data-ttu-id="432d6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="432d6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="432d6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="432d6-109">Permission type</span></span>      | <span data-ttu-id="432d6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="432d6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="432d6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="432d6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="432d6-112">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="432d6-112">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="432d6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="432d6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="432d6-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="432d6-114">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="432d6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="432d6-115">Application</span></span> | <span data-ttu-id="432d6-116">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="432d6-116">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="432d6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="432d6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailboxSettings
PATCH /users/{id|userPrincipalName}/mailboxSettings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="432d6-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="432d6-118">Optional query parameters</span></span>
<span data-ttu-id="432d6-119">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="432d6-119">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="432d6-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="432d6-120">Request headers</span></span>
| <span data-ttu-id="432d6-121">Имя</span><span class="sxs-lookup"><span data-stu-id="432d6-121">Name</span></span>       | <span data-ttu-id="432d6-122">Тип</span><span class="sxs-lookup"><span data-stu-id="432d6-122">Type</span></span> | <span data-ttu-id="432d6-123">Описание</span><span class="sxs-lookup"><span data-stu-id="432d6-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="432d6-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="432d6-124">Authorization</span></span>  | <span data-ttu-id="432d6-125">string</span><span class="sxs-lookup"><span data-stu-id="432d6-125">string</span></span>  | <span data-ttu-id="432d6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="432d6-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="432d6-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="432d6-128">Request body</span></span>
<span data-ttu-id="432d6-p104">В тексте запроса укажите значения для соответствующих свойств, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом изменений других значений свойств. Чтобы обеспечить максимальную производительность, не включайте существующие значения, которые не изменились, в запрос. Ниже перечислены свойства, значения которых можно записать или обновить.</span><span class="sxs-lookup"><span data-stu-id="432d6-p104">In the request body, supply the values for the relevant properties that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. The following are the writable/updatable properties:</span></span>

| <span data-ttu-id="432d6-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="432d6-133">Property</span></span>     | <span data-ttu-id="432d6-134">Тип</span><span class="sxs-lookup"><span data-stu-id="432d6-134">Type</span></span>   |<span data-ttu-id="432d6-135">Описание</span><span class="sxs-lookup"><span data-stu-id="432d6-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="432d6-136">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="432d6-136">automaticRepliesSetting</span></span>|[<span data-ttu-id="432d6-137">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="432d6-137">automaticRepliesSetting</span></span>](../resources/automaticrepliessetting.md)|<span data-ttu-id="432d6-138">Параметры конфигурации для автоматического уведомления отправителя о входящем письме с помощью сообщения от пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="432d6-138">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span>|
|<span data-ttu-id="432d6-139">language</span><span class="sxs-lookup"><span data-stu-id="432d6-139">language</span></span>|[<span data-ttu-id="432d6-140">localeInfo</span><span class="sxs-lookup"><span data-stu-id="432d6-140">localeInfo</span></span>](../resources/localeinfo.md)|<span data-ttu-id="432d6-141">Сведения о языковом стандарте пользователя, в том числе о предпочитаемом языке и стране или регионе.</span><span class="sxs-lookup"><span data-stu-id="432d6-141">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="432d6-142">timeZone</span><span class="sxs-lookup"><span data-stu-id="432d6-142">timeZone</span></span>|<span data-ttu-id="432d6-143">string</span><span class="sxs-lookup"><span data-stu-id="432d6-143">string</span></span>|<span data-ttu-id="432d6-144">Часовой пояс, используемый по умолчанию, для почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="432d6-144">The default time zone for the user's mailbox.</span></span>|

## <a name="response"></a><span data-ttu-id="432d6-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="432d6-145">Response</span></span>

<span data-ttu-id="432d6-146">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [mailboxSettings](../resources/mailboxSettings.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="432d6-146">If successful, this method returns a `200 OK` response code and [mailboxSettings](../resources/mailboxSettings.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="432d6-147">Пример</span><span class="sxs-lookup"><span data-stu-id="432d6-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="432d6-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="432d6-148">Request</span></span>
<span data-ttu-id="432d6-149">В примере ниже показано, как включить автоматические ответы для диапазона дат, настроив для свойства **automaticRepliesSetting** следующие свойства: **status**, **scheduledStartDateTime** и **scheduledEndDateTime**.</span><span class="sxs-lookup"><span data-stu-id="432d6-149">The following example enables automatic replies for a date range, by setting the following properties of the **automaticRepliesSetting** property: **status**, **scheduledStartDateTime** and **scheduledEndDateTime**.</span></span>

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
##### <a name="response"></a><span data-ttu-id="432d6-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="432d6-150">Response</span></span>
<span data-ttu-id="432d6-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="432d6-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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