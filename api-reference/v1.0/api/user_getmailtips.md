# <a name="user-getmailtips"></a><span data-ttu-id="76cba-101">user: getMailTips</span><span class="sxs-lookup"><span data-stu-id="76cba-101">user: getMailTips</span></span>

<span data-ttu-id="76cba-102">Получение подсказки (MailTips) для одного или нескольких получателей, доступных для вошедшего в систему [пользователя](../resources/user.md) .</span><span class="sxs-lookup"><span data-stu-id="76cba-102">Get the MailTips of one or more recipients as available to the signed-in user.</span></span>

<span data-ttu-id="76cba-103">Обратите внимание, что при помощи вызова `POST` действия `getMailTips` можно запросить возврат определенного типа подсказок (MailTips) для нескольких получателей за один раз.</span><span class="sxs-lookup"><span data-stu-id="76cba-103">Note that by making a `POST` call to the `getMailTips` action, you can request specific types of MailTips to be returned for more than one recipient at one time.</span></span> <span data-ttu-id="76cba-104">Запрошенные подсказки (MailTips) возвращаются в коллекцию [mailTips](../resources/mailtips.md).</span><span class="sxs-lookup"><span data-stu-id="76cba-104">The requested MailTips are returned in a [mailTips](../resources/mailtips.md) collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="76cba-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="76cba-105">Permissions</span></span>
<span data-ttu-id="76cba-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="76cba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="76cba-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="76cba-108">Permission type</span></span>      | <span data-ttu-id="76cba-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="76cba-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="76cba-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="76cba-110">Delegated (work or school account)</span></span> | <span data-ttu-id="76cba-111">Mail.Read Mail.Read.Shared</span><span class="sxs-lookup"><span data-stu-id="76cba-111">Mail.Read, Mail.Read.Shared</span></span>    |
|<span data-ttu-id="76cba-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="76cba-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76cba-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="76cba-113">Mail.Read</span></span>    |
|<span data-ttu-id="76cba-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="76cba-114">Application</span></span> | <span data-ttu-id="76cba-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="76cba-115">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="76cba-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="76cba-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMailTips
POST /users/{id|userPrincipalName}/getMailTips
```
## <a name="optional-query-parameters"></a><span data-ttu-id="76cba-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="76cba-117">Optional query parameters</span></span>
<span data-ttu-id="76cba-118">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="76cba-118">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="76cba-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="76cba-119">Request headers</span></span>
| <span data-ttu-id="76cba-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="76cba-120">Header</span></span>       | <span data-ttu-id="76cba-121">Значение</span><span class="sxs-lookup"><span data-stu-id="76cba-121">Value</span></span>|
|:-----------  |:------|
| <span data-ttu-id="76cba-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="76cba-122">Authorization</span></span> | <span data-ttu-id="76cba-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="76cba-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="76cba-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="76cba-125">Content-Type</span></span>  | <span data-ttu-id="76cba-126">application/json</span><span class="sxs-lookup"><span data-stu-id="76cba-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="76cba-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="76cba-127">Request body</span></span>
<span data-ttu-id="76cba-128">В тексте запроса укажите JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="76cba-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="76cba-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="76cba-129">Property</span></span>     | <span data-ttu-id="76cba-130">Тип</span><span class="sxs-lookup"><span data-stu-id="76cba-130">Type</span></span>   |<span data-ttu-id="76cba-131">Описание</span><span class="sxs-lookup"><span data-stu-id="76cba-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="76cba-132">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="76cba-132">EmailAddresses</span></span>|<span data-ttu-id="76cba-133">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="76cba-133">String collection</span></span>|<span data-ttu-id="76cba-134">Коллекция SMTP-адресов получателей для получения подсказок (MailTips).</span><span class="sxs-lookup"><span data-stu-id="76cba-134">A collection of SMTP addresses of recipients to get MailTips for.</span></span>|
|<span data-ttu-id="76cba-135">MailTipsOptions</span><span class="sxs-lookup"><span data-stu-id="76cba-135">MailTipsOptions</span></span>|<span data-ttu-id="76cba-136">String (строка)</span><span class="sxs-lookup"><span data-stu-id="76cba-136">String</span></span>|<span data-ttu-id="76cba-137">Перечисление флагов, которое представляет запрошенные подсказки.</span><span class="sxs-lookup"><span data-stu-id="76cba-137">A enumeration of flags that represents the requested mailtips.</span></span> <span data-ttu-id="76cba-138">Возможные значения: `automaticReplies`, `customMailTip`, `deliveryRestriction`, `externalMemberCount`, `mailboxFullStatus`, `maxMessageSize`, `moderationStatus`, `recipientScope`, `recipientSuggestions` и `totalMemberCount`.</span><span class="sxs-lookup"><span data-stu-id="76cba-138">Possible values are: `automaticReplies`, `customMailTip`, `deliveryRestriction`, `externalMemberCount`,`mailboxFullStatus`, `maxMessageSize`, `moderationStatus`, `recipientScope`, `recipientSuggestions`, `totalMemberCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="76cba-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="76cba-139">Response</span></span>

<span data-ttu-id="76cba-140">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [mailTips](../resources/mailtips.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="76cba-140">If successful, this method returns a `200 OK` response code and a collection of [macOSCompliancePolicy](../resources/mailtips.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="76cba-141">Пример</span><span class="sxs-lookup"><span data-stu-id="76cba-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="76cba-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="76cba-142">Request</span></span>
<span data-ttu-id="76cba-143">Следующий пример демонстрирует получение подсказок (MailTips) для указанных получателей, для любых параметров автоматического ответа и состояния переполненности почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="76cba-143">The following example gets MailTips for the specified recipients, for any automatic reply settings and mailbox full status.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_getmailtips"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/getMailTips
Content-Type: application/json

{
    "EmailAddresses": [
        "danas@contoso.onmicrosoft.com", 
        "fannyd@contoso.onmicrosoft.com"
    ],
    "MailTipsOptions": "automaticReplies, mailboxFullStatus"
}
```

##### <a name="response"></a><span data-ttu-id="76cba-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="76cba-144">Response</span></span>
<span data-ttu-id="76cba-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="76cba-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailTips",
  isCollection: true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.mailTips)",
    "value":[
        {
            "emailAddress":{
                "name":"",
                "address":"danas@contoso.onmicrosoft.com"
            },
            "automaticReplies":{
                "message":"<style type=\"text/css\" style=\"\">\r\n<!--\r\np\r\n\t{margin-top:0;\r\n\tmargin-bottom:0}\r\n-->\r\n</style>\r\n<div dir=\"ltr\">\r\n<div id=\"x_divtagdefaultwrapper\" style=\"font-size:12pt; color:#000000; background-color:#FFFFFF; font-family:Calibri,Arial,Helvetica,sans-serif\">\r\n<p>Hi, I am on vacation right now. I'll get back to you after I return.<br>\r\n</p>\r\n</div>\r\n</div>",
                "messageLanguage":{
                    "locale":"en-US",
                    "displayName":"English (United States)"
                },
                "scheduledStartTime": {
                    "dateTime": "2018-08-07T02:00:00.0000000",
                    "timeZone": "UTC"
                },
                "scheduledEndTime": {
                    "dateTime": "2018-08-09T02:00:00.0000000",
                    "timeZone": "UTC"
                }
            },
            "mailboxFull":false
        },
        {
            "emailAddress":{
                "name":"",
                "address":"fannyd@contoso.onmicrosoft.com"
            },
            "automaticReplies":{
                "message":""
            },
            "mailboxFull":false
        }
    ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: getMailTips",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
