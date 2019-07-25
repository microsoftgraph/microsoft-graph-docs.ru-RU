---
title: Получение параметров почтового ящика пользователя
description: 'Получение объекта mailboxSettings пользователя. Этот объект включает параметры автоматических ответов (автоматического уведомления пользователей при '
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: aed5f5e3ca32aeac0714416e173c45f5507ee80c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867700"
---
# <a name="get-user-mailbox-settings"></a><span data-ttu-id="427ac-104">Получение параметров почтового ящика пользователя</span><span class="sxs-lookup"><span data-stu-id="427ac-104">Get user mailbox settings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="427ac-105">Получение объекта [mailboxSettings](../resources/mailboxsettings.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="427ac-105">Get the user's [mailboxSettings](../resources/mailboxsettings.md).</span></span> <span data-ttu-id="427ac-106">Сюда входят параметры для автоматических ответов (уведомлять пользователей автоматически после получения их электронной почты), языковой стандарт (язык и страну или регион), часовой пояс и рабочие часы.</span><span class="sxs-lookup"><span data-stu-id="427ac-106">This includes settings for automatic replies (notify people automatically upon receipt of their email), locale (language and country/region), time zone, and working hours.</span></span>

<span data-ttu-id="427ac-107">Вы можете просмотреть все параметры почтового ящика или получить определенные параметры.</span><span class="sxs-lookup"><span data-stu-id="427ac-107">You can view all mailbox settings, or, get specific settings.</span></span>

