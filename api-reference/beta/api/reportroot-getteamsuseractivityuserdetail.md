---
title: 'reportRoot: getTeamsUserActivityUserDetail'
description: Получение сведений о действиях отдельных пользователей Microsoft Teams.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: faf4ce624c745b388c87449b142af0dd11bb9ee2
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054996"
---
# <a name="reportroot-getteamsuseractivityuserdetail"></a><span data-ttu-id="53430-103">reportRoot: getTeamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="53430-103">reportRoot: getTeamsUserActivityUserDetail</span></span>

<span data-ttu-id="53430-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53430-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53430-105">Получение сведения о действиях отдельных пользователей Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="53430-105">Get details about Microsoft Teams user activity by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="53430-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="53430-106">Permissions</span></span>

<span data-ttu-id="53430-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53430-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="53430-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="53430-109">Permission type</span></span>                        | <span data-ttu-id="53430-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="53430-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="53430-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="53430-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="53430-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="53430-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="53430-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="53430-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53430-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53430-114">Not supported.</span></span>                           |
| <span data-ttu-id="53430-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="53430-115">Application</span></span>                            | <span data-ttu-id="53430-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="53430-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="53430-117">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="53430-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="53430-118">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="53430-118">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="53430-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="53430-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserDetail(period='D7')
GET /reports/getTeamsUserActivityUserDetail(date=2017-09-01)
```

## <a name="function-parameters"></a><span data-ttu-id="53430-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="53430-120">Function parameters</span></span>

<span data-ttu-id="53430-121">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="53430-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="53430-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="53430-122">Parameter</span></span> | <span data-ttu-id="53430-123">Тип</span><span class="sxs-lookup"><span data-stu-id="53430-123">Type</span></span>   | <span data-ttu-id="53430-124">Описание</span><span class="sxs-lookup"><span data-stu-id="53430-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="53430-125">period</span><span class="sxs-lookup"><span data-stu-id="53430-125">period</span></span>    | <span data-ttu-id="53430-126">string</span><span class="sxs-lookup"><span data-stu-id="53430-126">string</span></span> | <span data-ttu-id="53430-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="53430-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="53430-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="53430-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="53430-129">Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="53430-129">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="53430-130">date</span><span class="sxs-lookup"><span data-stu-id="53430-130">date</span></span>      | <span data-ttu-id="53430-131">Date</span><span class="sxs-lookup"><span data-stu-id="53430-131">Date</span></span>   | <span data-ttu-id="53430-132">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="53430-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="53430-133">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="53430-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="53430-134">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="53430-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="53430-135">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="53430-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="53430-136">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="53430-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="53430-137">Тип вывода по умолчанию — текст/csv.</span><span class="sxs-lookup"><span data-stu-id="53430-137">The default output type is text/csv.</span></span> <span data-ttu-id="53430-138">Однако, если требуется указать тип вывода, можно использовать параметр OData $format для параметра text/csv или application/json.</span><span class="sxs-lookup"><span data-stu-id="53430-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="53430-139">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="53430-139">Request headers</span></span>

| <span data-ttu-id="53430-140">Имя</span><span class="sxs-lookup"><span data-stu-id="53430-140">Name</span></span>          | <span data-ttu-id="53430-141">Описание</span><span class="sxs-lookup"><span data-stu-id="53430-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="53430-142">Авторизация</span><span class="sxs-lookup"><span data-stu-id="53430-142">Authorization</span></span> | <span data-ttu-id="53430-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="53430-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="53430-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="53430-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="53430-146">CSV</span><span class="sxs-lookup"><span data-stu-id="53430-146">CSV</span></span>

<span data-ttu-id="53430-147">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="53430-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="53430-148">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="53430-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="53430-149">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="53430-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="53430-150">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="53430-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="53430-151">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="53430-151">Report Refresh Date</span></span>
- <span data-ttu-id="53430-152">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="53430-152">User Principal Name</span></span>
- <span data-ttu-id="53430-153">Last Activity Date (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="53430-153">Last Activity Date</span></span>
- <span data-ttu-id="53430-154">Is Deleted (Удален);</span><span class="sxs-lookup"><span data-stu-id="53430-154">Is Deleted</span></span>
- <span data-ttu-id="53430-155">Deleted Date (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="53430-155">Deleted Date</span></span>
- <span data-ttu-id="53430-156">Assigned Products (Назначенные продукты);</span><span class="sxs-lookup"><span data-stu-id="53430-156">Assigned Products</span></span>
- <span data-ttu-id="53430-157">Team Chat Messages Count (Количество сообщений в чатах групп);</span><span class="sxs-lookup"><span data-stu-id="53430-157">Team Chat Message Count</span></span>
- <span data-ttu-id="53430-158">Private Chat Message Count (Количество сообщений в приватных чатах);</span><span class="sxs-lookup"><span data-stu-id="53430-158">Private Chat Message Count</span></span>
- <span data-ttu-id="53430-159">Call Count (Количество звонков);</span><span class="sxs-lookup"><span data-stu-id="53430-159">Call Count</span></span>
- <span data-ttu-id="53430-160">Meeting Count (Количество собраний);</span><span class="sxs-lookup"><span data-stu-id="53430-160">Meeting Count</span></span>
- <span data-ttu-id="53430-161">Организованный подсчет собраний</span><span class="sxs-lookup"><span data-stu-id="53430-161">Meetings Organized Count</span></span>
- <span data-ttu-id="53430-162">Собрания, на которые было посчитано</span><span class="sxs-lookup"><span data-stu-id="53430-162">Meetings Attended Count</span></span>
- <span data-ttu-id="53430-163">Ad Hoc Meetings Organized Count</span><span class="sxs-lookup"><span data-stu-id="53430-163">Ad Hoc Meetings Organized Count</span></span>
- <span data-ttu-id="53430-164">Ad Hoc Meetings Attended Count</span><span class="sxs-lookup"><span data-stu-id="53430-164">Ad Hoc Meetings Attended Count</span></span>
- <span data-ttu-id="53430-165">Запланированный разовый подсчет собраний</span><span class="sxs-lookup"><span data-stu-id="53430-165">Scheduled One-time Meetings Organized Count</span></span>
- <span data-ttu-id="53430-166">Плановые одновековые собрания, на которые присутствовало количество</span><span class="sxs-lookup"><span data-stu-id="53430-166">Scheduled One-time Meetings Attended Count</span></span>
- <span data-ttu-id="53430-167">Запланированные повторные собрания Организованный подсчет</span><span class="sxs-lookup"><span data-stu-id="53430-167">Scheduled Recurring Meetings Organized Count</span></span>
- <span data-ttu-id="53430-168">Запланированные повторяющиеся собрания, на которые присутствовало количество</span><span class="sxs-lookup"><span data-stu-id="53430-168">Scheduled Recurring Meetings Attended Count</span></span>
- <span data-ttu-id="53430-169">Продолжительность звука</span><span class="sxs-lookup"><span data-stu-id="53430-169">Audio Duration</span></span>
- <span data-ttu-id="53430-170">Длительность видео</span><span class="sxs-lookup"><span data-stu-id="53430-170">Video Duration</span></span>
- <span data-ttu-id="53430-171">Продолжительность обмена экранами</span><span class="sxs-lookup"><span data-stu-id="53430-171">Screen Share Duration</span></span>
- <span data-ttu-id="53430-172">Продолжительность звука в секундах</span><span class="sxs-lookup"><span data-stu-id="53430-172">Audio Duration In Seconds</span></span>
- <span data-ttu-id="53430-173">Длительность видео в секундах</span><span class="sxs-lookup"><span data-stu-id="53430-173">Video Duration In Seconds</span></span>
- <span data-ttu-id="53430-174">Продолжительность обмена экрана в секундах</span><span class="sxs-lookup"><span data-stu-id="53430-174">Screen Share Duration In Seconds</span></span>
- <span data-ttu-id="53430-175">Has Other Action (Есть другое действие);</span><span class="sxs-lookup"><span data-stu-id="53430-175">Has Other Action</span></span>
- <span data-ttu-id="53430-176">Лицензировано</span><span class="sxs-lookup"><span data-stu-id="53430-176">Is Licensed</span></span>
- <span data-ttu-id="53430-177">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="53430-177">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="53430-178">JSON</span><span class="sxs-lookup"><span data-stu-id="53430-178">JSON</span></span>

<span data-ttu-id="53430-179">В случае успешной работы этот метод возвращает код ответа и `200 OK` **[объект teamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md)** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="53430-179">If successful, this method returns a `200 OK` response code and a **[teamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="53430-180">Размер страницы по умолчанию для этого запроса — 2000 элементов.</span><span class="sxs-lookup"><span data-stu-id="53430-180">The default page size for this request is 2000 items.</span></span>

## <a name="example"></a><span data-ttu-id="53430-181">Пример</span><span class="sxs-lookup"><span data-stu-id="53430-181">Example</span></span>

### <a name="csv"></a><span data-ttu-id="53430-182">CSV</span><span class="sxs-lookup"><span data-stu-id="53430-182">CSV</span></span>

<span data-ttu-id="53430-183">Ниже приводится пример, который выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="53430-183">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="53430-184">Запрос</span><span class="sxs-lookup"><span data-stu-id="53430-184">Request</span></span>

<span data-ttu-id="53430-185">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="53430-185">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivityuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserDetail(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="53430-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="53430-186">Response</span></span>

<span data-ttu-id="53430-187">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="53430-187">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="53430-188">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="53430-188">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Is Deleted,Deleted Date,Assigned Products,Team Chat Message Count,Private Chat Message Count,Call Count,Meeting Count,Meetings Organized Count,Meetings Attended Count,Ad Hoc Meetings Organized Count,Ad Hoc Meetings Attended Count,Scheduled One-time Meetings Organized Count,Scheduled One-time Meetings Attended Count,Scheduled Recurring Meetings Organized Count,Scheduled Recurring Meetings Attended Count,Audio Duration,Video Duration,Screen Share Duration,Audio Duration In Seconds,Video Duration In Seconds,Screen Share Duration In Seconds,Has Other Action,Is Licensed,Report Period
```

