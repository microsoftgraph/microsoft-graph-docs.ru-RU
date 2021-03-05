---
title: Обновление параметров почтового ящика пользователя
description: Обновление одного или нескольких параметров почтового ящика пользователя. Это включает параметры автоматических ответов (оповещать людей автоматически при получении электронной почты), языкового языка (языка и страны/региона), часового пояса и рабочего времени.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f63768297d1930f4a06c82392e66086434f1a484
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475515"
---
# <a name="update-user-mailbox-settings"></a><span data-ttu-id="9d6f7-104">Обновление параметров почтового ящика пользователя</span><span class="sxs-lookup"><span data-stu-id="9d6f7-104">Update user mailbox settings</span></span>

<span data-ttu-id="9d6f7-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d6f7-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9d6f7-106">Включить, настроить или отключить один или несколько следующих параметров в составе почтовых [ящиков пользователя.](../resources/mailboxsettings.md)</span><span class="sxs-lookup"><span data-stu-id="9d6f7-106">Enable, configure, or disable one or more of the following settings as part of a user's [mailboxSettings](../resources/mailboxsettings.md):</span></span>

- <span data-ttu-id="9d6f7-107">[автоматические ответы](../resources/automaticrepliessetting.md) (автоматическое уведомление пользователей при получении их почты);</span><span class="sxs-lookup"><span data-stu-id="9d6f7-107">[automatic replies](../resources/automaticrepliessetting.md) (notify people automatically upon receipt of their email)</span></span>
- <span data-ttu-id="9d6f7-108">dateFormat</span><span class="sxs-lookup"><span data-stu-id="9d6f7-108">dateFormat</span></span>
- <span data-ttu-id="9d6f7-109">delegateMeetingMessageDeliveryOptions</span><span class="sxs-lookup"><span data-stu-id="9d6f7-109">delegateMeetingMessageDeliveryOptions</span></span>
- <span data-ttu-id="9d6f7-110">[языковой стандарт](../resources/localeinfo.md) (язык и страну или регион);</span><span class="sxs-lookup"><span data-stu-id="9d6f7-110">[locale](../resources/localeinfo.md) (language and country/region)</span></span>
- <span data-ttu-id="9d6f7-111">timeFormat</span><span class="sxs-lookup"><span data-stu-id="9d6f7-111">timeFormat</span></span>
- <span data-ttu-id="9d6f7-112">часовой пояс;</span><span class="sxs-lookup"><span data-stu-id="9d6f7-112">time zone</span></span>
- <span data-ttu-id="9d6f7-113">[рабочее время](../resources/workinghours.md).</span><span class="sxs-lookup"><span data-stu-id="9d6f7-113">[working hours](../resources/workinghours.md)</span></span>

<span data-ttu-id="9d6f7-114">При обновлении предпочтительного формата даты или времени для пользователя укажите его соответственно, короткий или [короткий](/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortDate) [формат](/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortTime) времени.</span><span class="sxs-lookup"><span data-stu-id="9d6f7-114">When updating the preferred date or time format for a user, specify it in respectively, the [short date](/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortDate) or [short time](/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortTime) format.</span></span>

