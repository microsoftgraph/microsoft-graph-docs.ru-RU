---
title: Обновление параметров почтового ящика пользователя
description: Обновление одного или нескольких параметров почтового ящика пользователя. Сюда входят параметры для автоматических ответов (уведомлять пользователей автоматически после получения их электронной почты), языковой стандарт (язык и страну или регион), часовой пояс и рабочие часы.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 088b1f1d6f575cc96029f282ae6608cdeff6b3fb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508914"
---
# <a name="update-user-mailbox-settings"></a><span data-ttu-id="270dd-104">Обновление параметров почтового ящика пользователя</span><span class="sxs-lookup"><span data-stu-id="270dd-104">Update user mailbox settings</span></span>

<span data-ttu-id="270dd-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="270dd-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="270dd-106">Включить, настроить или отключить один или несколько из следующих параметров в составе [mailboxSettings](../resources/mailboxsettings.md)пользователя:</span><span class="sxs-lookup"><span data-stu-id="270dd-106">Enable, configure, or disable one or more of the following settings as part of a user's [mailboxSettings](../resources/mailboxsettings.md):</span></span>

- <span data-ttu-id="270dd-107">[автоматические ответы](../resources/automaticrepliessetting.md) (автоматическое уведомление пользователей при получении их почты);</span><span class="sxs-lookup"><span data-stu-id="270dd-107">[automatic replies](../resources/automaticrepliessetting.md) (notify people automatically upon receipt of their email)</span></span>
- <span data-ttu-id="270dd-108">dateFormat</span><span class="sxs-lookup"><span data-stu-id="270dd-108">dateFormat</span></span>
- <span data-ttu-id="270dd-109">[языковой стандарт](../resources/localeinfo.md) (язык и страну или регион);</span><span class="sxs-lookup"><span data-stu-id="270dd-109">[locale](../resources/localeinfo.md) (language and country/region)</span></span>
- <span data-ttu-id="270dd-110">тимеформат</span><span class="sxs-lookup"><span data-stu-id="270dd-110">timeFormat</span></span>
- <span data-ttu-id="270dd-111">часовой пояс;</span><span class="sxs-lookup"><span data-stu-id="270dd-111">time zone</span></span>
- <span data-ttu-id="270dd-112">[рабочее время](../resources/workinghours.md).</span><span class="sxs-lookup"><span data-stu-id="270dd-112">[working hours](../resources/workinghours.md)</span></span>

<span data-ttu-id="270dd-113">При обновлении предпочтительного формата даты или времени для пользователя укажите его соответственно в [кратком формате даты](/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortDate) или [коротком формате времени](/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortTime) .</span><span class="sxs-lookup"><span data-stu-id="270dd-113">When updating the preferred date or time format for a user, specify it in respectively, the [short date](/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortDate) or [short time](/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortTime) format.</span></span>

