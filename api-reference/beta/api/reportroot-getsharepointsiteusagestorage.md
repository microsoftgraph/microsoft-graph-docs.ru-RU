---
title: 'reportRoot: getSharePointSiteUsageStorage'
description: Отслеживайте динамику выделенного и использованного объема хранилища за отчетный период.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: de1ec58757f6b2ae11df4ee8dd91aeebcb6ad16e
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33639252"
---
# <a name="reportroot-getsharepointsiteusagestorage"></a><span data-ttu-id="588cc-103">reportRoot: getSharePointSiteUsageStorage</span><span class="sxs-lookup"><span data-stu-id="588cc-103">reportRoot: getSharePointSiteUsageStorage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="588cc-104">Отслеживайте динамику выделенного и использованного объема хранилища за отчетный период.</span><span class="sxs-lookup"><span data-stu-id="588cc-104">Get the trend of storage allocated and consumed during the reporting period.</span></span>

> <span data-ttu-id="588cc-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span><span class="sxs-lookup"><span data-stu-id="588cc-105">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="588cc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="588cc-106">Permissions</span></span>

<span data-ttu-id="588cc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="588cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="588cc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="588cc-109">Permission type</span></span>                        | <span data-ttu-id="588cc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="588cc-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="588cc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="588cc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="588cc-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="588cc-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="588cc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="588cc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="588cc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="588cc-114">Not supported.</span></span>                           |
| <span data-ttu-id="588cc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="588cc-115">Application</span></span>                            | <span data-ttu-id="588cc-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="588cc-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="588cc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="588cc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageStorage(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="588cc-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="588cc-118">Function parameters</span></span>

<span data-ttu-id="588cc-119">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="588cc-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="588cc-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="588cc-120">Parameter</span></span> | <span data-ttu-id="588cc-121">Тип</span><span class="sxs-lookup"><span data-stu-id="588cc-121">Type</span></span>   | <span data-ttu-id="588cc-122">Описание</span><span class="sxs-lookup"><span data-stu-id="588cc-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="588cc-123">period</span><span class="sxs-lookup"><span data-stu-id="588cc-123">period</span></span>    | <span data-ttu-id="588cc-124">string</span><span class="sxs-lookup"><span data-stu-id="588cc-124">string</span></span> | <span data-ttu-id="588cc-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="588cc-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="588cc-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="588cc-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="588cc-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="588cc-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="588cc-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="588cc-128">Required.</span></span> |

<span data-ttu-id="588cc-129">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="588cc-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="588cc-130">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="588cc-130">The default output type is text/csv.</span></span> <span data-ttu-id="588cc-131">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="588cc-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="588cc-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="588cc-132">Request headers</span></span>

| <span data-ttu-id="588cc-133">Имя</span><span class="sxs-lookup"><span data-stu-id="588cc-133">Name</span></span>          | <span data-ttu-id="588cc-134">Описание</span><span class="sxs-lookup"><span data-stu-id="588cc-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="588cc-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="588cc-135">Authorization</span></span> | <span data-ttu-id="588cc-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="588cc-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="588cc-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="588cc-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="588cc-139">CSV</span><span class="sxs-lookup"><span data-stu-id="588cc-139">CSV</span></span>

<span data-ttu-id="588cc-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="588cc-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="588cc-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="588cc-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="588cc-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="588cc-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="588cc-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="588cc-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="588cc-144">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="588cc-144">Report Refresh Date</span></span>
- <span data-ttu-id="588cc-145">"Site Type" (Тип сайта);</span><span class="sxs-lookup"><span data-stu-id="588cc-145">Site Type</span></span>
- <span data-ttu-id="588cc-146">"Storage Used (Byte)" (Используемый объем хранилища в байтах);</span><span class="sxs-lookup"><span data-stu-id="588cc-146">Storage Used (Byte)</span></span>
- <span data-ttu-id="588cc-147">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="588cc-147">Report Date</span></span>
- <span data-ttu-id="588cc-148">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="588cc-148">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="588cc-149">JSON</span><span class="sxs-lookup"><span data-stu-id="588cc-149">JSON</span></span>

<span data-ttu-id="588cc-150">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[ситеусажестораже](../resources/siteusagestorage.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="588cc-150">If successful, this method returns a `200 OK` response code and a **[siteUsageStorage](../resources/siteusagestorage.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="588cc-151">Пример</span><span class="sxs-lookup"><span data-stu-id="588cc-151">Example</span></span>

### <a name="csv"></a><span data-ttu-id="588cc-152">CSV</span><span class="sxs-lookup"><span data-stu-id="588cc-152">CSV</span></span>

<span data-ttu-id="588cc-153">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="588cc-153">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="588cc-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="588cc-154">Request</span></span>

<span data-ttu-id="588cc-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="588cc-155">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagestorage_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageStorage(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="588cc-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="588cc-156">Response</span></span>

<span data-ttu-id="588cc-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="588cc-157">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="588cc-158">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="588cc-158">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="588cc-159">Языках</span><span class="sxs-lookup"><span data-stu-id="588cc-159">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getsharepointsiteusagestorage_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="588cc-160">Язык</span><span class="sxs-lookup"><span data-stu-id="588cc-160">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getsharepointsiteusagestorage_csv-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="588cc-161">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="588cc-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Storage Used (Byte),Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="588cc-162">JSON</span><span class="sxs-lookup"><span data-stu-id="588cc-162">JSON</span></span>

<span data-ttu-id="588cc-163">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="588cc-163">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="588cc-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="588cc-164">Request</span></span>

<span data-ttu-id="588cc-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="588cc-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagestorage_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageStorage(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="588cc-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="588cc-166">Response</span></span>

<span data-ttu-id="588cc-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="588cc-167">The following is an example of the response.</span></span>

> <span data-ttu-id="588cc-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="588cc-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.siteUsageStorage"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 248

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.siteUsageStorage)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteType": "All", 
      "storageUsedInBytes": 171835798971, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="588cc-170">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="588cc-170">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="588cc-171">Языках</span><span class="sxs-lookup"><span data-stu-id="588cc-171">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getsharepointsiteusagestorage_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="588cc-172">Язык</span><span class="sxs-lookup"><span data-stu-id="588cc-172">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getsharepointsiteusagestorage_json-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/reportroot-getsharepointsiteusagestorage.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getsharepointsiteusagestorage.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getsharepointsiteusagestorage.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getsharepointsiteusagestorage.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
