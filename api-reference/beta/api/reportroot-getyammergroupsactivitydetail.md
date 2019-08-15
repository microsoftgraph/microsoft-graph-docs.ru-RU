---
title: 'reportRoot: getYammerGroupsActivityDetail'
description: Получите сведения об активности в группах Yammer.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 85368416acae9a0a55dde1a9c57ad483b7be5e0c
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36410985"
---
# <a name="reportroot-getyammergroupsactivitydetail"></a><span data-ttu-id="029d8-103">reportRoot: getYammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="029d8-103">reportRoot: getYammerGroupsActivityDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="029d8-104">Получите сведения об активности в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="029d8-104">Get details about Yammer groups activity by group.</span></span>

> <span data-ttu-id="029d8-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span><span class="sxs-lookup"><span data-stu-id="029d8-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="029d8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="029d8-106">Permissions</span></span>

<span data-ttu-id="029d8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="029d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="029d8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="029d8-109">Permission type</span></span>                        | <span data-ttu-id="029d8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="029d8-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="029d8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="029d8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="029d8-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="029d8-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="029d8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="029d8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="029d8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="029d8-114">Not supported.</span></span>                           |
| <span data-ttu-id="029d8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="029d8-115">Application</span></span>                            | <span data-ttu-id="029d8-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="029d8-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="029d8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="029d8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityDetail(period='{period_value}')
GET /reports/getYammerGroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="029d8-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="029d8-118">Function parameters</span></span>

<span data-ttu-id="029d8-119">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="029d8-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="029d8-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="029d8-120">Parameter</span></span> | <span data-ttu-id="029d8-121">Тип</span><span class="sxs-lookup"><span data-stu-id="029d8-121">Type</span></span>   | <span data-ttu-id="029d8-122">Описание</span><span class="sxs-lookup"><span data-stu-id="029d8-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="029d8-123">period</span><span class="sxs-lookup"><span data-stu-id="029d8-123">period</span></span>    | <span data-ttu-id="029d8-124">string</span><span class="sxs-lookup"><span data-stu-id="029d8-124">string</span></span> | <span data-ttu-id="029d8-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="029d8-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="029d8-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="029d8-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="029d8-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="029d8-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="029d8-128">date</span><span class="sxs-lookup"><span data-stu-id="029d8-128">date</span></span>      | <span data-ttu-id="029d8-129">Date</span><span class="sxs-lookup"><span data-stu-id="029d8-129">Date</span></span>   | <span data-ttu-id="029d8-130">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="029d8-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="029d8-131">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="029d8-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="029d8-132">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="029d8-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="029d8-133">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="029d8-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="029d8-134">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="029d8-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="029d8-135">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="029d8-135">The default output type is text/csv.</span></span> <span data-ttu-id="029d8-136">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="029d8-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="029d8-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="029d8-137">Request headers</span></span>

| <span data-ttu-id="029d8-138">Имя</span><span class="sxs-lookup"><span data-stu-id="029d8-138">Name</span></span>          | <span data-ttu-id="029d8-139">Описание</span><span class="sxs-lookup"><span data-stu-id="029d8-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="029d8-140">Авторизация</span><span class="sxs-lookup"><span data-stu-id="029d8-140">Authorization</span></span> | <span data-ttu-id="029d8-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="029d8-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="029d8-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="029d8-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="029d8-144">CSV</span><span class="sxs-lookup"><span data-stu-id="029d8-144">CSV</span></span>

