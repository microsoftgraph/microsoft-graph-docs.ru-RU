---
title: Получение параметров почтового ящика пользователя
description: 'Получение объекта mailboxSettings пользователя. Этот объект включает параметры автоматических ответов (автоматического уведомления пользователей при '
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e2f697a332eb4912f0f4f442f57ccf79b86d03ca
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054310"
---
# <a name="get-user-mailbox-settings"></a><span data-ttu-id="9d27a-104">Получение параметров почтового ящика пользователя</span><span class="sxs-lookup"><span data-stu-id="9d27a-104">Get user mailbox settings</span></span>

<span data-ttu-id="9d27a-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d27a-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9d27a-106">Получение объекта [mailboxSettings](../resources/mailboxsettings.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="9d27a-106">Get the user's [mailboxSettings](../resources/mailboxsettings.md).</span></span> <span data-ttu-id="9d27a-107">Вы можете просмотреть все параметры почтового ящика или получить определенные параметры.</span><span class="sxs-lookup"><span data-stu-id="9d27a-107">You can view all mailbox settings, or get specific settings.</span></span>

<span data-ttu-id="9d27a-108">Пользователи могут настраивать указанные ниже параметры для своих почтовых ящиков с помощью клиента Outlook:</span><span class="sxs-lookup"><span data-stu-id="9d27a-108">Users can set the following settings for their mailboxes through an Outlook client:</span></span>

- <span data-ttu-id="9d27a-109">[автоматические ответы](../resources/automaticrepliessetting.md) (автоматическое уведомление пользователей при получении их почты);</span><span class="sxs-lookup"><span data-stu-id="9d27a-109">[automatic replies](../resources/automaticrepliessetting.md) (notify people automatically upon receipt of their email)</span></span>
- <span data-ttu-id="9d27a-110">формат даты;</span><span class="sxs-lookup"><span data-stu-id="9d27a-110">date format</span></span>
- <span data-ttu-id="9d27a-111">delegateMeetingMessageDeliveryOptions</span><span class="sxs-lookup"><span data-stu-id="9d27a-111">delegateMeetingMessageDeliveryOptions</span></span>
- <span data-ttu-id="9d27a-112">[языковой стандарт](../resources/localeinfo.md) (язык и страну или регион);</span><span class="sxs-lookup"><span data-stu-id="9d27a-112">[locale](../resources/localeinfo.md) (language and country/region)</span></span>
- <span data-ttu-id="9d27a-113">формат времени;</span><span class="sxs-lookup"><span data-stu-id="9d27a-113">time format</span></span>
- <span data-ttu-id="9d27a-114">часовой пояс;</span><span class="sxs-lookup"><span data-stu-id="9d27a-114">time zone</span></span>
- <span data-ttu-id="9d27a-115">[рабочее время](../resources/workinghours.md).</span><span class="sxs-lookup"><span data-stu-id="9d27a-115">[working hours](../resources/workinghours.md)</span></span>

<span data-ttu-id="9d27a-116">С помощью Outlook в Интернете пользователи могут настраивать предпочитаемый формат даты и времени.</span><span class="sxs-lookup"><span data-stu-id="9d27a-116">Users can set their preferred date and time formats using Outlook on the web.</span></span> <span data-ttu-id="9d27a-117">Пользователи могут выбрать один из поддерживаемых [кратких форматов даты](/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortDate) или [кратких форматов времени](/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortTime).</span><span class="sxs-lookup"><span data-stu-id="9d27a-117">Users can choose one of the supported [short date](/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortDate) or [short time](/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortTime) formats.</span></span> <span data-ttu-id="9d27a-118">Эта операция `GET` возвращает формат, выбранный пользователем.</span><span class="sxs-lookup"><span data-stu-id="9d27a-118">This `GET` operation returns the format the user has chosen.</span></span>

<span data-ttu-id="9d27a-119">Пользователи могут настроить нужный часовой пояс в любом клиенте Outlook, выбрав из [поддерживаемых часовых поясов](outlookuser-supportedtimezones.md), настроенных администратором для почтового сервера.</span><span class="sxs-lookup"><span data-stu-id="9d27a-119">Users can set the time zone they prefer on any Outlook client, by choosing from the [supported time zones](outlookuser-supportedtimezones.md) that their administrator has set up for their mailbox server.</span></span> <span data-ttu-id="9d27a-120">Администратор может настроить часовые пояса в формате часовых поясов Windows или [Администрации адресного пространства Интернета](https://www.iana.org/time-zones) (IANA, другое название — часовой пояс Олсона).</span><span class="sxs-lookup"><span data-stu-id="9d27a-120">The administrator can set up time zones in the Windows time zone format or  [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="9d27a-121">Формат Windows используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="9d27a-121">The Windows format is the default.</span></span>

<span data-ttu-id="9d27a-122">Эта операция `GET` возвращает предпочитаемый пользователем часовой пояс в формате, настроенном администратором.</span><span class="sxs-lookup"><span data-stu-id="9d27a-122">This `GET` operation returns the user's preferred time zone in the format that the administrator has set up.</span></span> <span data-ttu-id="9d27a-123">Чтобы задать определенный формат часового пояса (Windows или IANA), сначала [обновите предпочтительный часовой пояс в этом формате как параметр почтового ящика](user-update-mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="9d27a-123">If you want that time zone to be in a specific format (Windows or IANA), you can first [update the preferred time zone in that format as a mailbox setting](user-update-mailboxsettings.md).</span></span> <span data-ttu-id="9d27a-124">Затем вы сможете получить часовой пояс в этом формате.</span><span class="sxs-lookup"><span data-stu-id="9d27a-124">Subsequently you will be able to get the time zone in that format.</span></span> <span data-ttu-id="9d27a-125">Кроме того, вы можете управлять преобразованием форматов в своем приложении.</span><span class="sxs-lookup"><span data-stu-id="9d27a-125">Alternatively, you can manage the format conversion separately in your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="9d27a-126">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9d27a-126">Permissions</span></span>
<span data-ttu-id="9d27a-p106">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d27a-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d27a-129">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9d27a-129">Permission type</span></span>      | <span data-ttu-id="9d27a-130">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9d27a-130">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d27a-131">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9d27a-131">Delegated (work or school account)</span></span> | <span data-ttu-id="9d27a-132">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9d27a-132">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="9d27a-133">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9d27a-133">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d27a-134">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9d27a-134">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="9d27a-135">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9d27a-135">Application</span></span> | <span data-ttu-id="9d27a-136">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9d27a-136">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d27a-137">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9d27a-137">HTTP request</span></span>
<span data-ttu-id="9d27a-138">Получение всех параметров почтового ящика пользователя:</span><span class="sxs-lookup"><span data-stu-id="9d27a-138">To get all the mailbox settings for a user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings
GET /users/{id|userPrincipalName}/mailboxSettings
```

<span data-ttu-id="9d27a-139">Получение определенных параметров (только параметров автоматических ответов, формата даты, языкового стандарта, часового пояса или рабочего времени):</span><span class="sxs-lookup"><span data-stu-id="9d27a-139">To get specific settings - only the automatic replies settings, date format, locale, time format, time zone, or working hours:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings/automaticRepliesSetting
GET /users/{id|userPrincipalName}/mailboxSettings/automaticRepliesSetting

GET /me/mailboxSettings/dateFormat
GET /users/{id|userPrincipalName}/mailboxSettings/dateFormat

GET /me/mailboxSettings/delegateMeetingMessageDeliveryOptions
GET /users/{id|userPrincipalName}/mailboxSettings/delegateMeetingMessageDeliveryOptions

GET /me/mailboxSettings/language
GET /users/{id|userPrincipalName}/mailboxSettings/language

GET /me/mailboxSettings/timeFormat
GET /users/{id|userPrincipalName}/mailboxSettings/timeFormat

GET /me/mailboxSettings/timeZone
GET /users/{id|userPrincipalName}/mailboxSettings/timeZone

GET /me/mailboxSettings/workingHours
GET /users/{id|userPrincipalName}/mailboxSettings/workingHours
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9d27a-140">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9d27a-140">Optional query parameters</span></span>
<span data-ttu-id="9d27a-141">Этот метод поддерживает некоторые [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="9d27a-141">This method supports some of the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9d27a-142">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9d27a-142">Request headers</span></span>
| <span data-ttu-id="9d27a-143">Имя</span><span class="sxs-lookup"><span data-stu-id="9d27a-143">Name</span></span>       | <span data-ttu-id="9d27a-144">Тип</span><span class="sxs-lookup"><span data-stu-id="9d27a-144">Type</span></span> | <span data-ttu-id="9d27a-145">Описание</span><span class="sxs-lookup"><span data-stu-id="9d27a-145">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9d27a-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d27a-146">Authorization</span></span>  | <span data-ttu-id="9d27a-147">string</span><span class="sxs-lookup"><span data-stu-id="9d27a-147">string</span></span>  | <span data-ttu-id="9d27a-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9d27a-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9d27a-150">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9d27a-150">Request body</span></span>
<span data-ttu-id="9d27a-151">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9d27a-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9d27a-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d27a-152">Response</span></span>

<span data-ttu-id="9d27a-153">При успешном выполнении этот метод возвращает код отклика `200 OK` и один из указанных ниже запрошенных объектов в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9d27a-153">If successful, this method returns a `200 OK` response code and one of the following requested objects in the response body:</span></span>

- <span data-ttu-id="9d27a-154">Объект [mailboxSettings](../resources/mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="9d27a-154">[mailboxSettings](../resources/mailboxsettings.md) object</span></span>
- <span data-ttu-id="9d27a-155">Объект [automaticRepliesSetting](../resources/automaticrepliessetting.md).</span><span class="sxs-lookup"><span data-stu-id="9d27a-155">[automaticRepliesSetting](../resources/automaticrepliessetting.md) object</span></span>
- <span data-ttu-id="9d27a-156">Строка (для параметра **dateFormat**).</span><span class="sxs-lookup"><span data-stu-id="9d27a-156">string (for **dateFormat**)</span></span>
- <span data-ttu-id="9d27a-157">string **(для delegateMeetingMessageDeliveryOptions)**</span><span class="sxs-lookup"><span data-stu-id="9d27a-157">string (for **delegateMeetingMessageDeliveryOptions**)</span></span>
- <span data-ttu-id="9d27a-158">Объект [localeInfo](../resources/localeinfo.md).</span><span class="sxs-lookup"><span data-stu-id="9d27a-158">[localeInfo](../resources/localeinfo.md) object</span></span>
- <span data-ttu-id="9d27a-159">Строка (для параметра **timeFormat**).</span><span class="sxs-lookup"><span data-stu-id="9d27a-159">string (for **timeFormat**)</span></span>
- <span data-ttu-id="9d27a-160">Строка (для параметра **timeZone**).</span><span class="sxs-lookup"><span data-stu-id="9d27a-160">string (for **timeZone**)</span></span>
- [<span data-ttu-id="9d27a-161">workingHours</span><span class="sxs-lookup"><span data-stu-id="9d27a-161">workingHours</span></span>](../resources/workinghours.md)

## <a name="examples"></a><span data-ttu-id="9d27a-162">Примеры</span><span class="sxs-lookup"><span data-stu-id="9d27a-162">Examples</span></span>

### <a name="example-1"></a><span data-ttu-id="9d27a-163">Пример 1</span><span class="sxs-lookup"><span data-stu-id="9d27a-163">Example 1</span></span>
#### <a name="request"></a><span data-ttu-id="9d27a-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="9d27a-164">Request</span></span>
<span data-ttu-id="9d27a-165">В первом примере считываются все параметры для почтового ящика вошедшего пользователя, в том числе параметры автоматических ответов, формата даты, языкового стандарта (язык и страна или регион), формата времени, часового пояса и рабочего времени.</span><span class="sxs-lookup"><span data-stu-id="9d27a-165">The first example gets all the mailbox settings of the signed-in user's mailbox, which include settings for automatic replies, date format, locale (language and country/region), time format, time zone, and working hours.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailboxSettings
```

#### <a name="response"></a><span data-ttu-id="9d27a-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d27a-166">Response</span></span>
<span data-ttu-id="9d27a-167">Отклик включает все параметры почтового ящика вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="9d27a-167">The response includes all the mailbox settings of the signed-in user.</span></span>
<span data-ttu-id="9d27a-168">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9d27a-168">Note: The response object shown here might be shortened for readability.</span></span>
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
    "timeFormat": "hh:mm tt",
    "delegateMeetingMessageDeliveryOptions": "sendToDelegateOnly"
}
```

### <a name="example-2"></a><span data-ttu-id="9d27a-169">Пример 2</span><span class="sxs-lookup"><span data-stu-id="9d27a-169">Example 2</span></span>
#### <a name="request"></a><span data-ttu-id="9d27a-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="9d27a-170">Request</span></span>
<span data-ttu-id="9d27a-171">Во втором примере показано, как получить только параметры автоматических ответов почтового ящика пользователя, выполнившего вход в систему.</span><span class="sxs-lookup"><span data-stu-id="9d27a-171">The second example gets specifically the automatic replies settings of the signed-in user's mailbox.</span></span>

# <a name="http"></a>[<span data-ttu-id="9d27a-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="9d27a-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailboxSettings/automaticRepliesSetting
```
# <a name="c"></a>[<span data-ttu-id="9d27a-173">C#</span><span class="sxs-lookup"><span data-stu-id="9d27a-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailboxsettings-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9d27a-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9d27a-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailboxsettings-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9d27a-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9d27a-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailboxsettings-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9d27a-176">Java</span><span class="sxs-lookup"><span data-stu-id="9d27a-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailboxsettings-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="9d27a-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d27a-177">Response</span></span>
<span data-ttu-id="9d27a-178">Ответ включает только параметры автоматических ответов.</span><span class="sxs-lookup"><span data-stu-id="9d27a-178">The response includes only the automatic replies settings.</span></span>
<span data-ttu-id="9d27a-179">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9d27a-179">Note: The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-3"></a><span data-ttu-id="9d27a-180">Пример 3</span><span class="sxs-lookup"><span data-stu-id="9d27a-180">Example 3</span></span>
#### <a name="request"></a><span data-ttu-id="9d27a-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="9d27a-181">Request</span></span>
<span data-ttu-id="9d27a-182">В третьем примере показано, как получить только параметры рабочего времени для почтового ящика пользователя, выполнившего вход в систему.</span><span class="sxs-lookup"><span data-stu-id="9d27a-182">The third example gets specifically the working hour settings of the signed-in user's mailbox.</span></span>

# <a name="http"></a>[<span data-ttu-id="9d27a-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="9d27a-183">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_3"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailboxSettings/workingHours
```
# <a name="c"></a>[<span data-ttu-id="9d27a-184">C#</span><span class="sxs-lookup"><span data-stu-id="9d27a-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailboxsettings-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9d27a-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9d27a-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailboxsettings-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9d27a-186">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9d27a-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailboxsettings-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9d27a-187">Java</span><span class="sxs-lookup"><span data-stu-id="9d27a-187">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailboxsettings-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="9d27a-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d27a-188">Response</span></span>
<span data-ttu-id="9d27a-189">Ответ включает только параметры рабочего времени.</span><span class="sxs-lookup"><span data-stu-id="9d27a-189">The response includes only the working hours settings.</span></span> <span data-ttu-id="9d27a-190">Обратите внимание, что рабочее время пользователя относится к [пользовательскому часовому поясу](../resources/customtimezone.md).</span><span class="sxs-lookup"><span data-stu-id="9d27a-190">Notice that the user's work hours are in a [custom time zone](../resources/customtimezone.md).</span></span>
<span data-ttu-id="9d27a-191">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9d27a-191">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
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
