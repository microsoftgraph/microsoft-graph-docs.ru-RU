---
title: 'reportRoot: getOneDriveUsageAccountDetail'
description: Получите сведения об использовании OneDrive с разбивкой по учетным записям.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: c61edd40172e4f95268efec0fd1ec18aaff56ffb
ms.sourcegitcommit: afea19508ad74a3583b11b5f7b544c53eafb3740
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/22/2019
ms.locfileid: "34344943"
---
# <a name="reportroot-getonedriveusageaccountdetail"></a><span data-ttu-id="c87fb-103">reportRoot: getOneDriveUsageAccountDetail</span><span class="sxs-lookup"><span data-stu-id="c87fb-103">reportRoot: getOneDriveUsageAccountDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c87fb-104">Получите сведения об использовании OneDrive с разбивкой по учетным записям.</span><span class="sxs-lookup"><span data-stu-id="c87fb-104">Get details about OneDrive usage by account.</span></span>

> <span data-ttu-id="c87fb-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span><span class="sxs-lookup"><span data-stu-id="c87fb-105">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="c87fb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c87fb-106">Permissions</span></span>

<span data-ttu-id="c87fb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c87fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c87fb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c87fb-109">Permission type</span></span>                        | <span data-ttu-id="c87fb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c87fb-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="c87fb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c87fb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c87fb-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c87fb-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="c87fb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c87fb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c87fb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c87fb-114">Not supported.</span></span>                           |
| <span data-ttu-id="c87fb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c87fb-115">Application</span></span>                            | <span data-ttu-id="c87fb-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c87fb-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="c87fb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c87fb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageAccountDetail(period='{period_value}')
GET /reports/getOneDriveUsageAccountDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="c87fb-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="c87fb-118">Function parameters</span></span>

<span data-ttu-id="c87fb-119">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="c87fb-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="c87fb-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="c87fb-120">Parameter</span></span> | <span data-ttu-id="c87fb-121">Тип</span><span class="sxs-lookup"><span data-stu-id="c87fb-121">Type</span></span>   | <span data-ttu-id="c87fb-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c87fb-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="c87fb-123">period</span><span class="sxs-lookup"><span data-stu-id="c87fb-123">period</span></span>    | <span data-ttu-id="c87fb-124">string</span><span class="sxs-lookup"><span data-stu-id="c87fb-124">string</span></span> | <span data-ttu-id="c87fb-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="c87fb-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="c87fb-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="c87fb-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="c87fb-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="c87fb-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="c87fb-128">date</span><span class="sxs-lookup"><span data-stu-id="c87fb-128">date</span></span>      | <span data-ttu-id="c87fb-129">Date</span><span class="sxs-lookup"><span data-stu-id="c87fb-129">Date</span></span>   | <span data-ttu-id="c87fb-130">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="c87fb-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="c87fb-131">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="c87fb-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="c87fb-132">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="c87fb-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="c87fb-133">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="c87fb-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="c87fb-134">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c87fb-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="c87fb-135">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="c87fb-135">The default output type is text/csv.</span></span> <span data-ttu-id="c87fb-136">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="c87fb-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c87fb-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c87fb-137">Request headers</span></span>

| <span data-ttu-id="c87fb-138">Имя</span><span class="sxs-lookup"><span data-stu-id="c87fb-138">Name</span></span>          | <span data-ttu-id="c87fb-139">Описание</span><span class="sxs-lookup"><span data-stu-id="c87fb-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="c87fb-140">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c87fb-140">Authorization</span></span> | <span data-ttu-id="c87fb-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c87fb-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="c87fb-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="c87fb-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="c87fb-144">CSV</span><span class="sxs-lookup"><span data-stu-id="c87fb-144">CSV</span></span>

