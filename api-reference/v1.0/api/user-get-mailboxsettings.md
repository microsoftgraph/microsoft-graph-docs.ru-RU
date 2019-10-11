---
title: Получение параметров почтового ящика пользователя
description: 'Получение объекта mailboxSettings пользователя. Этот объект включает параметры автоматических ответов (автоматического уведомления пользователей при '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: d4cb9e9a665ea6e1a06162ddc6cee3067f0e21d1
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2019
ms.locfileid: "37427762"
---
# <a name="get-user-mailbox-settings"></a><span data-ttu-id="371bc-104">Получение параметров почтового ящика пользователя</span><span class="sxs-lookup"><span data-stu-id="371bc-104">Get user mailbox settings</span></span>

<span data-ttu-id="371bc-105">Получение объекта [mailboxSettings](../resources/mailboxsettings.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="371bc-105">Get the user's [mailboxSettings](../resources/mailboxsettings.md).</span></span> <span data-ttu-id="371bc-106">Вы можете просмотреть все параметры почтового ящика или получить определенные параметры.</span><span class="sxs-lookup"><span data-stu-id="371bc-106">You can view all mailbox settings, or get specific settings.</span></span>

<span data-ttu-id="371bc-107">Пользователи могут настраивать указанные ниже параметры для своих почтовых ящиков с помощью клиента Outlook:</span><span class="sxs-lookup"><span data-stu-id="371bc-107">Users can set the following settings for their mailboxes through an Outlook client:</span></span>

- <span data-ttu-id="371bc-108">[автоматические ответы](../resources/automaticrepliessetting.md) (автоматическое уведомление пользователей при получении их почты);</span><span class="sxs-lookup"><span data-stu-id="371bc-108">[automatic replies](../resources/automaticrepliessetting.md) (notify people automatically upon receipt of their email)</span></span>
- <span data-ttu-id="371bc-109">формат даты;</span><span class="sxs-lookup"><span data-stu-id="371bc-109">date format</span></span>
- <span data-ttu-id="371bc-110">[языковой стандарт](../resources/localeinfo.md) (язык и страну или регион);</span><span class="sxs-lookup"><span data-stu-id="371bc-110">[locale](../resources/localeinfo.md) (language and country/region)</span></span>
- <span data-ttu-id="371bc-111">формат времени;</span><span class="sxs-lookup"><span data-stu-id="371bc-111">time format</span></span>
- <span data-ttu-id="371bc-112">часовой пояс;</span><span class="sxs-lookup"><span data-stu-id="371bc-112">time zone</span></span>
- <span data-ttu-id="371bc-113">[рабочее время](../resources/workinghours.md).</span><span class="sxs-lookup"><span data-stu-id="371bc-113">[working hours](../resources/workinghours.md)</span></span>

<span data-ttu-id="371bc-114">С помощью Outlook в Интернете пользователи могут настраивать предпочитаемый формат даты и времени.</span><span class="sxs-lookup"><span data-stu-id="371bc-114">Users can set their preferred date and time formats using Outlook on the web.</span></span> <span data-ttu-id="371bc-115">Пользователи могут выбрать один из поддерживаемых [кратких форматов даты](https://docs.microsoft.com/en-us/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortDate) или [кратких форматов времени](https://docs.microsoft.com/en-us/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortTime).</span><span class="sxs-lookup"><span data-stu-id="371bc-115">Users can choose one of the supported [short date](https://docs.microsoft.com/en-us/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortDate) or [short time](https://docs.microsoft.com/en-us/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortTime) formats.</span></span> <span data-ttu-id="371bc-116">Эта операция `GET` возвращает формат, выбранный пользователем.</span><span class="sxs-lookup"><span data-stu-id="371bc-116">This `GET` operation returns the format the user has chosen.</span></span>

<span data-ttu-id="371bc-117">Пользователи могут настроить нужный часовой пояс в любом клиенте Outlook, выбрав из [поддерживаемых часовых поясов](outlookuser-supportedtimezones.md), настроенных администратором для почтового сервера.</span><span class="sxs-lookup"><span data-stu-id="371bc-117">Users can set the time zone they prefer on any Outlook client, by choosing from the [supported time zones](outlookuser-supportedtimezones.md) that their administrator has set up for their mailbox server.</span></span> <span data-ttu-id="371bc-118">Администратор может настроить часовые пояса в формате часовых поясов Windows или [Администрации адресного пространства Интернета](https://www.iana.org/time-zones) (IANA, другое название — часовой пояс Олсона).</span><span class="sxs-lookup"><span data-stu-id="371bc-118">The administrator can set up time zones in the Windows time zone format or  [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="371bc-119">Формат Windows используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="371bc-119">The Windows format is the default.</span></span> 

<span data-ttu-id="371bc-120">Эта операция `GET` возвращает предпочитаемый пользователем часовой пояс в формате, настроенном администратором.</span><span class="sxs-lookup"><span data-stu-id="371bc-120">This `GET` operation returns the user's preferred time zone in the format that the administrator has set up.</span></span> <span data-ttu-id="371bc-121">Чтобы задать определенный формат часового пояса (Windows или IANA), сначала [обновите предпочтительный часовой пояс в этом формате как параметр почтового ящика](user-update-mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="371bc-121">If you want that time zone to be in a specific format (Windows or IANA), you can first [update the preferred time zone in that format as a mailbox setting](user-update-mailboxsettings.md).</span></span> <span data-ttu-id="371bc-122">Затем вы сможете получить часовой пояс в этом формате.</span><span class="sxs-lookup"><span data-stu-id="371bc-122">Subsequently you will be able to get the time zone in that format.</span></span> <span data-ttu-id="371bc-123">Кроме того, вы можете управлять преобразованием форматов в своем приложении.</span><span class="sxs-lookup"><span data-stu-id="371bc-123">Alternatively, you can manage the format conversion separately in your app.</span></span> 

## <a name="permissions"></a><span data-ttu-id="371bc-124">Разрешения</span><span class="sxs-lookup"><span data-stu-id="371bc-124">Permissions</span></span>
<span data-ttu-id="371bc-p106">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="371bc-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="371bc-127">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="371bc-127">Permission type</span></span>      | <span data-ttu-id="371bc-128">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="371bc-128">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="371bc-129">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="371bc-129">Delegated (work or school account)</span></span> | <span data-ttu-id="371bc-130">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="371bc-130">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="371bc-131">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="371bc-131">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="371bc-132">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="371bc-132">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="371bc-133">Для приложений</span><span class="sxs-lookup"><span data-stu-id="371bc-133">Application</span></span> | <span data-ttu-id="371bc-134">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="371bc-134">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="371bc-135">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="371bc-135">HTTP request</span></span>
<span data-ttu-id="371bc-136">Получение всех параметров почтового ящика пользователя:</span><span class="sxs-lookup"><span data-stu-id="371bc-136">To get all the mailbox settings for a user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings
GET /users/{id|userPrincipalName}/mailboxSettings
```

<span data-ttu-id="371bc-137">Получение определенных параметров (только параметров автоматических ответов, формата даты, языкового стандарта, часового пояса или рабочего времени):</span><span class="sxs-lookup"><span data-stu-id="371bc-137">To get specific settings - only the automatic replies settings, date format, locale, time format, time zone, or working hours:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings/automaticRepliesSetting
GET /users/{id|userPrincipalName}/mailboxSettings/automaticRepliesSetting

GET /me/mailboxSettings/dateFormat
GET /users/{id|userPrincipalName}/mailboxSettings/dateFormat

GET /me/mailboxSettings/language
GET /users/{id|userPrincipalName}/mailboxSettings/language

GET /me/mailboxSettings/timeFormat
GET /users/{id|userPrincipalName}/mailboxSettings/timeFormat

GET /me/mailboxSettings/timeZone
GET /users/{id|userPrincipalName}/mailboxSettings/timeZone

GET /me/mailboxSettings/workingHours
GET /users/{id|userPrincipalName}/mailboxSettings/workingHours
```
## <a name="optional-query-parameters"></a><span data-ttu-id="371bc-138">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="371bc-138">Optional query parameters</span></span>
<span data-ttu-id="371bc-139">Этот метод поддерживает некоторые [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="371bc-139">This method supports some of the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="371bc-140">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="371bc-140">Request headers</span></span>
| <span data-ttu-id="371bc-141">Имя</span><span class="sxs-lookup"><span data-stu-id="371bc-141">Name</span></span>       | <span data-ttu-id="371bc-142">Тип</span><span class="sxs-lookup"><span data-stu-id="371bc-142">Type</span></span> | <span data-ttu-id="371bc-143">Описание</span><span class="sxs-lookup"><span data-stu-id="371bc-143">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="371bc-144">Authorization</span><span class="sxs-lookup"><span data-stu-id="371bc-144">Authorization</span></span>  | <span data-ttu-id="371bc-145">string</span><span class="sxs-lookup"><span data-stu-id="371bc-145">string</span></span>  | <span data-ttu-id="371bc-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="371bc-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="371bc-148">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="371bc-148">Request body</span></span>
<span data-ttu-id="371bc-149">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="371bc-149">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="371bc-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="371bc-150">Response</span></span>

<span data-ttu-id="371bc-151">При успешном выполнении этот метод возвращает код отклика `200 OK` и один из указанных ниже запрошенных объектов в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="371bc-151">If successful, this method returns a `200 OK` response code and one of the following requested objects in the response body:</span></span>

- <span data-ttu-id="371bc-152">Объект [mailboxSettings](../resources/mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="371bc-152">[mailboxSettings](../resources/mailboxsettings.md) object</span></span>
- <span data-ttu-id="371bc-153">Объект [automaticRepliesSetting](../resources/automaticrepliessetting.md).</span><span class="sxs-lookup"><span data-stu-id="371bc-153">[automaticRepliesSetting](../resources/automaticrepliessetting.md) object</span></span>
- <span data-ttu-id="371bc-154">Строка (для параметра **dateFormat**).</span><span class="sxs-lookup"><span data-stu-id="371bc-154">string (for **dateFormat**)</span></span>
- <span data-ttu-id="371bc-155">Объект [localeInfo](../resources/localeinfo.md).</span><span class="sxs-lookup"><span data-stu-id="371bc-155">[localeInfo](../resources/localeinfo.md) object</span></span>
- <span data-ttu-id="371bc-156">Строка (для параметра **timeFormat**).</span><span class="sxs-lookup"><span data-stu-id="371bc-156">string (for **timeFormat**)</span></span>
- <span data-ttu-id="371bc-157">Строка (для параметра **timeZone**).</span><span class="sxs-lookup"><span data-stu-id="371bc-157">string (for **timeZone**)</span></span>
- [<span data-ttu-id="371bc-158">workingHours</span><span class="sxs-lookup"><span data-stu-id="371bc-158">workingHours</span></span>](../resources/workinghours.md)

## <a name="examples"></a><span data-ttu-id="371bc-159">Примеры</span><span class="sxs-lookup"><span data-stu-id="371bc-159">Examples</span></span>

### <a name="example-1"></a><span data-ttu-id="371bc-160">Пример 1</span><span class="sxs-lookup"><span data-stu-id="371bc-160">Example 1</span></span>
#### <a name="request"></a><span data-ttu-id="371bc-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="371bc-161">Request</span></span> 
<span data-ttu-id="371bc-162">В первом примере считываются все параметры для почтового ящика вошедшего пользователя, в том числе параметры автоматических ответов, формата даты, языкового стандарта (язык и страна или регион), формата времени, часового пояса и рабочего времени.</span><span class="sxs-lookup"><span data-stu-id="371bc-162">The first example gets all the mailbox settings of the signed-in user's mailbox, which include settings for automatic replies, date format, locale (language and country/region), time format, time zone, and working hours.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailboxSettings
```

#### <a name="response"></a><span data-ttu-id="371bc-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="371bc-163">Response</span></span>
<span data-ttu-id="371bc-164">Отклик включает все параметры почтового ящика вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="371bc-164">The response includes all the mailbox settings of the signed-in user.</span></span> <span data-ttu-id="371bc-165">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="371bc-165">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="371bc-166">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="371bc-166">All of the properties will be returned from an actual call.</span></span>
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
        "startTime": "08:00:00.0000000",
        "endTime": "17:00:00.0000000",
        "timeZone":{
            "name":"Pacific Standard Time"
        }
    },
    "dateFormat": "MM/dd/yyyy",
    "timeFormat": "hh:mm tt"
}
```

### <a name="example-2"></a><span data-ttu-id="371bc-167">Пример 2</span><span class="sxs-lookup"><span data-stu-id="371bc-167">Example 2</span></span>
#### <a name="request"></a><span data-ttu-id="371bc-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="371bc-168">Request</span></span>
<span data-ttu-id="371bc-169">Во втором примере показано, как получить только параметры автоматических ответов почтового ящика пользователя, выполнившего вход в систему.</span><span class="sxs-lookup"><span data-stu-id="371bc-169">The second example gets specifically the automatic replies settings of the signed-in user's mailbox.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="371bc-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="371bc-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailboxSettings/automaticRepliesSetting
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="371bc-171">C#</span><span class="sxs-lookup"><span data-stu-id="371bc-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailboxsettings-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="371bc-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="371bc-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailboxsettings-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="371bc-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="371bc-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailboxsettings-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="371bc-174">Java</span><span class="sxs-lookup"><span data-stu-id="371bc-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailboxsettings-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="371bc-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="371bc-175">Response</span></span>
<span data-ttu-id="371bc-p109">Отклик включает только параметры автоматических ответов. Примечание. Показанный здесь объект отклика может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="371bc-p109">The response includes only the automatic replies settings. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.automaticRepliesSetting"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/mailboxSettings/automaticRepliesSetting",
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

### <a name="example-3"></a><span data-ttu-id="371bc-179">Пример 3</span><span class="sxs-lookup"><span data-stu-id="371bc-179">Example 3</span></span>
#### <a name="request"></a><span data-ttu-id="371bc-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="371bc-180">Request</span></span>
<span data-ttu-id="371bc-181">В третьем примере показано, как получить только параметры рабочего времени для почтового ящика пользователя, выполнившего вход в систему.</span><span class="sxs-lookup"><span data-stu-id="371bc-181">The third example gets specifically the working hour settings of the signed-in user's mailbox.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_mailboxsettings_3"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailboxSettings/workingHours
```
#### <a name="response"></a><span data-ttu-id="371bc-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="371bc-182">Response</span></span>
<span data-ttu-id="371bc-183">Ответ включает только параметры рабочего времени.</span><span class="sxs-lookup"><span data-stu-id="371bc-183">The response includes only the working hours settings.</span></span> <span data-ttu-id="371bc-184">Обратите внимание, что рабочее время пользователя относится к [пользовательскому часовому поясу](../resources/customtimezone.md).</span><span class="sxs-lookup"><span data-stu-id="371bc-184">Notice that the user's work hours are in a [custom time zone](../resources/customtimezone.md).</span></span> <span data-ttu-id="371bc-185">Примечание. Представленный здесь объект ответа может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="371bc-185">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="371bc-186">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="371bc-186">All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
