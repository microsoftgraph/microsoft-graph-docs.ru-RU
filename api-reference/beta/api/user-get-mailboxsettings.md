---
title: Получение параметров почтового ящика пользователя
description: 'Получите mailboxSettings пользователя. Это включает параметры для автоматических ответов (уведомление людей автоматически при '
ms.openlocfilehash: fae1bb16ec533abf7f29d0aadc0f66ba33f5ec25
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081284"
---
# <a name="get-user-mailbox-settings"></a><span data-ttu-id="52e76-104">Получение параметров почтового ящика пользователя</span><span class="sxs-lookup"><span data-stu-id="52e76-104">Get user mailbox settings</span></span>

> <span data-ttu-id="52e76-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="52e76-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="52e76-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52e76-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="52e76-107">Получите пользователя [mailboxSettings](../resources/mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="52e76-107">Get the user's [mailboxSettings](../resources/mailboxsettings.md).</span></span> <span data-ttu-id="52e76-108">Этот компонент включает параметры для автоматических ответов (уведомление людей автоматически при получении своей электронной почте), языковой стандарт (язык и Страна или регион), часовой пояс и рабочее время.</span><span class="sxs-lookup"><span data-stu-id="52e76-108">This includes settings for automatic replies (notify people automatically upon receipt of their email), locale (language and country/region), time zone, and working hours.</span></span>

<span data-ttu-id="52e76-109">Вы можете просмотреть все параметры почтового ящика или получить определенные параметры.</span><span class="sxs-lookup"><span data-stu-id="52e76-109">You can view all mailbox settings, or, get specific settings.</span></span>