### <a name="json"></a><span data-ttu-id="53430-189">JSON</span><span class="sxs-lookup"><span data-stu-id="53430-189">JSON</span></span>

<span data-ttu-id="53430-190">Ниже приводится пример, который возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="53430-190">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="53430-191">Запрос</span><span class="sxs-lookup"><span data-stu-id="53430-191">Request</span></span>

<span data-ttu-id="53430-192">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="53430-192">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivityuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserDetail(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="53430-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="53430-193">Response</span></span>

<span data-ttu-id="53430-194">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="53430-194">The following is an example of the response.</span></span>

> <span data-ttu-id="53430-195">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="53430-195">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsUserActivityUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 452

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsUserActivityUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "isLicensed": true, 
      "lastActivityDate": "2017-09-01", 
      "isDeleted": false, 
      "deletedDate": null, 
      "assignedProducts": [
        "Microsoft 365 ENTERPRISE E5"
      ], 
      "teamChatMessageCount": 0, 
      "privateChatMessageCount": 49, 
      "callCount": 2, 
      "meetingCount": 0, 
      "meetingsOrganizedCount": 0, 
      "meetingsAttendedCount": 0, 
      "adHocMeetingsOrganizedCount": 0, 
      "adHocMeetingsAttendedCount": 0, 
      "scheduledOneTimeMeetingsOrganizedCount": 0, 
      "scheduledOneTimeMeetingsAttendedCount": 0, 
      "scheduledRecurringMeetingsOrganizedCount": 0, 
      "scheduledRecurringMeetingsAttendedCount": 0, 
      "audioDuration": 00:00:00, 
      "videoDuration": 00:00:00, 
      "screenShareDuration": 00:00:00, 
      "hasOtherAction": true, 
      "reportPeriod": "7"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