<span data-ttu-id="270dd-114">При обновлении предпочтительного часового пояса для пользователя укажите его в формате [часового пояса Windows или Internet Assigned Numbers Authority (IANA)](https://www.iana.org/time-zones) (также известного как часовой пояс Олсона).</span><span class="sxs-lookup"><span data-stu-id="270dd-114">When updating the preferred time zone for a user, specify it in the Windows or [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="270dd-115">Кроме того, можно настроить часовой пояс, как показано в [примере 2](#example-2) ниже.</span><span class="sxs-lookup"><span data-stu-id="270dd-115">You can also further customize the time zone as shown in [example 2](#example-2) below.</span></span>

> [!TIP]
> <span data-ttu-id="270dd-116">Вы не можете создавать или удалять параметры почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="270dd-116">You cannot create or delete any mailbox settings.</span></span>

## <a name="permissions"></a><span data-ttu-id="270dd-117">Разрешения</span><span class="sxs-lookup"><span data-stu-id="270dd-117">Permissions</span></span>
<span data-ttu-id="270dd-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="270dd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="270dd-120">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="270dd-120">Permission type</span></span>      | <span data-ttu-id="270dd-121">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="270dd-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="270dd-122">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="270dd-122">Delegated (work or school account)</span></span> | <span data-ttu-id="270dd-123">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="270dd-123">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="270dd-124">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="270dd-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="270dd-125">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="270dd-125">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="270dd-126">Для приложений</span><span class="sxs-lookup"><span data-stu-id="270dd-126">Application</span></span> | <span data-ttu-id="270dd-127">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="270dd-127">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="270dd-128">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="270dd-128">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailboxSettings
PATCH /users/{id|userPrincipalName}/mailboxSettings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="270dd-129">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="270dd-129">Optional query parameters</span></span>
<span data-ttu-id="270dd-130">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="270dd-130">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="270dd-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="270dd-131">Request headers</span></span>
| <span data-ttu-id="270dd-132">Имя</span><span class="sxs-lookup"><span data-stu-id="270dd-132">Name</span></span>       | <span data-ttu-id="270dd-133">Тип</span><span class="sxs-lookup"><span data-stu-id="270dd-133">Type</span></span> | <span data-ttu-id="270dd-134">Описание</span><span class="sxs-lookup"><span data-stu-id="270dd-134">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="270dd-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="270dd-135">Authorization</span></span>  | <span data-ttu-id="270dd-136">string</span><span class="sxs-lookup"><span data-stu-id="270dd-136">string</span></span>  | <span data-ttu-id="270dd-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="270dd-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="270dd-139">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="270dd-139">Request body</span></span>
<span data-ttu-id="270dd-p105">В тексте запроса укажите значения для соответствующих свойств, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом изменений других значений свойств. Чтобы обеспечить максимальную производительность, не включайте существующие значения, которые не изменились, в запрос. Ниже перечислены свойства, значения которых можно записать или обновить.</span><span class="sxs-lookup"><span data-stu-id="270dd-p105">In the request body, supply the values for the relevant properties that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. The following are the writable/updatable properties:</span></span>

| <span data-ttu-id="270dd-144">Свойство</span><span class="sxs-lookup"><span data-stu-id="270dd-144">Property</span></span>     | <span data-ttu-id="270dd-145">Тип</span><span class="sxs-lookup"><span data-stu-id="270dd-145">Type</span></span>   |<span data-ttu-id="270dd-146">Описание</span><span class="sxs-lookup"><span data-stu-id="270dd-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="270dd-147">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="270dd-147">automaticRepliesSetting</span></span>|[<span data-ttu-id="270dd-148">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="270dd-148">automaticRepliesSetting</span></span>](../resources/automaticrepliessetting.md)|<span data-ttu-id="270dd-149">Параметры конфигурации для автоматического уведомления отправителя о входящем письме с помощью сообщения от пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="270dd-149">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span> <span data-ttu-id="270dd-150">Вы можете настроить такие уведомления только для диапазона дат в будущем.</span><span class="sxs-lookup"><span data-stu-id="270dd-150">You can set such notifications for only a future date range.</span></span>|
|<span data-ttu-id="270dd-151">dateFormat</span><span class="sxs-lookup"><span data-stu-id="270dd-151">dateFormat</span></span>|<span data-ttu-id="270dd-152">string</span><span class="sxs-lookup"><span data-stu-id="270dd-152">string</span></span>|<span data-ttu-id="270dd-153">Формат даты для почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="270dd-153">The date format for the user's mailbox.</span></span>|
|<span data-ttu-id="270dd-154">language</span><span class="sxs-lookup"><span data-stu-id="270dd-154">language</span></span>|[<span data-ttu-id="270dd-155">localeInfo</span><span class="sxs-lookup"><span data-stu-id="270dd-155">localeInfo</span></span>](../resources/localeinfo.md)|<span data-ttu-id="270dd-156">Сведения о языковом стандарте пользователя, в том числе о предпочитаемом языке и стране или регионе.</span><span class="sxs-lookup"><span data-stu-id="270dd-156">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="270dd-157">тимеформат</span><span class="sxs-lookup"><span data-stu-id="270dd-157">timeFormat</span></span>|<span data-ttu-id="270dd-158">string</span><span class="sxs-lookup"><span data-stu-id="270dd-158">string</span></span>|<span data-ttu-id="270dd-159">Формат времени для почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="270dd-159">The time format for the user's mailbox.</span></span>|
|<span data-ttu-id="270dd-160">timeZone</span><span class="sxs-lookup"><span data-stu-id="270dd-160">timeZone</span></span>|<span data-ttu-id="270dd-161">string</span><span class="sxs-lookup"><span data-stu-id="270dd-161">string</span></span>|<span data-ttu-id="270dd-162">Часовой пояс, используемый по умолчанию, для почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="270dd-162">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="270dd-163">workingHours</span><span class="sxs-lookup"><span data-stu-id="270dd-163">workingHours</span></span>|[<span data-ttu-id="270dd-164">workingHours</span><span class="sxs-lookup"><span data-stu-id="270dd-164">workingHours</span></span>](../resources/workinghours.md)|<span data-ttu-id="270dd-165">Часы, дни недели и часовой пояс работы пользователя.</span><span class="sxs-lookup"><span data-stu-id="270dd-165">The hours, days of a week, and time zone that the user works.</span></span>|

## <a name="response"></a><span data-ttu-id="270dd-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="270dd-166">Response</span></span>

<span data-ttu-id="270dd-167">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленные свойства объекта [mailboxSettings](../resources/mailboxsettings.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="270dd-167">If successful, this method returns a `200 OK` response code and the updated properties of a [mailboxSettings](../resources/mailboxsettings.md) object in the response body.</span></span>

## <a name="errors"></a><span data-ttu-id="270dd-168">Ошибки</span><span class="sxs-lookup"><span data-stu-id="270dd-168">Errors</span></span>

<span data-ttu-id="270dd-169">Если заданы недопустимые значения рабочего времени, могут возникать указанные ниже ошибки.</span><span class="sxs-lookup"><span data-stu-id="270dd-169">Setting working hours with inappropriate values may return the following errors.</span></span>

| <span data-ttu-id="270dd-170">Сценарий</span><span class="sxs-lookup"><span data-stu-id="270dd-170">Scenario</span></span>   | <span data-ttu-id="270dd-171">Код состояния HTTP</span><span class="sxs-lookup"><span data-stu-id="270dd-171">HTTP status code</span></span> | <span data-ttu-id="270dd-172">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="270dd-172">Error code</span></span> | <span data-ttu-id="270dd-173">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="270dd-173">Error message</span></span> |
|:-----------|:------|:----------|:----------|
| <span data-ttu-id="270dd-174">Недопустимое значение **startTime** или **endTime**</span><span class="sxs-lookup"><span data-stu-id="270dd-174">Invalid **startTime** or **endTime**</span></span> | <span data-ttu-id="270dd-175">400</span><span class="sxs-lookup"><span data-stu-id="270dd-175">400</span></span> | <span data-ttu-id="270dd-176">RequestBodyRead</span><span class="sxs-lookup"><span data-stu-id="270dd-176">RequestBodyRead</span></span> | <span data-ttu-id="270dd-177">Не удается преобразовать литерал "08" в ожидаемый тип Edm.TimeOfDay.</span><span class="sxs-lookup"><span data-stu-id="270dd-177">Cannot convert the literal '08' to the expected type 'Edm.TimeOfDay'.</span></span>|
| <span data-ttu-id="270dd-178">Время начала больше времени окончания</span><span class="sxs-lookup"><span data-stu-id="270dd-178">Start time is greater than end time</span></span> | <span data-ttu-id="270dd-179">400</span><span class="sxs-lookup"><span data-stu-id="270dd-179">400</span></span> | <span data-ttu-id="270dd-180">ErrorInvalidTimeSettings</span><span class="sxs-lookup"><span data-stu-id="270dd-180">ErrorInvalidTimeSettings</span></span> | <span data-ttu-id="270dd-181">Время начало должно быть раньше, чем время окончания.</span><span class="sxs-lookup"><span data-stu-id="270dd-181">Start Time should occur before End Time.</span></span> |
| <span data-ttu-id="270dd-182">Недопустимый день в свойстве **daysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="270dd-182">Invalid day in **daysOfWeek**</span></span> | <span data-ttu-id="270dd-183">400</span><span class="sxs-lookup"><span data-stu-id="270dd-183">400</span></span> | <span data-ttu-id="270dd-184">InvalidArguments</span><span class="sxs-lookup"><span data-stu-id="270dd-184">InvalidArguments</span></span> | <span data-ttu-id="270dd-185">Запрашиваемое значение RandomDay не найдено.</span><span class="sxs-lookup"><span data-stu-id="270dd-185">Requested value 'RandomDay' was not found.</span></span>|
| <span data-ttu-id="270dd-186">Недопустимое значение **timeZone**</span><span class="sxs-lookup"><span data-stu-id="270dd-186">Invalid **timeZone**</span></span> | <span data-ttu-id="270dd-187">400</span><span class="sxs-lookup"><span data-stu-id="270dd-187">400</span></span> | <span data-ttu-id="270dd-188">InvalidTimeZone</span><span class="sxs-lookup"><span data-stu-id="270dd-188">InvalidTimeZone</span></span> | <span data-ttu-id="270dd-189">Указаны недопустимые параметры часового пояса.</span><span class="sxs-lookup"><span data-stu-id="270dd-189">Time Zone settings provided are invalid.</span></span>|


## <a name="examples"></a><span data-ttu-id="270dd-190">Примеры</span><span class="sxs-lookup"><span data-stu-id="270dd-190">Examples</span></span>
### <a name="example-1"></a><span data-ttu-id="270dd-191">Пример 1</span><span class="sxs-lookup"><span data-stu-id="270dd-191">Example 1</span></span>
#### <a name="request"></a><span data-ttu-id="270dd-192">Запрос</span><span class="sxs-lookup"><span data-stu-id="270dd-192">Request</span></span>
<span data-ttu-id="270dd-193">В первом примере показано, как включить автоматические ответы для диапазона дат, настроив для свойства **automaticRepliesSetting** следующие свойства: **status**, **scheduledStartDateTime** и **scheduledEndDateTime**.</span><span class="sxs-lookup"><span data-stu-id="270dd-193">The first example enables automatic replies for a date range, by setting the following properties of the **automaticRepliesSetting** property: **status**, **scheduledStartDateTime** and **scheduledEndDateTime**.</span></span>


# <a name="http"></a>[<span data-ttu-id="270dd-194">HTTP</span><span class="sxs-lookup"><span data-stu-id="270dd-194">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_mailboxsettings_1"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/mailboxSettings
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/mailboxSettings",
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
# <a name="c"></a>[<span data-ttu-id="270dd-195">C#</span><span class="sxs-lookup"><span data-stu-id="270dd-195">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-mailboxsettings-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="270dd-196">JavaScript</span><span class="sxs-lookup"><span data-stu-id="270dd-196">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-mailboxsettings-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="270dd-197">Objective-C</span><span class="sxs-lookup"><span data-stu-id="270dd-197">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-mailboxsettings-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="270dd-198">Java</span><span class="sxs-lookup"><span data-stu-id="270dd-198">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-mailboxsettings-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="270dd-199">Отклик</span><span class="sxs-lookup"><span data-stu-id="270dd-199">Response</span></span>
<span data-ttu-id="270dd-200">Ответ включает обновленные параметры автоматических ответов.</span><span class="sxs-lookup"><span data-stu-id="270dd-200">The response includes the updated settings for automatic replies.</span></span> <span data-ttu-id="270dd-201">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="270dd-201">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="270dd-202">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="270dd-202">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "update_mailboxsettings_1",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxSettings"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/mailboxSettings",
    "automaticRepliesSetting": {
        "status": "scheduled",
        "externalAudience": "all",
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
    }
}
```

### <a name="example-2"></a><span data-ttu-id="270dd-203">Пример 2</span><span class="sxs-lookup"><span data-stu-id="270dd-203">Example 2</span></span>
#### <a name="request"></a><span data-ttu-id="270dd-204">Запрос</span><span class="sxs-lookup"><span data-stu-id="270dd-204">Request</span></span>
<span data-ttu-id="270dd-205">Во втором примере настраивается часовой пояс для рабочего времени вошедшего пользователя. Для этого в свойстве **timeZone** указывается [пользовательский часовой пояс](../resources/customtimezone.md).</span><span class="sxs-lookup"><span data-stu-id="270dd-205">The second example customizes the time zone for the working hours of the signed-in user, by setting the **timeZone** property to a [custom time zone](../resources/customtimezone.md).</span></span>

<!-- {
  "blockType": "ignored",
  "name": "update_mailboxsettings_2"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/mailboxSettings
Content-Type: application/json

{
  "workingHours": {
      "endTime" : "18:30:00.0000000", 
      "daysOfWeek": [ 
          "Monday", 
          "Tuesday", 
          "Wednesday", 
          "Thursday", 
          "Friday", 
          "Saturday" 
      ], 
      "timeZone" : { 
         "@odata.type": "#microsoft.graph.customTimeZone", 
         "bias":-300, 
         "name": "Customized Time Zone",
         "standardOffset":{   
           "time":"02:00:00.0000000", 
           "dayOccurrence":2, 
           "dayOfWeek":"Sunday", 
           "month":10, 
           "year":0 
         }, 
         "daylightOffset":{   
           "daylightBias":100, 
           "time":"02:00:00.0000000", 
           "dayOccurrence":4, 
           "dayOfWeek":"Sunday", 
           "month":5, 
           "year":0 
         } 
      } 
  }
} 
```
#### <a name="response"></a><span data-ttu-id="270dd-206">Отклик</span><span class="sxs-lookup"><span data-stu-id="270dd-206">Response</span></span>
<span data-ttu-id="270dd-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="270dd-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "update_mailboxsettings_2",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxSettings"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('94447c6e-ea4c-494c-a9ed-d905e366c5cb')/mailboxSettings",
    "workingHours":{
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
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update mailbox settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