<span data-ttu-id="c87fb-145">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="c87fb-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="c87fb-146">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="c87fb-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="c87fb-147">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="c87fb-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="c87fb-148">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="c87fb-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="c87fb-149">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="c87fb-149">Report Refresh Date</span></span>
- <span data-ttu-id="c87fb-150">"Site URL" (URL-адрес сайта);</span><span class="sxs-lookup"><span data-stu-id="c87fb-150">Site URL</span></span>
- <span data-ttu-id="c87fb-151">"Owner Display Name" (Отображаемое имя владельца);</span><span class="sxs-lookup"><span data-stu-id="c87fb-151">Owner Display Name</span></span>
- <span data-ttu-id="c87fb-152">Is Deleted (удален)</span><span class="sxs-lookup"><span data-stu-id="c87fb-152">Is Deleted</span></span>
- <span data-ttu-id="c87fb-153">"Last Activity Date" (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="c87fb-153">Last Activity Date</span></span>
- <span data-ttu-id="c87fb-154">"File Count" (Количество файлов);</span><span class="sxs-lookup"><span data-stu-id="c87fb-154">File Count</span></span>
- <span data-ttu-id="c87fb-155">Active File Count (количество активных файлов)</span><span class="sxs-lookup"><span data-stu-id="c87fb-155">Active File Count</span></span>
- <span data-ttu-id="c87fb-156">Storage Used (Byte) [использовано (байт)]</span><span class="sxs-lookup"><span data-stu-id="c87fb-156">Storage Used (Byte)</span></span>
- <span data-ttu-id="c87fb-157">"Storage Allocated (Byte)" (Объем выделенного хранилища в байтах);</span><span class="sxs-lookup"><span data-stu-id="c87fb-157">Storage Allocated (Byte)</span></span>
- <span data-ttu-id="c87fb-158">Owner Principal Name (имя участника-владельца)</span><span class="sxs-lookup"><span data-stu-id="c87fb-158">Owner Principal Name</span></span>
- <span data-ttu-id="c87fb-159">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="c87fb-159">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="c87fb-160">JSON</span><span class="sxs-lookup"><span data-stu-id="c87fb-160">JSON</span></span>

<span data-ttu-id="c87fb-161">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[онедривеусажеаккаунтдетаил](../resources/onedriveusageaccountdetail.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c87fb-161">If successful, this method returns a `200 OK` response code and a **[oneDriveUsageAccountDetail](../resources/onedriveusageaccountdetail.md)** object in the response body.</span></span>

<span data-ttu-id="c87fb-162">Размер страницы по умолчанию для этого запроса составляет 200 элементов.</span><span class="sxs-lookup"><span data-stu-id="c87fb-162">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="c87fb-163">Пример</span><span class="sxs-lookup"><span data-stu-id="c87fb-163">Example</span></span>

<span data-ttu-id="c87fb-164">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="c87fb-164">The following is an example that outputs CSV.</span></span>

### <a name="csv"></a><span data-ttu-id="c87fb-165">CSV</span><span class="sxs-lookup"><span data-stu-id="c87fb-165">CSV</span></span>

#### <a name="request"></a><span data-ttu-id="c87fb-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="c87fb-166">Request</span></span>

<span data-ttu-id="c87fb-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c87fb-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="c87fb-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="c87fb-168">Response</span></span>

<span data-ttu-id="c87fb-169">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c87fb-169">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c87fb-170">Образец кода SDK</span><span class="sxs-lookup"><span data-stu-id="c87fb-170">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c87fb-171">C#</span><span class="sxs-lookup"><span data-stu-id="c87fb-171">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveusageaccountdetail_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c87fb-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c87fb-172">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveusageaccountdetail_csv-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="c87fb-173">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="c87fb-173">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site URL,Owner Display Name,Is Deleted,Last Activity Date,File Count,Active File Count,Storage Used (Byte),Storage Allocated (Byte),Owner Principal Name,Report Period
```

### <a name="json"></a><span data-ttu-id="c87fb-174">JSON</span><span class="sxs-lookup"><span data-stu-id="c87fb-174">JSON</span></span>

<span data-ttu-id="c87fb-175">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="c87fb-175">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="c87fb-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="c87fb-176">Request</span></span>

<span data-ttu-id="c87fb-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c87fb-177">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="c87fb-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="c87fb-178">Response</span></span>

<span data-ttu-id="c87fb-179">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c87fb-179">The following is an example of the response.</span></span>

> <span data-ttu-id="c87fb-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c87fb-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oneDriveUsageAccountDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 400

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.oneDriveUsageAccountDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteUrl": "siteUrl-value", 
      "ownerDisplayName": "ownerDisplayName-value", 
      "ownerPrincipalName": "ownerPrincipalName-value", 
      "isDeleted": false, 
      "lastActivityDate": "2017-09-01", 
      "fileCount": 9, 
      "activeFileCount": 5, 
      "storageUsedInBytes": 12190375, 
      "storageAllocatedInBytes": 549755813880, 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c87fb-182">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="c87fb-182">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c87fb-183">C#</span><span class="sxs-lookup"><span data-stu-id="c87fb-183">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveusageaccountdetail_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c87fb-184">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c87fb-184">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveusageaccountdetail_json-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getonedriveusageaccountdetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getonedriveusageaccountdetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getonedriveusageaccountdetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getonedriveusageaccountdetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