<span data-ttu-id="427ac-108">Часовой пояс относится к предпочтительным параметрам, настраиваемым пользователями.</span><span class="sxs-lookup"><span data-stu-id="427ac-108">Time zone is one of the preferred settings a user can set up for the user's mailbox.</span></span> <span data-ttu-id="427ac-109">Пользователь выбирает его из поддерживаемых часовых [поясов](outlookuser-supportedtimezones.md) , настроенных администратором для сервера почтовых ящиков пользователя.</span><span class="sxs-lookup"><span data-stu-id="427ac-109">The user chooses it from the [supported time zones](outlookuser-supportedtimezones.md) that an administrator has set up for the user's mailbox server.</span></span> <span data-ttu-id="427ac-110">Администратор настраивает Часовые пояса в формате часового пояса Windows или в часовом [поясе IANA](https://www.iana.org/time-zones) (который также называется часовым поясом Олсона).</span><span class="sxs-lookup"><span data-stu-id="427ac-110">The administrator sets up time zones in the Windows time zone format or  [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="427ac-111">Формат Windows используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="427ac-111">The Windows format is the default.</span></span> 

<span data-ttu-id="427ac-112">Когда вы получаете предпочтительный часовой пояс пользователя, часовой пояс возвращается в том формате, который был настроен.</span><span class="sxs-lookup"><span data-stu-id="427ac-112">When you get a user's preferred time zone, the time zone is returned in the format that it was set up.</span></span> <span data-ttu-id="427ac-113">Чтобы задать определенный формат часового пояса (Windows или IANA), сначала [обновите предпочтительный часовой пояс в этом формате как параметр почтового ящика](user-update-mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="427ac-113">If you want that time zone to be in a specific format (Windows or IANA), you can first [update the preferred time zone in that format as a mailbox setting](user-update-mailboxsettings.md).</span></span> <span data-ttu-id="427ac-114">Затем вы сможете получить часовой пояс в этом формате.</span><span class="sxs-lookup"><span data-stu-id="427ac-114">Subsequently you will be able to get the time zone in that format.</span></span> <span data-ttu-id="427ac-115">Кроме того, вы можете управлять преобразованием форматов в своем приложении.</span><span class="sxs-lookup"><span data-stu-id="427ac-115">Alternatively, you can manage the format conversion separately in your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="427ac-116">Разрешения</span><span class="sxs-lookup"><span data-stu-id="427ac-116">Permissions</span></span>
<span data-ttu-id="427ac-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="427ac-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="427ac-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="427ac-119">Permission type</span></span>      | <span data-ttu-id="427ac-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="427ac-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="427ac-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="427ac-121">Delegated (work or school account)</span></span> | <span data-ttu-id="427ac-122">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="427ac-122">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="427ac-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="427ac-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="427ac-124">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="427ac-124">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="427ac-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="427ac-125">Application</span></span> | <span data-ttu-id="427ac-126">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="427ac-126">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="427ac-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="427ac-127">HTTP request</span></span>
<span data-ttu-id="427ac-128">Чтобы получить все параметры почтового ящика для пользователя, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="427ac-128">To get all the mailbox settings for a user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings
GET /users/{id|userPrincipalName}/mailboxSettings
```

<span data-ttu-id="427ac-129">Чтобы получить определенные параметры, можно использовать только параметры автоматических ответов, языковой стандарт, часовой пояс или рабочие часы.</span><span class="sxs-lookup"><span data-stu-id="427ac-129">To get specific settings - only the automatic replies settings, locale, time zone, or working hours:</span></span>
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
## <a name="optional-query-parameters"></a><span data-ttu-id="427ac-130">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="427ac-130">Optional query parameters</span></span>
<span data-ttu-id="427ac-131">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="427ac-131">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="427ac-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="427ac-132">Request headers</span></span>
| <span data-ttu-id="427ac-133">Имя</span><span class="sxs-lookup"><span data-stu-id="427ac-133">Name</span></span>       | <span data-ttu-id="427ac-134">Тип</span><span class="sxs-lookup"><span data-stu-id="427ac-134">Type</span></span> | <span data-ttu-id="427ac-135">Описание</span><span class="sxs-lookup"><span data-stu-id="427ac-135">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="427ac-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="427ac-136">Authorization</span></span>  | <span data-ttu-id="427ac-137">string</span><span class="sxs-lookup"><span data-stu-id="427ac-137">string</span></span>  | <span data-ttu-id="427ac-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="427ac-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="427ac-140">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="427ac-140">Request body</span></span>
<span data-ttu-id="427ac-141">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="427ac-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="427ac-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="427ac-142">Response</span></span>

<span data-ttu-id="427ac-143">При успешном выполнении этот метод возвращает код отклика `200 OK` и один из указанных ниже запрошенных объектов в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="427ac-143">If successful, this method returns a `200 OK` response code and one of the following requested objects in the response body:</span></span>

- <span data-ttu-id="427ac-144">Объект [mailboxSettings](../resources/mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="427ac-144">[mailboxSettings](../resources/mailboxsettings.md) object</span></span>
- <span data-ttu-id="427ac-145">Объект [automaticRepliesSetting](../resources/automaticrepliessetting.md).</span><span class="sxs-lookup"><span data-stu-id="427ac-145">[automaticRepliesSetting](../resources/automaticrepliessetting.md) object</span></span>
- <span data-ttu-id="427ac-146">Объект [localeInfo](../resources/localeinfo.md).</span><span class="sxs-lookup"><span data-stu-id="427ac-146">[localeInfo](../resources/localeinfo.md) object</span></span>
- <span data-ttu-id="427ac-147">Строка (для параметра **timeZone**).</span><span class="sxs-lookup"><span data-stu-id="427ac-147">string (for **timeZone**)</span></span>
- [<span data-ttu-id="427ac-148">workingHours</span><span class="sxs-lookup"><span data-stu-id="427ac-148">workingHours</span></span>](../resources/workinghours.md)

## <a name="example"></a><span data-ttu-id="427ac-149">Пример</span><span class="sxs-lookup"><span data-stu-id="427ac-149">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="427ac-150">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="427ac-150">Request 1</span></span>
<span data-ttu-id="427ac-151">В первом примере считываются все параметры часового пояса для почтового ящика вошедшего пользователя, в том числе параметры часового пояса, автоматических ответов, языкового стандарта (язык и страна или регион) и рабочего времени.</span><span class="sxs-lookup"><span data-stu-id="427ac-151">The first example gets all the mailbox settings of the signed-in user's mailbox, which include settings for time zone, automatic replies, locale (language and country/region), and working hours.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="427ac-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="427ac-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_1"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailboxSettings
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="427ac-153">C#</span><span class="sxs-lookup"><span data-stu-id="427ac-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailboxsettings-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="427ac-154">Javascript</span><span class="sxs-lookup"><span data-stu-id="427ac-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailboxsettings-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="427ac-155">Цель — C</span><span class="sxs-lookup"><span data-stu-id="427ac-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailboxsettings-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="427ac-156">Java</span><span class="sxs-lookup"><span data-stu-id="427ac-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailboxsettings-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-1"></a><span data-ttu-id="427ac-157">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="427ac-157">Response 1</span></span>
<span data-ttu-id="427ac-158">Ответ включает все параметры почтового ящика вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="427ac-158">The response includes all the mailbox settings of the signed-in user.</span></span> <span data-ttu-id="427ac-159">Примечание. Представленный здесь объект ответа может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="427ac-159">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="427ac-160">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="427ac-160">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxSettings"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/mailboxSettings",
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

##### <a name="request-2"></a><span data-ttu-id="427ac-161">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="427ac-161">Request 2</span></span>
<span data-ttu-id="427ac-162">Во втором примере показано, как получить только параметры автоматических ответов почтового ящика пользователя, выполнившего вход в систему.</span><span class="sxs-lookup"><span data-stu-id="427ac-162">The second example gets specifically the automatic replies settings of the signed-in user's mailbox.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="427ac-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="427ac-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_2"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailboxSettings/automaticRepliesSetting
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="427ac-164">C#</span><span class="sxs-lookup"><span data-stu-id="427ac-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailboxsettings-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="427ac-165">Javascript</span><span class="sxs-lookup"><span data-stu-id="427ac-165">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailboxsettings-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="427ac-166">Цель — C</span><span class="sxs-lookup"><span data-stu-id="427ac-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailboxsettings-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="427ac-167">Java</span><span class="sxs-lookup"><span data-stu-id="427ac-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailboxsettings-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-2"></a><span data-ttu-id="427ac-168">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="427ac-168">Response 2</span></span>
<span data-ttu-id="427ac-p108">Отклик включает только параметры автоматических ответов. Примечание. Показанный здесь объект отклика может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="427ac-p108">The response includes only the automatic replies settings. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.automaticRepliesSetting"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/mailboxSettings/automaticRepliesSetting",
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


##### <a name="request-3"></a><span data-ttu-id="427ac-172">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="427ac-172">Request 3</span></span>
<span data-ttu-id="427ac-173">В третьем примере показано, как получить только параметры рабочего времени для почтового ящика пользователя, выполнившего вход в систему.</span><span class="sxs-lookup"><span data-stu-id="427ac-173">The third example gets specifically the working hour settings of the signed-in user's mailbox.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_mailboxsettings_3"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailboxSettings/workingHours
```
##### <a name="response-3"></a><span data-ttu-id="427ac-174">Ответ 3</span><span class="sxs-lookup"><span data-stu-id="427ac-174">Response 3</span></span>
<span data-ttu-id="427ac-175">Ответ включает только параметры рабочего времени.</span><span class="sxs-lookup"><span data-stu-id="427ac-175">The response includes only the working hours settings.</span></span> <span data-ttu-id="427ac-176">Обратите внимание, что рабочее время пользователя относится к [пользовательскому часовому поясу](../resources/customtimezone.md).</span><span class="sxs-lookup"><span data-stu-id="427ac-176">Notice that the user's work hours are in a [custom time zone](../resources/customtimezone.md).</span></span> <span data-ttu-id="427ac-177">Примечание. Представленный здесь объект ответа может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="427ac-177">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="427ac-178">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="427ac-178">All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('94447c6e-ea4c-494c-a9ed-d905e366c5cb')/mailboxSettings/workingHours",
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
<!--
{
  "type": "#page.annotation",
  "description": "Get mailbox settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
