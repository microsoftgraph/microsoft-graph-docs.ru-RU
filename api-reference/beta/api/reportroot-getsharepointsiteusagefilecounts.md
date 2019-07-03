---
title: 'reportRoot: getSharePointSiteUsageFileCounts'
description: Узнайте, сколько всего файлов на всех сайтах и сколько из них активны. Файл (пользователь или система) считается активным, если он был сохранен, синхронизирован, изменен или отправлен в указанный период.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 7b7155db0f0fd7d63aab98bda6639dc61b8172a5
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35446684"
---
# <a name="reportroot-getsharepointsiteusagefilecounts"></a><span data-ttu-id="017f5-104">reportRoot: getSharePointSiteUsageFileCounts</span><span class="sxs-lookup"><span data-stu-id="017f5-104">reportRoot: getSharePointSiteUsageFileCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="017f5-105">Узнайте, сколько всего файлов на всех сайтах и сколько из них активны.</span><span class="sxs-lookup"><span data-stu-id="017f5-105">Get the total number of files across all sites and the number of active files.</span></span> <span data-ttu-id="017f5-106">Файл (пользователь или система) считается активным, если он был сохранен, синхронизирован, изменен в указанный период или им поделились в указанный период.</span><span class="sxs-lookup"><span data-stu-id="017f5-106">A file (user or system) is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span>

> <span data-ttu-id="017f5-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: использование сайтов SharePoint](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span><span class="sxs-lookup"><span data-stu-id="017f5-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="017f5-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="017f5-108">Permissions</span></span>

<span data-ttu-id="017f5-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="017f5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="017f5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="017f5-111">Permission type</span></span>                        | <span data-ttu-id="017f5-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="017f5-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="017f5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="017f5-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="017f5-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="017f5-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="017f5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="017f5-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="017f5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="017f5-116">Not supported.</span></span>                           |
| <span data-ttu-id="017f5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="017f5-117">Application</span></span>                            | <span data-ttu-id="017f5-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="017f5-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="017f5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="017f5-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="017f5-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="017f5-120">Function parameters</span></span>

<span data-ttu-id="017f5-121">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="017f5-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="017f5-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="017f5-122">Parameter</span></span> | <span data-ttu-id="017f5-123">Тип</span><span class="sxs-lookup"><span data-stu-id="017f5-123">Type</span></span>   | <span data-ttu-id="017f5-124">Описание</span><span class="sxs-lookup"><span data-stu-id="017f5-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="017f5-125">period</span><span class="sxs-lookup"><span data-stu-id="017f5-125">period</span></span>    | <span data-ttu-id="017f5-126">string</span><span class="sxs-lookup"><span data-stu-id="017f5-126">string</span></span> | <span data-ttu-id="017f5-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="017f5-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="017f5-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="017f5-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="017f5-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="017f5-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="017f5-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="017f5-130">Required.</span></span> |

<span data-ttu-id="017f5-131">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="017f5-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="017f5-132">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="017f5-132">The default output type is text/csv.</span></span> <span data-ttu-id="017f5-133">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="017f5-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="017f5-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="017f5-134">Request headers</span></span>

| <span data-ttu-id="017f5-135">Имя</span><span class="sxs-lookup"><span data-stu-id="017f5-135">Name</span></span>          | <span data-ttu-id="017f5-136">Описание</span><span class="sxs-lookup"><span data-stu-id="017f5-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="017f5-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="017f5-137">Authorization</span></span> | <span data-ttu-id="017f5-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="017f5-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="017f5-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="017f5-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="017f5-141">CSV</span><span class="sxs-lookup"><span data-stu-id="017f5-141">CSV</span></span>

<span data-ttu-id="017f5-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="017f5-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="017f5-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="017f5-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="017f5-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="017f5-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="017f5-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="017f5-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="017f5-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="017f5-146">Report Refresh Date</span></span>
- <span data-ttu-id="017f5-147">"Site Type" (Тип сайта);</span><span class="sxs-lookup"><span data-stu-id="017f5-147">Site Type</span></span>
- <span data-ttu-id="017f5-148">"Total" (Всего);</span><span class="sxs-lookup"><span data-stu-id="017f5-148">Total</span></span>
- <span data-ttu-id="017f5-149">Active (активные)</span><span class="sxs-lookup"><span data-stu-id="017f5-149">Active</span></span>
- <span data-ttu-id="017f5-150">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="017f5-150">Report Date</span></span>
- <span data-ttu-id="017f5-151">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="017f5-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="017f5-152">JSON</span><span class="sxs-lookup"><span data-stu-id="017f5-152">JSON</span></span>

<span data-ttu-id="017f5-153">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[шарепоинтситеусажефилекаунтс](../resources/sharepointsiteusagefilecounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="017f5-153">If successful, this method returns a `200 OK` response code and a **[sharePointSiteUsageFileCounts](../resources/sharepointsiteusagefilecounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="017f5-154">Пример</span><span class="sxs-lookup"><span data-stu-id="017f5-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="017f5-155">CSV</span><span class="sxs-lookup"><span data-stu-id="017f5-155">CSV</span></span>

<span data-ttu-id="017f5-156">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="017f5-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="017f5-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="017f5-157">Request</span></span>

<span data-ttu-id="017f5-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="017f5-158">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="017f5-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="017f5-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagefilecounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageFileCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="017f5-160">C#</span><span class="sxs-lookup"><span data-stu-id="017f5-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointsiteusagefilecounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="017f5-161">Javascript</span><span class="sxs-lookup"><span data-stu-id="017f5-161">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointsiteusagefilecounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="017f5-162">Цель — C</span><span class="sxs-lookup"><span data-stu-id="017f5-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointsiteusagefilecounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="017f5-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="017f5-163">Response</span></span>

<span data-ttu-id="017f5-164">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="017f5-164">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="017f5-165">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="017f5-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Total,Active,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="017f5-166">JSON</span><span class="sxs-lookup"><span data-stu-id="017f5-166">JSON</span></span>

<span data-ttu-id="017f5-167">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="017f5-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="017f5-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="017f5-168">Request</span></span>

<span data-ttu-id="017f5-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="017f5-169">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="017f5-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="017f5-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagefilecounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageFileCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="017f5-171">C#</span><span class="sxs-lookup"><span data-stu-id="017f5-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointsiteusagefilecounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="017f5-172">Javascript</span><span class="sxs-lookup"><span data-stu-id="017f5-172">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointsiteusagefilecounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="017f5-173">Цель — C</span><span class="sxs-lookup"><span data-stu-id="017f5-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointsiteusagefilecounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="017f5-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="017f5-174">Response</span></span>

<span data-ttu-id="017f5-175">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="017f5-175">The following is an example of the response.</span></span>

> <span data-ttu-id="017f5-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="017f5-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointSiteUsageFileCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 255

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.sharePointSiteUsageFileCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteType": "All", 
      "total": 25687, 
      "active": 209, 
      "reportDate": "2017-09-01", 
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
