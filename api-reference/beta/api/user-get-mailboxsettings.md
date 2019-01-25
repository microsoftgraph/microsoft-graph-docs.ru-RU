---
title: Получение параметров почтового ящика пользователя
description: 'Получите mailboxSettings пользователя. Это включает параметры для автоматических ответов (уведомление людей автоматически при '
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 569a891e51d09c03467108c0a7ed012e04ba6352
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510248"
---
# <a name="get-user-mailbox-settings"></a><span data-ttu-id="3da51-104">Получение параметров почтового ящика пользователя</span><span class="sxs-lookup"><span data-stu-id="3da51-104">Get user mailbox settings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3da51-105">Получите пользователя [mailboxSettings](../resources/mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="3da51-105">Get the user's [mailboxSettings](../resources/mailboxsettings.md).</span></span> <span data-ttu-id="3da51-106">Этот компонент включает параметры для автоматических ответов (уведомление людей автоматически при получении своей электронной почте), языковой стандарт (язык и Страна или регион), часовой пояс и рабочее время.</span><span class="sxs-lookup"><span data-stu-id="3da51-106">This includes settings for automatic replies (notify people automatically upon receipt of their email), locale (language and country/region), time zone, and working hours.</span></span>

<span data-ttu-id="3da51-107">Вы можете просмотреть все параметры почтового ящика или получить определенные параметры.</span><span class="sxs-lookup"><span data-stu-id="3da51-107">You can view all mailbox settings, or, get specific settings.</span></span>

