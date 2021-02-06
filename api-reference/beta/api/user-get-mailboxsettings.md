---
title: Получение параметров почтового ящика пользователя
description: 'Получение объекта mailboxSettings пользователя. Этот объект включает параметры автоматических ответов (автоматического уведомления пользователей при '
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 1cc87e9d4c111c7e0204614df4ece37ecef6452d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131693"
---
# <a name="get-user-mailbox-settings"></a><span data-ttu-id="485e4-104">Получение параметров почтового ящика пользователя</span><span class="sxs-lookup"><span data-stu-id="485e4-104">Get user mailbox settings</span></span>

<span data-ttu-id="485e4-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="485e4-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="485e4-106">Получение объекта [mailboxSettings](../resources/mailboxsettings.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="485e4-106">Get the user's [mailboxSettings](../resources/mailboxsettings.md).</span></span> <span data-ttu-id="485e4-107">Вы можете просмотреть все параметры почтового ящика или получить определенные параметры.</span><span class="sxs-lookup"><span data-stu-id="485e4-107">You can view all mailbox settings, or get specific settings.</span></span>

<span data-ttu-id="485e4-108">Пользователи могут настраивать указанные ниже параметры для своих почтовых ящиков с помощью клиента Outlook:</span><span class="sxs-lookup"><span data-stu-id="485e4-108">Users can set the following settings for their mailboxes through an Outlook client:</span></span>

- <span data-ttu-id="485e4-109">[автоматические ответы](../resources/automaticrepliessetting.md) (автоматическое уведомление пользователей при получении их почты);</span><span class="sxs-lookup"><span data-stu-id="485e4-109">[automatic replies](../resources/automaticrepliessetting.md) (notify people automatically upon receipt of their email)</span></span>
- <span data-ttu-id="485e4-110">формат даты;</span><span class="sxs-lookup"><span data-stu-id="485e4-110">date format</span></span>
- <span data-ttu-id="485e4-111">delegateMeetingMessageDeliveryOptions</span><span class="sxs-lookup"><span data-stu-id="485e4-111">delegateMeetingMessageDeliveryOptions</span></span>
- <span data-ttu-id="485e4-112">[языковой стандарт](../resources/localeinfo.md) (язык и страну или регион);</span><span class="sxs-lookup"><span data-stu-id="485e4-112">[locale](../resources/localeinfo.md) (language and country/region)</span></span>
- <span data-ttu-id="485e4-113">формат времени;</span><span class="sxs-lookup"><span data-stu-id="485e4-113">time format</span></span>
- <span data-ttu-id="485e4-114">часовой пояс;</span><span class="sxs-lookup"><span data-stu-id="485e4-114">time zone</span></span>
- <span data-ttu-id="485e4-115">[рабочее время](../resources/workinghours.md).</span><span class="sxs-lookup"><span data-stu-id="485e4-115">[working hours](../resources/workinghours.md)</span></span>
- [<span data-ttu-id="485e4-116">назначение пользователя</span><span class="sxs-lookup"><span data-stu-id="485e4-116">user purpose</span></span>](../resources/userpurpose.md)

<span data-ttu-id="485e4-117">С помощью Outlook в Интернете пользователи могут настраивать предпочитаемый формат даты и времени.</span><span class="sxs-lookup"><span data-stu-id="485e4-117">Users can set their preferred date and time formats using Outlook on the web.</span></span> <span data-ttu-id="485e4-118">Пользователи могут выбрать один из поддерживаемых [кратких форматов даты](/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortDate) или [кратких форматов времени](/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortTime).</span><span class="sxs-lookup"><span data-stu-id="485e4-118">Users can choose one of the supported [short date](/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortDate) or [short time](/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortTime) formats.</span></span> <span data-ttu-id="485e4-119">Эта операция `GET` возвращает формат, выбранный пользователем.</span><span class="sxs-lookup"><span data-stu-id="485e4-119">This `GET` operation returns the format the user has chosen.</span></span>

<span data-ttu-id="485e4-120">Пользователи могут настроить нужный часовой пояс в любом клиенте Outlook, выбрав из [поддерживаемых часовых поясов](outlookuser-supportedtimezones.md), настроенных администратором для почтового сервера.</span><span class="sxs-lookup"><span data-stu-id="485e4-120">Users can set the time zone they prefer on any Outlook client, by choosing from the [supported time zones](outlookuser-supportedtimezones.md) that their administrator has set up for their mailbox server.</span></span> <span data-ttu-id="485e4-121">Администратор может настроить часовые пояса в формате часовых поясов Windows или [Администрации адресного пространства Интернета](https://www.iana.org/time-zones) (IANA, другое название — часовой пояс Олсона).</span><span class="sxs-lookup"><span data-stu-id="485e4-121">The administrator can set up time zones in the Windows time zone format or  [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="485e4-122">Формат Windows используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="485e4-122">The Windows format is the default.</span></span> 

<span data-ttu-id="485e4-123">Эта операция `GET` возвращает предпочитаемый пользователем часовой пояс в формате, настроенном администратором.</span><span class="sxs-lookup"><span data-stu-id="485e4-123">This `GET` operation returns the user's preferred time zone in the format that the administrator has set up.</span></span> <span data-ttu-id="485e4-124">Чтобы задать определенный формат часового пояса (Windows или IANA), сначала [обновите предпочтительный часовой пояс в этом формате как параметр почтового ящика](user-update-mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="485e4-124">If you want that time zone to be in a specific format (Windows or IANA), you can first [update the preferred time zone in that format as a mailbox setting](user-update-mailboxsettings.md).</span></span> <span data-ttu-id="485e4-125">Затем вы сможете получить часовой пояс в этом формате.</span><span class="sxs-lookup"><span data-stu-id="485e4-125">Subsequently you will be able to get the time zone in that format.</span></span> <span data-ttu-id="485e4-126">Кроме того, вы можете управлять преобразованием форматов в своем приложении.</span><span class="sxs-lookup"><span data-stu-id="485e4-126">Alternatively, you can manage the format conversion separately in your app.</span></span> 

## <a name="permissions"></a><span data-ttu-id="485e4-127">Разрешения</span><span class="sxs-lookup"><span data-stu-id="485e4-127">Permissions</span></span>
<span data-ttu-id="485e4-p106">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="485e4-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="485e4-130">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="485e4-130">Permission type</span></span>      | <span data-ttu-id="485e4-131">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="485e4-131">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="485e4-132">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="485e4-132">Delegated (work or school account)</span></span> | <span data-ttu-id="485e4-133">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="485e4-133">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="485e4-134">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="485e4-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="485e4-135">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="485e4-135">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="485e4-136">Для приложений</span><span class="sxs-lookup"><span data-stu-id="485e4-136">Application</span></span> | <span data-ttu-id="485e4-137">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="485e4-137">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="485e4-138">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="485e4-138">HTTP request</span></span>
<span data-ttu-id="485e4-139">Получение всех параметров почтового ящика пользователя:</span><span class="sxs-lookup"><span data-stu-id="485e4-139">To get all the mailbox settings for a user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings
GET /users/{id|userPrincipalName}/mailboxSettings
```

<span data-ttu-id="485e4-140">Чтобы получить определенные параметры — только параметры автоматических ответов, формат даты, региональные параметры, формат времени, часовой пояс, рабочие часы или назначение пользователя:</span><span class="sxs-lookup"><span data-stu-id="485e4-140">To get specific settings - only the automatic replies settings, date format, locale, time format, time zone, working hours, or user purpose:</span></span>
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

GET /me/mailboxSettings/userPurpose
GET /users/{id|userPrincipalName}/mailboxSettings/userPurpose
```
## <a name="optional-query-parameters"></a><span data-ttu-id="485e4-141">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="485e4-141">Optional query parameters</span></span>
<span data-ttu-id="485e4-142">Этот метод поддерживает некоторые [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="485e4-142">This method supports some of the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="485e4-143">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="485e4-143">Request headers</span></span>
| <span data-ttu-id="485e4-144">Имя</span><span class="sxs-lookup"><span data-stu-id="485e4-144">Name</span></span>       | <span data-ttu-id="485e4-145">Тип</span><span class="sxs-lookup"><span data-stu-id="485e4-145">Type</span></span> | <span data-ttu-id="485e4-146">Описание</span><span class="sxs-lookup"><span data-stu-id="485e4-146">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="485e4-147">Authorization</span><span class="sxs-lookup"><span data-stu-id="485e4-147">Authorization</span></span>  | <span data-ttu-id="485e4-148">string</span><span class="sxs-lookup"><span data-stu-id="485e4-148">string</span></span>  | <span data-ttu-id="485e4-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="485e4-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="485e4-151">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="485e4-151">Request body</span></span>
<span data-ttu-id="485e4-152">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="485e4-152">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="485e4-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="485e4-153">Response</span></span>

<span data-ttu-id="485e4-154">При успешном выполнении этот метод возвращает код отклика `200 OK` и один из указанных ниже запрошенных объектов в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="485e4-154">If successful, this method returns a `200 OK` response code and one of the following requested objects in the response body:</span></span>

- <span data-ttu-id="485e4-155">Объект [mailboxSettings](../resources/mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="485e4-155">[mailboxSettings](../resources/mailboxsettings.md) object</span></span>
- <span data-ttu-id="485e4-156">Объект [automaticRepliesSetting](../resources/automaticrepliessetting.md).</span><span class="sxs-lookup"><span data-stu-id="485e4-156">[automaticRepliesSetting](../resources/automaticrepliessetting.md) object</span></span>
- <span data-ttu-id="485e4-157">Строка (для параметра **dateFormat**).</span><span class="sxs-lookup"><span data-stu-id="485e4-157">string (for **dateFormat**)</span></span>
- <span data-ttu-id="485e4-158">string (для **delegateMeetingMessageDeliveryOptions)**</span><span class="sxs-lookup"><span data-stu-id="485e4-158">string (for **delegateMeetingMessageDeliveryOptions**)</span></span>
- <span data-ttu-id="485e4-159">Объект [localeInfo](../resources/localeinfo.md).</span><span class="sxs-lookup"><span data-stu-id="485e4-159">[localeInfo](../resources/localeinfo.md) object</span></span>
- <span data-ttu-id="485e4-160">Строка (для параметра **timeFormat**).</span><span class="sxs-lookup"><span data-stu-id="485e4-160">string (for **timeFormat**)</span></span>
- <span data-ttu-id="485e4-161">Строка (для параметра **timeZone**).</span><span class="sxs-lookup"><span data-stu-id="485e4-161">string (for **timeZone**)</span></span>
- [<span data-ttu-id="485e4-162">workingHours</span><span class="sxs-lookup"><span data-stu-id="485e4-162">workingHours</span></span>](../resources/workinghours.md)
- [<span data-ttu-id="485e4-163">userPurpose</span><span class="sxs-lookup"><span data-stu-id="485e4-163">userPurpose</span></span>](../resources/userpurpose.md)

## <a name="examples"></a><span data-ttu-id="485e4-164">Примеры</span><span class="sxs-lookup"><span data-stu-id="485e4-164">Examples</span></span>

### <a name="example-1"></a><span data-ttu-id="485e4-165">Пример 1</span><span class="sxs-lookup"><span data-stu-id="485e4-165">Example 1</span></span>
#### <a name="request"></a><span data-ttu-id="485e4-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="485e4-166">Request</span></span> 
<span data-ttu-id="485e4-167">Первый пример получает все параметры почтового ящика воходящего пользователя, которые включают параметры автоматических ответов, формат даты, языковой стандарт (язык и страна или регион), формат времени, часовой пояс, рабочие часы и назначение пользователя.</span><span class="sxs-lookup"><span data-stu-id="485e4-167">The first example gets all the mailbox settings of the signed-in user's mailbox, which include settings for automatic replies, date format, locale (language and country/region), time format, time zone, working hours, and user purpose.</span></span>

# <a name="http"></a>[<span data-ttu-id="485e4-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="485e4-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailboxSettings
```
# <a name="c"></a>[<span data-ttu-id="485e4-169">C#</span><span class="sxs-lookup"><span data-stu-id="485e4-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailboxsettings-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="485e4-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="485e4-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailboxsettings-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="485e4-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="485e4-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailboxsettings-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="485e4-172">Java</span><span class="sxs-lookup"><span data-stu-id="485e4-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailboxsettings-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="485e4-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="485e4-173">Response</span></span>
<span data-ttu-id="485e4-174">Отклик включает все параметры почтового ящика вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="485e4-174">The response includes all the mailbox settings of the signed-in user.</span></span> <span data-ttu-id="485e4-175">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="485e4-175">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="485e4-176">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="485e4-176">All of the properties will be returned from an actual call.</span></span>
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
    },
    "userPurpose": {
        "value": "user"
    },
    "dateFormat": "MM/dd/yyyy",
    "timeFormat": "hh:mm tt",
    "delegateMeetingMessageDeliveryOptions": "sendToDelegateOnly"
}
```

### <a name="example-2"></a><span data-ttu-id="485e4-177">Пример 2</span><span class="sxs-lookup"><span data-stu-id="485e4-177">Example 2</span></span>
#### <a name="request"></a><span data-ttu-id="485e4-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="485e4-178">Request</span></span>
<span data-ttu-id="485e4-179">Во втором примере показано, как получить только параметры автоматических ответов почтового ящика пользователя, выполнившего вход в систему.</span><span class="sxs-lookup"><span data-stu-id="485e4-179">The second example gets specifically the automatic replies settings of the signed-in user's mailbox.</span></span>

# <a name="http"></a>[<span data-ttu-id="485e4-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="485e4-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailboxSettings/automaticRepliesSetting
```
# <a name="c"></a>[<span data-ttu-id="485e4-181">C#</span><span class="sxs-lookup"><span data-stu-id="485e4-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailboxsettings-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="485e4-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="485e4-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailboxsettings-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="485e4-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="485e4-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailboxsettings-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="485e4-184">Java</span><span class="sxs-lookup"><span data-stu-id="485e4-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailboxsettings-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="485e4-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="485e4-185">Response</span></span>
<span data-ttu-id="485e4-p109">Отклик включает только параметры автоматических ответов. Примечание. Показанный здесь объект отклика может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="485e4-p109">The response includes only the automatic replies settings. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

### <a name="example-3"></a><span data-ttu-id="485e4-189">Пример 3</span><span class="sxs-lookup"><span data-stu-id="485e4-189">Example 3</span></span>
#### <a name="request"></a><span data-ttu-id="485e4-190">Запрос</span><span class="sxs-lookup"><span data-stu-id="485e4-190">Request</span></span>
<span data-ttu-id="485e4-191">В третьем примере показано, как получить только параметры рабочего времени для почтового ящика пользователя, выполнившего вход в систему.</span><span class="sxs-lookup"><span data-stu-id="485e4-191">The third example gets specifically the working hour settings of the signed-in user's mailbox.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_mailboxsettings_3"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailboxSettings/workingHours
```
#### <a name="response"></a><span data-ttu-id="485e4-192">Отклик</span><span class="sxs-lookup"><span data-stu-id="485e4-192">Response</span></span>
<span data-ttu-id="485e4-193">Ответ включает только параметры рабочего времени.</span><span class="sxs-lookup"><span data-stu-id="485e4-193">The response includes only the working hours settings.</span></span> <span data-ttu-id="485e4-194">Обратите внимание, что рабочее время пользователя относится к [пользовательскому часовому поясу](../resources/customtimezone.md).</span><span class="sxs-lookup"><span data-stu-id="485e4-194">Notice that the user's work hours are in a [custom time zone](../resources/customtimezone.md).</span></span> <span data-ttu-id="485e4-195">Примечание. Представленный здесь объект ответа может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="485e4-195">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="485e4-196">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="485e4-196">All of the properties will be returned from an actual call.</span></span>
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

### <a name="example-4"></a><span data-ttu-id="485e4-197">Пример 4</span><span class="sxs-lookup"><span data-stu-id="485e4-197">Example 4</span></span>
#### <a name="request"></a><span data-ttu-id="485e4-198">Запрос</span><span class="sxs-lookup"><span data-stu-id="485e4-198">Request</span></span>
<span data-ttu-id="485e4-199">В четвертом примере [](../resources/userpurpose.md) получаются параметры назначения пользователя для почтового ящика воходящего пользователя.</span><span class="sxs-lookup"><span data-stu-id="485e4-199">The fourth example gets specifically the [user purpose](../resources/userpurpose.md) settings of the signed-in user's mailbox.</span></span>

# <a name="http"></a>[<span data-ttu-id="485e4-200">HTTP</span><span class="sxs-lookup"><span data-stu-id="485e4-200">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_4"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailboxSettings/userPurpose
```
# <a name="c"></a>[<span data-ttu-id="485e4-201">C#</span><span class="sxs-lookup"><span data-stu-id="485e4-201">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailboxsettings-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="485e4-202">JavaScript</span><span class="sxs-lookup"><span data-stu-id="485e4-202">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailboxsettings-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="485e4-203">Objective-C</span><span class="sxs-lookup"><span data-stu-id="485e4-203">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailboxsettings-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="485e4-204">Java</span><span class="sxs-lookup"><span data-stu-id="485e4-204">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailboxsettings-4-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="485e4-205">Отклик</span><span class="sxs-lookup"><span data-stu-id="485e4-205">Response</span></span>
<span data-ttu-id="485e4-206">Ответ включает только параметры [назначения](../resources/userpurpose.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="485e4-206">The response includes only the [user purpose](../resources/userpurpose.md) settings.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_mailboxsettings_4",
  "truncated": true,
  "@odata.type": "microsoft.graph.userPurpose"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('622eaaff-0683-4862-9de4-f2ec83c2bd98')/mailboxSettings/userPurpose",
    "value": "user"
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
