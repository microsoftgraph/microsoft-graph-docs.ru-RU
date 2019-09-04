---
title: 'reportRoot: getSharePointSiteUsageDetail'
description: Получение сведений об использовании сайтов SharePoint.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 509fb3944dba760ec80d04d8f005474bff02fdcf
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36722925"
---
# <a name="reportroot-getsharepointsiteusagedetail"></a><span data-ttu-id="a84e1-103">reportRoot: getSharePointSiteUsageDetail</span><span class="sxs-lookup"><span data-stu-id="a84e1-103">reportRoot: getSharePointSiteUsageDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a84e1-104">Получение сведений об использовании сайтов SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a84e1-104">Get details about SharePoint site usage.</span></span>

> <span data-ttu-id="a84e1-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: использование сайтов SharePoint](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span><span class="sxs-lookup"><span data-stu-id="a84e1-105">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="a84e1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a84e1-106">Permissions</span></span>

<span data-ttu-id="a84e1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a84e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a84e1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a84e1-109">Permission type</span></span>                        | <span data-ttu-id="a84e1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a84e1-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="a84e1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a84e1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a84e1-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a84e1-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="a84e1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a84e1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a84e1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a84e1-114">Not supported.</span></span>                           |
| <span data-ttu-id="a84e1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a84e1-115">Application</span></span>                            | <span data-ttu-id="a84e1-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a84e1-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="a84e1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a84e1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageDetail(period='{period_value}')
GET /reports/getSharePointSiteUsageDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="a84e1-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="a84e1-118">Function parameters</span></span>

<span data-ttu-id="a84e1-119">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="a84e1-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="a84e1-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="a84e1-120">Parameter</span></span> | <span data-ttu-id="a84e1-121">Тип</span><span class="sxs-lookup"><span data-stu-id="a84e1-121">Type</span></span>   | <span data-ttu-id="a84e1-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a84e1-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="a84e1-123">period</span><span class="sxs-lookup"><span data-stu-id="a84e1-123">period</span></span>    | <span data-ttu-id="a84e1-124">string</span><span class="sxs-lookup"><span data-stu-id="a84e1-124">string</span></span> | <span data-ttu-id="a84e1-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="a84e1-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="a84e1-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="a84e1-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="a84e1-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="a84e1-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="a84e1-128">date</span><span class="sxs-lookup"><span data-stu-id="a84e1-128">date</span></span>      | <span data-ttu-id="a84e1-129">Date</span><span class="sxs-lookup"><span data-stu-id="a84e1-129">Date</span></span>   | <span data-ttu-id="a84e1-130">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="a84e1-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="a84e1-131">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="a84e1-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="a84e1-132">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="a84e1-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="a84e1-133">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="a84e1-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="a84e1-134">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a84e1-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="a84e1-135">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="a84e1-135">The default output type is text/csv.</span></span> <span data-ttu-id="a84e1-136">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="a84e1-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a84e1-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a84e1-137">Request headers</span></span>

| <span data-ttu-id="a84e1-138">Имя</span><span class="sxs-lookup"><span data-stu-id="a84e1-138">Name</span></span>          | <span data-ttu-id="a84e1-139">Описание</span><span class="sxs-lookup"><span data-stu-id="a84e1-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="a84e1-140">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a84e1-140">Authorization</span></span> | <span data-ttu-id="a84e1-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a84e1-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="a84e1-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="a84e1-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="a84e1-144">CSV</span><span class="sxs-lookup"><span data-stu-id="a84e1-144">CSV</span></span>