<span data-ttu-id="9d6f7-115">При обновлении предпочтительного часового пояса для пользователя укажите его в формате часового пояса Windows или Internet [Assigned Numbers Authority (IANA)](https://www.iana.org/time-zones) (также известного как часовой пояс Olson).</span><span class="sxs-lookup"><span data-stu-id="9d6f7-115">When updating the preferred time zone for a user, specify it in the Windows or [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="9d6f7-116">Вы также можете дополнительно настроить часовой пояс, как показано в [примере 2](#example-2) ниже.</span><span class="sxs-lookup"><span data-stu-id="9d6f7-116">You can also further customize the time zone as shown in [example 2](#example-2) below.</span></span>

> [!TIP]
> <span data-ttu-id="9d6f7-117">Невозможно создать или удалить параметры почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="9d6f7-117">You cannot create or delete any mailbox settings.</span></span>

## <a name="permissions"></a><span data-ttu-id="9d6f7-118">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9d6f7-118">Permissions</span></span>
<span data-ttu-id="9d6f7-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d6f7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d6f7-121">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9d6f7-121">Permission type</span></span>      | <span data-ttu-id="9d6f7-122">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9d6f7-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d6f7-123">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9d6f7-123">Delegated (work or school account)</span></span> | <span data-ttu-id="9d6f7-124">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9d6f7-124">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="9d6f7-125">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9d6f7-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d6f7-126">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9d6f7-126">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="9d6f7-127">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9d6f7-127">Application</span></span> | <span data-ttu-id="9d6f7-128">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9d6f7-128">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d6f7-129">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9d6f7-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailboxSettings
PATCH /users/{id|userPrincipalName}/mailboxSettings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9d6f7-130">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9d6f7-130">Optional query parameters</span></span>
<span data-ttu-id="9d6f7-131">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9d6f7-131">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9d6f7-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9d6f7-132">Request headers</span></span>
| <span data-ttu-id="9d6f7-133">Имя</span><span class="sxs-lookup"><span data-stu-id="9d6f7-133">Name</span></span>       | <span data-ttu-id="9d6f7-134">Тип</span><span class="sxs-lookup"><span data-stu-id="9d6f7-134">Type</span></span> | <span data-ttu-id="9d6f7-135">Описание</span><span class="sxs-lookup"><span data-stu-id="9d6f7-135">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9d6f7-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d6f7-136">Authorization</span></span>  | <span data-ttu-id="9d6f7-137">string</span><span class="sxs-lookup"><span data-stu-id="9d6f7-137">string</span></span>  | <span data-ttu-id="9d6f7-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9d6f7-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9d6f7-140">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9d6f7-140">Request body</span></span>
<span data-ttu-id="9d6f7-p105">В тексте запроса укажите значения для соответствующих свойств, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом изменений других значений свойств. Чтобы обеспечить максимальную производительность, не включайте существующие значения, которые не изменились, в запрос. Ниже перечислены свойства, значения которых можно записать или обновить.</span><span class="sxs-lookup"><span data-stu-id="9d6f7-p105">In the request body, supply the values for the relevant properties that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. The following are the writable/updatable properties:</span></span>

| <span data-ttu-id="9d6f7-145">Свойство</span><span class="sxs-lookup"><span data-stu-id="9d6f7-145">Property</span></span>     | <span data-ttu-id="9d6f7-146">Тип</span><span class="sxs-lookup"><span data-stu-id="9d6f7-146">Type</span></span>   |<span data-ttu-id="9d6f7-147">Описание</span><span class="sxs-lookup"><span data-stu-id="9d6f7-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9d6f7-148">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="9d6f7-148">automaticRepliesSetting</span></span>|[<span data-ttu-id="9d6f7-149">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="9d6f7-149">automaticRepliesSetting</span></span>](../resources/automaticrepliessetting.md)|<span data-ttu-id="9d6f7-150">Параметры конфигурации для автоматического уведомления отправителя о входящем письме с помощью сообщения от пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="9d6f7-150">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span> <span data-ttu-id="9d6f7-151">Такие уведомления можно настроить только для диапазона будущих дат.</span><span class="sxs-lookup"><span data-stu-id="9d6f7-151">You can set such notifications for only a future date range.</span></span>|
|<span data-ttu-id="9d6f7-152">dateFormat</span><span class="sxs-lookup"><span data-stu-id="9d6f7-152">dateFormat</span></span>|<span data-ttu-id="9d6f7-153">string</span><span class="sxs-lookup"><span data-stu-id="9d6f7-153">string</span></span>|<span data-ttu-id="9d6f7-154">Формат даты для почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="9d6f7-154">The date format for the user's mailbox.</span></span>|
|<span data-ttu-id="9d6f7-155">delegateMeetingMessageDeliveryOptions</span><span class="sxs-lookup"><span data-stu-id="9d6f7-155">delegateMeetingMessageDeliveryOptions</span></span>|<span data-ttu-id="9d6f7-156">delegateMeetingMessageDeliveryOptions</span><span class="sxs-lookup"><span data-stu-id="9d6f7-156">delegateMeetingMessageDeliveryOptions</span></span>| <span data-ttu-id="9d6f7-157">Если у пользователя есть делегат календаря, это указывает, получает ли делегат, владелец почтового ящика или как получать сообщения о собраниях, так и ответы на собрания.</span><span class="sxs-lookup"><span data-stu-id="9d6f7-157">If the user has a calendar delegate, this specifies whether the delegate, mailbox owner, or both receive meeting messages and meeting responses.</span></span> <span data-ttu-id="9d6f7-158">Возможные значения: `sendToDelegateAndInformationToPrincipal`, `sendToDelegateAndPrincipal`, `sendToDelegateOnly`.</span><span class="sxs-lookup"><span data-stu-id="9d6f7-158">Possible values are: `sendToDelegateAndInformationToPrincipal`, `sendToDelegateAndPrincipal`, `sendToDelegateOnly`.</span></span>|
|<span data-ttu-id="9d6f7-159">language</span><span class="sxs-lookup"><span data-stu-id="9d6f7-159">language</span></span>|[<span data-ttu-id="9d6f7-160">localeInfo</span><span class="sxs-lookup"><span data-stu-id="9d6f7-160">localeInfo</span></span>](../resources/localeinfo.md)|<span data-ttu-id="9d6f7-161">Сведения о языковом стандарте пользователя, в том числе о предпочитаемом языке и стране или регионе.</span><span class="sxs-lookup"><span data-stu-id="9d6f7-161">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="9d6f7-162">timeFormat</span><span class="sxs-lookup"><span data-stu-id="9d6f7-162">timeFormat</span></span>|<span data-ttu-id="9d6f7-163">string</span><span class="sxs-lookup"><span data-stu-id="9d6f7-163">string</span></span>|<span data-ttu-id="9d6f7-164">Формат времени для почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="9d6f7-164">The time format for the user's mailbox.</span></span>|
|<span data-ttu-id="9d6f7-165">timeZone</span><span class="sxs-lookup"><span data-stu-id="9d6f7-165">timeZone</span></span>|<span data-ttu-id="9d6f7-166">string</span><span class="sxs-lookup"><span data-stu-id="9d6f7-166">string</span></span>|<span data-ttu-id="9d6f7-167">Часовой пояс, используемый по умолчанию, для почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="9d6f7-167">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="9d6f7-168">workingHours</span><span class="sxs-lookup"><span data-stu-id="9d6f7-168">workingHours</span></span>|[<span data-ttu-id="9d6f7-169">workingHours</span><span class="sxs-lookup"><span data-stu-id="9d6f7-169">workingHours</span></span>](../resources/workinghours.md)|<span data-ttu-id="9d6f7-170">Часы, дни недели и часовой пояс работы пользователя.</span><span class="sxs-lookup"><span data-stu-id="9d6f7-170">The hours, days of a week, and time zone that the user works.</span></span>|

## <a name="response"></a><span data-ttu-id="9d6f7-171">Ответ</span><span class="sxs-lookup"><span data-stu-id="9d6f7-171">Response</span></span>

<span data-ttu-id="9d6f7-172">В случае успешной работы этот метод возвращает код ответа и обновленные свойства объекта `200 OK` [mailboxSettings](../resources/mailboxsettings.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9d6f7-172">If successful, this method returns a `200 OK` response code and the updated properties of a [mailboxSettings](../resources/mailboxsettings.md) object in the response body.</span></span>

## <a name="errors"></a><span data-ttu-id="9d6f7-173">Ошибки</span><span class="sxs-lookup"><span data-stu-id="9d6f7-173">Errors</span></span>

<span data-ttu-id="9d6f7-174">Если заданы недопустимые значения рабочего времени, могут возникать указанные ниже ошибки.</span><span class="sxs-lookup"><span data-stu-id="9d6f7-174">Setting working hours with inappropriate values may return the following errors.</span></span>

| <span data-ttu-id="9d6f7-175">Сценарий</span><span class="sxs-lookup"><span data-stu-id="9d6f7-175">Scenario</span></span>   | <span data-ttu-id="9d6f7-176">Код состояния HTTP</span><span class="sxs-lookup"><span data-stu-id="9d6f7-176">HTTP status code</span></span> | <span data-ttu-id="9d6f7-177">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="9d6f7-177">Error code</span></span> | <span data-ttu-id="9d6f7-178">Сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="9d6f7-178">Error message</span></span> |
|:-----------|:------|:----------|:----------|
| <span data-ttu-id="9d6f7-179">Недопустимое значение **startTime** или **endTime**</span><span class="sxs-lookup"><span data-stu-id="9d6f7-179">Invalid **startTime** or **endTime**</span></span> | <span data-ttu-id="9d6f7-180">400</span><span class="sxs-lookup"><span data-stu-id="9d6f7-180">400</span></span> | <span data-ttu-id="9d6f7-181">RequestBodyRead</span><span class="sxs-lookup"><span data-stu-id="9d6f7-181">RequestBodyRead</span></span> | <span data-ttu-id="9d6f7-182">Не удается преобразовать литерал "08" в ожидаемый тип Edm.TimeOfDay.</span><span class="sxs-lookup"><span data-stu-id="9d6f7-182">Cannot convert the literal '08' to the expected type 'Edm.TimeOfDay'.</span></span>|
| <span data-ttu-id="9d6f7-183">Время начала больше времени окончания</span><span class="sxs-lookup"><span data-stu-id="9d6f7-183">Start time is greater than end time</span></span> | <span data-ttu-id="9d6f7-184">400</span><span class="sxs-lookup"><span data-stu-id="9d6f7-184">400</span></span> | <span data-ttu-id="9d6f7-185">ErrorInvalidTimeSettings</span><span class="sxs-lookup"><span data-stu-id="9d6f7-185">ErrorInvalidTimeSettings</span></span> | <span data-ttu-id="9d6f7-186">Время начало должно быть раньше, чем время окончания.</span><span class="sxs-lookup"><span data-stu-id="9d6f7-186">Start Time should occur before End Time.</span></span> |
| <span data-ttu-id="9d6f7-187">Недопустимый день в свойстве **daysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="9d6f7-187">Invalid day in **daysOfWeek**</span></span> | <span data-ttu-id="9d6f7-188">400</span><span class="sxs-lookup"><span data-stu-id="9d6f7-188">400</span></span> | <span data-ttu-id="9d6f7-189">InvalidArguments</span><span class="sxs-lookup"><span data-stu-id="9d6f7-189">InvalidArguments</span></span> | <span data-ttu-id="9d6f7-190">Запрашиваемое значение RandomDay не найдено.</span><span class="sxs-lookup"><span data-stu-id="9d6f7-190">Requested value 'RandomDay' was not found.</span></span>|
| <span data-ttu-id="9d6f7-191">Недопустимое значение **timeZone**</span><span class="sxs-lookup"><span data-stu-id="9d6f7-191">Invalid **timeZone**</span></span> | <span data-ttu-id="9d6f7-192">400</span><span class="sxs-lookup"><span data-stu-id="9d6f7-192">400</span></span> | <span data-ttu-id="9d6f7-193">InvalidTimeZone</span><span class="sxs-lookup"><span data-stu-id="9d6f7-193">InvalidTimeZone</span></span> | <span data-ttu-id="9d6f7-194">Указаны недопустимые параметры часового пояса.</span><span class="sxs-lookup"><span data-stu-id="9d6f7-194">Time Zone settings provided are invalid.</span></span>|


## <a name="examples"></a><span data-ttu-id="9d6f7-195">Примеры</span><span class="sxs-lookup"><span data-stu-id="9d6f7-195">Examples</span></span>
### <a name="example-1"></a><span data-ttu-id="9d6f7-196">Пример 1</span><span class="sxs-lookup"><span data-stu-id="9d6f7-196">Example 1</span></span>
#### <a name="request"></a><span data-ttu-id="9d6f7-197">Запрос</span><span class="sxs-lookup"><span data-stu-id="9d6f7-197">Request</span></span>
<span data-ttu-id="9d6f7-198">В первом примере показано, как включить автоматические ответы для диапазона дат, настроив для свойства **automaticRepliesSetting** следующие свойства: **status**, **scheduledStartDateTime** и **scheduledEndDateTime**.</span><span class="sxs-lookup"><span data-stu-id="9d6f7-198">The first example enables automatic replies for a date range, by setting the following properties of the **automaticRepliesSetting** property: **status**, **scheduledStartDateTime** and **scheduledEndDateTime**.</span></span>


# <a name="http"></a>[<span data-ttu-id="9d6f7-199">HTTP</span><span class="sxs-lookup"><span data-stu-id="9d6f7-199">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="9d6f7-200">C#</span><span class="sxs-lookup"><span data-stu-id="9d6f7-200">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-mailboxsettings-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9d6f7-201">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9d6f7-201">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-mailboxsettings-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9d6f7-202">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9d6f7-202">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-mailboxsettings-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9d6f7-203">Java</span><span class="sxs-lookup"><span data-stu-id="9d6f7-203">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-mailboxsettings-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9d6f7-204">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d6f7-204">Response</span></span>
<span data-ttu-id="9d6f7-205">Ответ включает обновленные параметры автоматических ответов.</span><span class="sxs-lookup"><span data-stu-id="9d6f7-205">The response includes the updated settings for automatic replies.</span></span> <span data-ttu-id="9d6f7-206">Примечание. Представленный здесь объект ответа может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="9d6f7-206">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="9d6f7-207">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9d6f7-207">All of the properties will be returned from an actual call.</span></span>
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

### <a name="example-2"></a><span data-ttu-id="9d6f7-208">Пример 2</span><span class="sxs-lookup"><span data-stu-id="9d6f7-208">Example 2</span></span>
#### <a name="request"></a><span data-ttu-id="9d6f7-209">Запрос</span><span class="sxs-lookup"><span data-stu-id="9d6f7-209">Request</span></span>
<span data-ttu-id="9d6f7-210">Во втором примере настраивается часовой пояс для рабочего времени вошедшего пользователя. Для этого в свойстве **timeZone** указывается [пользовательский часовой пояс](../resources/customtimezone.md).</span><span class="sxs-lookup"><span data-stu-id="9d6f7-210">The second example customizes the time zone for the working hours of the signed-in user, by setting the **timeZone** property to a [custom time zone](../resources/customtimezone.md).</span></span>


# <a name="http"></a>[<span data-ttu-id="9d6f7-211">HTTP</span><span class="sxs-lookup"><span data-stu-id="9d6f7-211">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
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
# <a name="c"></a>[<span data-ttu-id="9d6f7-212">C#</span><span class="sxs-lookup"><span data-stu-id="9d6f7-212">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-mailboxsettings-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9d6f7-213">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9d6f7-213">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-mailboxsettings-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9d6f7-214">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9d6f7-214">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-mailboxsettings-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9d6f7-215">Java</span><span class="sxs-lookup"><span data-stu-id="9d6f7-215">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-mailboxsettings-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="9d6f7-216">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d6f7-216">Response</span></span>
<span data-ttu-id="9d6f7-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9d6f7-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
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