<span data-ttu-id="029d8-145">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="029d8-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="029d8-146">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="029d8-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="029d8-147">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="029d8-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="029d8-148">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="029d8-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="029d8-149">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="029d8-149">Report Refresh Date</span></span>
- <span data-ttu-id="029d8-150">Group Display Name (отображаемое имя группы)</span><span class="sxs-lookup"><span data-stu-id="029d8-150">Group Display Name</span></span>
- <span data-ttu-id="029d8-151">Is Deleted (удален)</span><span class="sxs-lookup"><span data-stu-id="029d8-151">Is Deleted</span></span>
- <span data-ttu-id="029d8-152">Owner Principal Name (имя участника-владельца)</span><span class="sxs-lookup"><span data-stu-id="029d8-152">Owner Principal Name</span></span>
- <span data-ttu-id="029d8-153">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="029d8-153">Last Activity Date</span></span>
- <span data-ttu-id="029d8-154">Group Type (тип группы)</span><span class="sxs-lookup"><span data-stu-id="029d8-154">Group Type</span></span>
- <span data-ttu-id="029d8-155">Office 365 Connected (подключены к Office 365)</span><span class="sxs-lookup"><span data-stu-id="029d8-155">Office 365 Connected</span></span>
- <span data-ttu-id="029d8-156">Member Count (количество участников)</span><span class="sxs-lookup"><span data-stu-id="029d8-156">Member Count</span></span>
- <span data-ttu-id="029d8-157">Posted Count (количество опубликованных сообщений)</span><span class="sxs-lookup"><span data-stu-id="029d8-157">Posted Count</span></span>
- <span data-ttu-id="029d8-158">Read Count (количество прочитанных сообщений)</span><span class="sxs-lookup"><span data-stu-id="029d8-158">Read Count</span></span>
- <span data-ttu-id="029d8-159">Liked Count (количество понравившихся сообщений)</span><span class="sxs-lookup"><span data-stu-id="029d8-159">Liked Count</span></span>
- <span data-ttu-id="029d8-160">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="029d8-160">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="029d8-161">JSON</span><span class="sxs-lookup"><span data-stu-id="029d8-161">JSON</span></span>

<span data-ttu-id="029d8-162">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[яммерграупсактивитидетаил](../resources/yammergroupsactivitydetail.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="029d8-162">If successful, this method returns a `200 OK` response code and a **[yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md)** object in the response body.</span></span>

<span data-ttu-id="029d8-163">Размер страницы по умолчанию для этого запроса составляет 200 элементов.</span><span class="sxs-lookup"><span data-stu-id="029d8-163">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="029d8-164">Пример</span><span class="sxs-lookup"><span data-stu-id="029d8-164">Example</span></span>

### <a name="csv"></a><span data-ttu-id="029d8-165">CSV</span><span class="sxs-lookup"><span data-stu-id="029d8-165">CSV</span></span>

<span data-ttu-id="029d8-166">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="029d8-166">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="029d8-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="029d8-167">Request</span></span>

<span data-ttu-id="029d8-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="029d8-168">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="029d8-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="029d8-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitydetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="029d8-170">C#</span><span class="sxs-lookup"><span data-stu-id="029d8-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammergroupsactivitydetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="029d8-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="029d8-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammergroupsactivitydetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="029d8-172">Цель — C</span><span class="sxs-lookup"><span data-stu-id="029d8-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammergroupsactivitydetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="029d8-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="029d8-173">Response</span></span>

<span data-ttu-id="029d8-174">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="029d8-174">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="029d8-175">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="029d8-175">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Group Display Name,Is Deleted,Owner Principal Name,Last Activity Date,Group Type,Office 365 Connected,Member Count,Posted Count,Read Count,Liked Count,Report Period
```

### <a name="json"></a><span data-ttu-id="029d8-176">JSON</span><span class="sxs-lookup"><span data-stu-id="029d8-176">JSON</span></span>

<span data-ttu-id="029d8-177">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="029d8-177">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="029d8-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="029d8-178">Request</span></span>

<span data-ttu-id="029d8-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="029d8-179">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="029d8-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="029d8-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitydetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="029d8-181">C#</span><span class="sxs-lookup"><span data-stu-id="029d8-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammergroupsactivitydetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="029d8-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="029d8-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammergroupsactivitydetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="029d8-183">Цель — C</span><span class="sxs-lookup"><span data-stu-id="029d8-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammergroupsactivitydetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="029d8-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="029d8-184">Response</span></span>

<span data-ttu-id="029d8-185">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="029d8-185">The following is an example of the response.</span></span>

> <span data-ttu-id="029d8-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="029d8-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerGroupsActivityDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 441

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerGroupsActivityDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "groupDisplayName": "groupDisplayName-value", 
      "isDeleted": false, 
      "ownerPrincipalName": "ownerPrincipalName-value", 
      "lastActivityDate": "2017-08-30", 
      "groupType": "private", 
      "office365Connected": true, 
      "memberCount": 176, 
      "postedCount": 15, 
      "readCount": 24, 
      "likedCount": 3, 
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