<span data-ttu-id="3da51-108">Часовой пояс относится к предпочтительным параметрам, настраиваемым пользователями.</span><span class="sxs-lookup"><span data-stu-id="3da51-108">Time zone is one of the preferred settings a user can set up for the user's mailbox.</span></span> <span data-ttu-id="3da51-109">Пользователь выбирает его на [поддерживаемых часовых поясов](outlookuser-supportedtimezones.md) , которые настроены администратором для сервера почтовых ящиков пользователя.</span><span class="sxs-lookup"><span data-stu-id="3da51-109">The user chooses it from the [supported time zones](outlookuser-supportedtimezones.md) that an administrator has set up for the user's mailbox server.</span></span> <span data-ttu-id="3da51-110">Администратор настраивает часовые пояса в формате Windows часовой пояс или формат [назначенных номеров сертификации IANA (Internet) часового пояса](https://www.iana.org/time-zones) (также известной как Олсон часового пояса).</span><span class="sxs-lookup"><span data-stu-id="3da51-110">The administrator sets up time zones in the Windows time zone format or  [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="3da51-111">Формат Windows используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="3da51-111">The Windows format is the default.</span></span> 

<span data-ttu-id="3da51-112">Когда вы получаете предпочтительный часовой пояс пользователя, часовой пояс возвращается в том формате, который был настроен.</span><span class="sxs-lookup"><span data-stu-id="3da51-112">When you get a user's preferred time zone, the time zone is returned in the format that it was set up.</span></span> <span data-ttu-id="3da51-113">Чтобы задать определенный формат часового пояса (Windows или IANA), сначала [обновите предпочтительный часовой пояс в этом формате как параметр почтового ящика](user-update-mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="3da51-113">If you want that time zone to be in a specific format (Windows or IANA), you can first [update the preferred time zone in that format as a mailbox setting](user-update-mailboxsettings.md).</span></span> <span data-ttu-id="3da51-114">Затем вы сможете получить часовой пояс в этом формате.</span><span class="sxs-lookup"><span data-stu-id="3da51-114">Subsequently you will be able to get the time zone in that format.</span></span> <span data-ttu-id="3da51-115">Кроме того, вы можете управлять преобразованием форматов в своем приложении.</span><span class="sxs-lookup"><span data-stu-id="3da51-115">Alternatively, you can manage the format conversion separately in your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="3da51-116">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3da51-116">Permissions</span></span>
<span data-ttu-id="3da51-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3da51-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3da51-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3da51-119">Permission type</span></span>      | <span data-ttu-id="3da51-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3da51-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3da51-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3da51-121">Delegated (work or school account)</span></span> | <span data-ttu-id="3da51-122">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3da51-122">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="3da51-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3da51-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3da51-124">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3da51-124">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="3da51-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3da51-125">Application</span></span> | <span data-ttu-id="3da51-126">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3da51-126">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3da51-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3da51-127">HTTP request</span></span>
<span data-ttu-id="3da51-128">Для получения всех параметров почтового ящика для пользователя:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="3da51-128">To get all the mailbox settings for a user: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/mailboxSettings
GET /users/{id|userPrincipalName}/mailboxSettings
```

<span data-ttu-id="3da51-129">Получение определенных параметров - только параметров автоматических ответов, языкового стандарта, часовой пояс или рабочее время:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="3da51-129">To get specific settings - only the automatic replies settings, locale, time zone, or working hours: <!-- { "blockType": "ignored" } --></span></span>
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
## <a name="optional-query-parameters"></a><span data-ttu-id="3da51-130">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3da51-130">Optional query parameters</span></span>
<span data-ttu-id="3da51-131">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3da51-131">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3da51-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3da51-132">Request headers</span></span>
| <span data-ttu-id="3da51-133">Имя</span><span class="sxs-lookup"><span data-stu-id="3da51-133">Name</span></span>       | <span data-ttu-id="3da51-134">Тип</span><span class="sxs-lookup"><span data-stu-id="3da51-134">Type</span></span> | <span data-ttu-id="3da51-135">Описание</span><span class="sxs-lookup"><span data-stu-id="3da51-135">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3da51-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="3da51-136">Authorization</span></span>  | <span data-ttu-id="3da51-137">string</span><span class="sxs-lookup"><span data-stu-id="3da51-137">string</span></span>  | <span data-ttu-id="3da51-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3da51-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3da51-140">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3da51-140">Request body</span></span>
<span data-ttu-id="3da51-141">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3da51-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3da51-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="3da51-142">Response</span></span>

<span data-ttu-id="3da51-143">При успешном выполнении этот метод возвращает код отклика `200 OK` и один из указанных ниже запрошенных объектов в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3da51-143">If successful, this method returns a `200 OK` response code and one of the following requested objects in the response body:</span></span>

- <span data-ttu-id="3da51-144">Объект [mailboxSettings](../resources/mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="3da51-144">[mailboxSettings](../resources/mailboxsettings.md) object</span></span>
- <span data-ttu-id="3da51-145">Объект [automaticRepliesSetting](../resources/automaticrepliessetting.md).</span><span class="sxs-lookup"><span data-stu-id="3da51-145">[automaticRepliesSetting](../resources/automaticrepliessetting.md) object</span></span>
- <span data-ttu-id="3da51-146">Объект [localeInfo](../resources/localeinfo.md).</span><span class="sxs-lookup"><span data-stu-id="3da51-146">[localeInfo](../resources/localeinfo.md) object</span></span>
- <span data-ttu-id="3da51-147">Строка (для параметра **timeZone**).</span><span class="sxs-lookup"><span data-stu-id="3da51-147">string (for **timeZone**)</span></span>
- [<span data-ttu-id="3da51-148">workingHours</span><span class="sxs-lookup"><span data-stu-id="3da51-148">workingHours</span></span>](../resources/workinghours.md)

## <a name="example"></a><span data-ttu-id="3da51-149">Пример</span><span class="sxs-lookup"><span data-stu-id="3da51-149">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="3da51-150">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="3da51-150">Request 1</span></span>
<span data-ttu-id="3da51-151">В первом примере считываются все параметры часового пояса для почтового ящика вошедшего пользователя, в том числе параметры часового пояса, автоматических ответов, языкового стандарта (язык и страна или регион) и рабочего времени.</span><span class="sxs-lookup"><span data-stu-id="3da51-151">The first example gets all the mailbox settings of the signed-in user's mailbox, which include settings for time zone, automatic replies, locale (language and country/region), and working hours.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_1"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailboxSettings
```
##### <a name="response-1"></a><span data-ttu-id="3da51-152">Ответ 1</span><span class="sxs-lookup"><span data-stu-id="3da51-152">Response 1</span></span>
<span data-ttu-id="3da51-153">Ответ содержит все параметры почтового ящика пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="3da51-153">The response includes all the mailbox settings of the signed-in user.</span></span> <span data-ttu-id="3da51-154">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="3da51-154">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3da51-155">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3da51-155">All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request-2"></a><span data-ttu-id="3da51-156">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="3da51-156">Request 2</span></span>
<span data-ttu-id="3da51-157">Во втором примере показано, как получить только параметры автоматических ответов почтового ящика пользователя, выполнившего вход в систему.</span><span class="sxs-lookup"><span data-stu-id="3da51-157">The second example gets specifically the automatic replies settings of the signed-in user's mailbox.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_2"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailboxSettings/automaticRepliesSetting
```
##### <a name="response-2"></a><span data-ttu-id="3da51-158">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="3da51-158">Response 2</span></span>
<span data-ttu-id="3da51-p108">Отклик включает только параметры автоматических ответов. Примечание. Показанный здесь объект отклика может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3da51-p108">The response includes only the automatic replies settings. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


##### <a name="request-3"></a><span data-ttu-id="3da51-162">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="3da51-162">Request 3</span></span>
<span data-ttu-id="3da51-163">В третьем примере показано, как получить только параметры рабочего времени для почтового ящика пользователя, выполнившего вход в систему.</span><span class="sxs-lookup"><span data-stu-id="3da51-163">The third example gets specifically the working hour settings of the signed-in user's mailbox.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_mailboxsettings_3"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailboxSettings/workingHours
```
##### <a name="response-3"></a><span data-ttu-id="3da51-164">Ответ 3</span><span class="sxs-lookup"><span data-stu-id="3da51-164">Response 3</span></span>
<span data-ttu-id="3da51-165">Ответ включает только параметры рабочего времени.</span><span class="sxs-lookup"><span data-stu-id="3da51-165">The response includes only the working hours settings.</span></span> <span data-ttu-id="3da51-166">Обратите внимание, что рабочее время пользователя относится к [пользовательскому часовому поясу](../resources/customtimezone.md).</span><span class="sxs-lookup"><span data-stu-id="3da51-166">Notice that the user's work hours are in a [custom time zone](../resources/customtimezone.md).</span></span> <span data-ttu-id="3da51-167">Примечание. Представленный здесь объект ответа может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="3da51-167">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3da51-168">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3da51-168">All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/user-get-mailboxsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