<span data-ttu-id="a84e1-145">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="a84e1-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="a84e1-146">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="a84e1-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="a84e1-147">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="a84e1-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="a84e1-148">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="a84e1-148">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="a84e1-149">Report Refresh Date (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="a84e1-149">Report Refresh Date</span></span>
- <span data-ttu-id="a84e1-150">Идентификатор сайта</span><span class="sxs-lookup"><span data-stu-id="a84e1-150">Site Id</span></span>
- <span data-ttu-id="a84e1-151">"Site URL" (URL-адрес сайта);</span><span class="sxs-lookup"><span data-stu-id="a84e1-151">Site URL</span></span>
- <span data-ttu-id="a84e1-152">"Owner Display Name" (Отображаемое имя владельца);</span><span class="sxs-lookup"><span data-stu-id="a84e1-152">Owner Display Name</span></span>
- <span data-ttu-id="a84e1-153">Is Deleted (удален)</span><span class="sxs-lookup"><span data-stu-id="a84e1-153">Is Deleted</span></span>
- <span data-ttu-id="a84e1-154">"Last Activity Date" (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="a84e1-154">Last Activity Date</span></span>
- <span data-ttu-id="a84e1-155">"File Count" (Количество файлов);</span><span class="sxs-lookup"><span data-stu-id="a84e1-155">File Count</span></span>
- <span data-ttu-id="a84e1-156">"Active File Count" (Количество активных файлов);</span><span class="sxs-lookup"><span data-stu-id="a84e1-156">Active File Count</span></span>
- <span data-ttu-id="a84e1-157">"Page View Count" (Количество просмотров страницы);</span><span class="sxs-lookup"><span data-stu-id="a84e1-157">Page View Count</span></span>
- <span data-ttu-id="a84e1-158">"Visited Page Count" (Количество посещенных страниц);</span><span class="sxs-lookup"><span data-stu-id="a84e1-158">Visited Page Count</span></span>
- <span data-ttu-id="a84e1-159">"Storage Used (Byte)" (Используемый объем хранилища в байтах);</span><span class="sxs-lookup"><span data-stu-id="a84e1-159">Storage Used (Byte)</span></span>
- <span data-ttu-id="a84e1-160">"Storage Allocated (Byte)" (Объем выделенного хранилища в байтах);</span><span class="sxs-lookup"><span data-stu-id="a84e1-160">Storage Allocated (Byte)</span></span>
- <span data-ttu-id="a84e1-161">"Root Web Template" (Шаблон корневого веб-сайта);</span><span class="sxs-lookup"><span data-stu-id="a84e1-161">Root Web Template</span></span>
- <span data-ttu-id="a84e1-162">Owner Principal Name (имя участника-владельца)</span><span class="sxs-lookup"><span data-stu-id="a84e1-162">Owner Principal Name</span></span>
- <span data-ttu-id="a84e1-163">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="a84e1-163">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="a84e1-164">JSON</span><span class="sxs-lookup"><span data-stu-id="a84e1-164">JSON</span></span>

<span data-ttu-id="a84e1-165">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[шарепоинтситеусажедетаил](../resources/sharepointsiteusagedetail.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a84e1-165">If successful, this method returns a `200 OK` response code and a **[sharePointSiteUsageDetail](../resources/sharepointsiteusagedetail.md)** object in the response body.</span></span>

<span data-ttu-id="a84e1-166">Размер страницы по умолчанию для этого запроса составляет 200 элементов.</span><span class="sxs-lookup"><span data-stu-id="a84e1-166">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="a84e1-167">Пример</span><span class="sxs-lookup"><span data-stu-id="a84e1-167">Example</span></span>

### <a name="csv"></a><span data-ttu-id="a84e1-168">CSV</span><span class="sxs-lookup"><span data-stu-id="a84e1-168">CSV</span></span>

<span data-ttu-id="a84e1-169">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="a84e1-169">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="a84e1-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="a84e1-170">Request</span></span>

<span data-ttu-id="a84e1-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a84e1-171">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a84e1-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="a84e1-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagedetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a84e1-173">C#</span><span class="sxs-lookup"><span data-stu-id="a84e1-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointsiteusagedetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a84e1-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a84e1-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointsiteusagedetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a84e1-175">Цель — C</span><span class="sxs-lookup"><span data-stu-id="a84e1-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointsiteusagedetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a84e1-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="a84e1-176">Response</span></span>

<span data-ttu-id="a84e1-177">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a84e1-177">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="a84e1-178">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="a84e1-178">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Id,Site URL,Owner Display Name,Is Deleted,Last Activity Date,File Count,Active File Count,Page View Count,Visited Page Count,Storage Used (Byte),Storage Allocated (Byte),Root Web Template,Owner Principal Name,Report Period
```

### <a name="json"></a><span data-ttu-id="a84e1-179">JSON</span><span class="sxs-lookup"><span data-stu-id="a84e1-179">JSON</span></span>

<span data-ttu-id="a84e1-180">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="a84e1-180">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="a84e1-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="a84e1-181">Request</span></span>

<span data-ttu-id="a84e1-182">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a84e1-182">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a84e1-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="a84e1-183">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagedetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a84e1-184">C#</span><span class="sxs-lookup"><span data-stu-id="a84e1-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointsiteusagedetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a84e1-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a84e1-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointsiteusagedetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a84e1-186">Цель — C</span><span class="sxs-lookup"><span data-stu-id="a84e1-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointsiteusagedetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a84e1-187">Отклик</span><span class="sxs-lookup"><span data-stu-id="a84e1-187">Response</span></span>

<span data-ttu-id="a84e1-188">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a84e1-188">The following is an example of the response.</span></span>

> <span data-ttu-id="a84e1-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a84e1-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointSiteUsageDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 484

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.sharePointSiteUsageDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteId": "siteId-value", 
      "siteUrl": "siteUrl-value", 
      "ownerDisplayName": "ownerDisplayName-value", 
      "ownerPrincipalName": "ownerPrincipalName-value", 
      "isDeleted": false, 
      "lastActivityDate": "2017-09-01", 
      "fileCount": 170, 
      "activeFileCount": 25, 
      "pageViewCount": 7, 
      "visitedPageCount": 3, 
      "storageUsedInBytes": 63442116, 
      "storageAllocatedInBytes": 2748779094400, 
      "rootWebTemplate": "Publishing Site", 
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