<span data-ttu-id="52e76-110">Часовой пояс относится к предпочтительным параметрам, настраиваемым пользователями.</span><span class="sxs-lookup"><span data-stu-id="52e76-110">Time zone is one of the preferred settings a user can set up for the user's mailbox.</span></span> <span data-ttu-id="52e76-111">Пользователь выбирает его на [поддерживаемых часовых поясов](outlookuser-supportedtimezones.md) , которые настроены администратором для сервера почтовых ящиков пользователя.</span><span class="sxs-lookup"><span data-stu-id="52e76-111">The user chooses it from the [supported time zones](outlookuser-supportedtimezones.md) that an administrator has set up for the user's mailbox server.</span></span> <span data-ttu-id="52e76-112">Администратор настраивает часовые пояса в формате Windows часовой пояс или формат [назначенных номеров сертификации IANA (Internet) часового пояса](https://www.iana.org/time-zones) (также известной как Олсон часового пояса).</span><span class="sxs-lookup"><span data-stu-id="52e76-112">The administrator sets up time zones in the Windows time zone format or  [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="52e76-113">Формат Windows используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="52e76-113">The Windows format is the default.</span></span> 

<span data-ttu-id="52e76-114">Когда вы получаете предпочтительный часовой пояс пользователя, часовой пояс возвращается в том формате, который был настроен.</span><span class="sxs-lookup"><span data-stu-id="52e76-114">When you get a user's preferred time zone, the time zone is returned in the format that it was set up.</span></span> <span data-ttu-id="52e76-115">Чтобы задать определенный формат часового пояса (Windows или IANA), сначала [обновите предпочтительный часовой пояс в этом формате как параметр почтового ящика](user-update-mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="52e76-115">If you want that time zone to be in a specific format (Windows or IANA), you can first [update the preferred time zone in that format as a mailbox setting](user-update-mailboxsettings.md).</span></span> <span data-ttu-id="52e76-116">Затем вы сможете получить часовой пояс в этом формате.</span><span class="sxs-lookup"><span data-stu-id="52e76-116">Subsequently you will be able to get the time zone in that format.</span></span> <span data-ttu-id="52e76-117">Кроме того, вы можете управлять преобразованием форматов в своем приложении.</span><span class="sxs-lookup"><span data-stu-id="52e76-117">Alternatively, you can manage the format conversion separately in your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="52e76-118">Разрешения</span><span class="sxs-lookup"><span data-stu-id="52e76-118">Permissions</span></span>
<span data-ttu-id="52e76-p106">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52e76-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52e76-121">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="52e76-121">Permission type</span></span>      | <span data-ttu-id="52e76-122">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="52e76-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="52e76-123">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="52e76-123">Delegated (work or school account)</span></span> | <span data-ttu-id="52e76-124">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="52e76-124">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="52e76-125">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="52e76-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52e76-126">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="52e76-126">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="52e76-127">Для приложений</span><span class="sxs-lookup"><span data-stu-id="52e76-127">Application</span></span> | <span data-ttu-id="52e76-128">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="52e76-128">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="52e76-129">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="52e76-129">HTTP request</span></span>
<span data-ttu-id="52e76-130">Для получения всех параметров почтового ящика для пользователя:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="52e76-130">To get all the mailbox settings for a user: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/mailboxSettings
GET /users/{id|userPrincipalName}/mailboxSettings
```

<span data-ttu-id="52e76-131">Получение определенных параметров - только параметров автоматических ответов, языкового стандарта, часовой пояс или рабочее время:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="52e76-131">To get specific settings - only the automatic replies settings, locale, time zone, or working hours: <!-- { "blockType": "ignored" } --></span></span>
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
## <a name="optional-query-parameters"></a><span data-ttu-id="52e76-132">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="52e76-132">Optional query parameters</span></span>
<span data-ttu-id="52e76-133">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="52e76-133">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="52e76-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="52e76-134">Request headers</span></span>
| <span data-ttu-id="52e76-135">Имя</span><span class="sxs-lookup"><span data-stu-id="52e76-135">Name</span></span>       | <span data-ttu-id="52e76-136">Тип</span><span class="sxs-lookup"><span data-stu-id="52e76-136">Type</span></span> | <span data-ttu-id="52e76-137">Описание</span><span class="sxs-lookup"><span data-stu-id="52e76-137">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="52e76-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="52e76-138">Authorization</span></span>  | <span data-ttu-id="52e76-139">string</span><span class="sxs-lookup"><span data-stu-id="52e76-139">string</span></span>  | <span data-ttu-id="52e76-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="52e76-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="52e76-142">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="52e76-142">Request body</span></span>
<span data-ttu-id="52e76-143">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="52e76-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="52e76-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="52e76-144">Response</span></span>

<span data-ttu-id="52e76-145">При успешном выполнении этот метод возвращает код отклика `200 OK` и один из указанных ниже запрошенных объектов в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="52e76-145">If successful, this method returns a `200 OK` response code and one of the following requested objects in the response body:</span></span>

- <span data-ttu-id="52e76-146">Объект [mailboxSettings](../resources/mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="52e76-146">[mailboxSettings](../resources/mailboxsettings.md) object</span></span>
- <span data-ttu-id="52e76-147">Объект [automaticRepliesSetting](../resources/automaticrepliessetting.md).</span><span class="sxs-lookup"><span data-stu-id="52e76-147">[automaticRepliesSetting](../resources/automaticrepliessetting.md) object</span></span>
- <span data-ttu-id="52e76-148">Объект [localeInfo](../resources/localeinfo.md).</span><span class="sxs-lookup"><span data-stu-id="52e76-148">[localeInfo](../resources/localeinfo.md) object</span></span>
- <span data-ttu-id="52e76-149">Строка (для параметра **timeZone**).</span><span class="sxs-lookup"><span data-stu-id="52e76-149">string (for **timeZone**)</span></span>
- [<span data-ttu-id="52e76-150">workingHours</span><span class="sxs-lookup"><span data-stu-id="52e76-150">workingHours</span></span>](../resources/workinghours.md)

## <a name="example"></a><span data-ttu-id="52e76-151">Пример</span><span class="sxs-lookup"><span data-stu-id="52e76-151">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="52e76-152">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="52e76-152">Request 1</span></span>
<span data-ttu-id="52e76-153">В первом примере считываются все параметры часового пояса для почтового ящика вошедшего пользователя, в том числе параметры часового пояса, автоматических ответов, языкового стандарта (язык и страна или регион) и рабочего времени.</span><span class="sxs-lookup"><span data-stu-id="52e76-153">The first example gets all the mailbox settings of the signed-in user's mailbox, which include settings for time zone, automatic replies, locale (language and country/region), and working hours.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_1"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailboxSettings
```
##### <a name="response-1"></a><span data-ttu-id="52e76-154">Ответ 1</span><span class="sxs-lookup"><span data-stu-id="52e76-154">Response 1</span></span>
<span data-ttu-id="52e76-155">Ответ содержит все параметры почтового ящика пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="52e76-155">The response includes all the mailbox settings of the signed-in user.</span></span> <span data-ttu-id="52e76-156">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="52e76-156">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="52e76-157">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="52e76-157">All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request-2"></a><span data-ttu-id="52e76-158">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="52e76-158">Request 2</span></span>
<span data-ttu-id="52e76-159">Во втором примере показано, как получить только параметры автоматических ответов почтового ящика пользователя, выполнившего вход в систему.</span><span class="sxs-lookup"><span data-stu-id="52e76-159">The second example gets specifically the automatic replies settings of the signed-in user's mailbox.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_2"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailboxSettings/automaticRepliesSetting
```
##### <a name="response-2"></a><span data-ttu-id="52e76-160">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="52e76-160">Response 2</span></span>
<span data-ttu-id="52e76-p109">Отклик включает только параметры автоматических ответов. Примечание. Показанный здесь объект отклика может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="52e76-p109">The response includes only the automatic replies settings. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


##### <a name="request-3"></a><span data-ttu-id="52e76-164">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="52e76-164">Request 3</span></span>
<span data-ttu-id="52e76-165">В третьем примере показано, как получить только параметры рабочего времени для почтового ящика пользователя, выполнившего вход в систему.</span><span class="sxs-lookup"><span data-stu-id="52e76-165">The third example gets specifically the working hour settings of the signed-in user's mailbox.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_mailboxsettings_3"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailboxSettings/workingHours
```
##### <a name="response-3"></a><span data-ttu-id="52e76-166">Ответ 3</span><span class="sxs-lookup"><span data-stu-id="52e76-166">Response 3</span></span>
<span data-ttu-id="52e76-167">Ответ включает только параметры рабочего времени.</span><span class="sxs-lookup"><span data-stu-id="52e76-167">The response includes only the working hours settings.</span></span> <span data-ttu-id="52e76-168">Обратите внимание, что рабочее время пользователя относится к [пользовательскому часовому поясу](../resources/customtimezone.md).</span><span class="sxs-lookup"><span data-stu-id="52e76-168">Notice that the user's work hours are in a [custom time zone](../resources/customtimezone.md).</span></span> <span data-ttu-id="52e76-169">Примечание. Представленный здесь объект ответа может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="52e76-169">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="52e76-170">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="52e76-170">All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get mailbox settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
