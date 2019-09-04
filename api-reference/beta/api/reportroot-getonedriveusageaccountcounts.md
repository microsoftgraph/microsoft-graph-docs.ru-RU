---
title: 'reportRoot: getOneDriveUsageAccountCounts'
description: Отслеживайте, как меняется количество активных сайтов OneDrive для бизнеса. Активным считается сайт, на котором пользователи просматривали, изменяли, добавляли, скачивали, отправляли или синхронизировали файлы.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 10c27753ae2a26675381e133494d9fbb01e506ce
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36722974"
---
# <a name="reportroot-getonedriveusageaccountcounts"></a><span data-ttu-id="8e426-104">reportRoot: getOneDriveUsageAccountCounts</span><span class="sxs-lookup"><span data-stu-id="8e426-104">reportRoot: getOneDriveUsageAccountCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e426-105">Отслеживайте, как меняется количество активных сайтов OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="8e426-105">Get the trend in the number of active OneDrive for Business sites.</span></span> <span data-ttu-id="8e426-106">Активным считается сайт, на котором пользователи просматривали, изменяли, добавляли, скачивали, отправляли или синхронизировали файлы.</span><span class="sxs-lookup"><span data-stu-id="8e426-106">Any site on which users viewed, modified, uploaded, downloaded, shared, or synced files is considered an active site.</span></span>

> <span data-ttu-id="8e426-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span><span class="sxs-lookup"><span data-stu-id="8e426-107">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="8e426-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8e426-108">Permissions</span></span>

<span data-ttu-id="8e426-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e426-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8e426-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e426-111">Permission type</span></span>                        | <span data-ttu-id="8e426-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e426-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="8e426-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e426-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="8e426-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8e426-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="8e426-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e426-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e426-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e426-116">Not supported.</span></span>                           |
| <span data-ttu-id="8e426-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8e426-117">Application</span></span>                            | <span data-ttu-id="8e426-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8e426-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="8e426-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e426-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageAccountCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="8e426-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="8e426-120">Function parameters</span></span>

<span data-ttu-id="8e426-121">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="8e426-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="8e426-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="8e426-122">Parameter</span></span> | <span data-ttu-id="8e426-123">Тип</span><span class="sxs-lookup"><span data-stu-id="8e426-123">Type</span></span>   | <span data-ttu-id="8e426-124">Описание</span><span class="sxs-lookup"><span data-stu-id="8e426-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="8e426-125">period</span><span class="sxs-lookup"><span data-stu-id="8e426-125">period</span></span>    | <span data-ttu-id="8e426-126">string</span><span class="sxs-lookup"><span data-stu-id="8e426-126">string</span></span> | <span data-ttu-id="8e426-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="8e426-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="8e426-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="8e426-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="8e426-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="8e426-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="8e426-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8e426-130">Required.</span></span> |

<span data-ttu-id="8e426-131">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="8e426-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="8e426-132">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="8e426-132">The default output type is text/csv.</span></span> <span data-ttu-id="8e426-133">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="8e426-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8e426-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8e426-134">Request headers</span></span>

| <span data-ttu-id="8e426-135">Имя</span><span class="sxs-lookup"><span data-stu-id="8e426-135">Name</span></span>          | <span data-ttu-id="8e426-136">Описание</span><span class="sxs-lookup"><span data-stu-id="8e426-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="8e426-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8e426-137">Authorization</span></span> | <span data-ttu-id="8e426-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8e426-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="8e426-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e426-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="8e426-141">CSV</span><span class="sxs-lookup"><span data-stu-id="8e426-141">CSV</span></span>

<span data-ttu-id="8e426-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="8e426-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="8e426-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="8e426-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="8e426-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="8e426-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="8e426-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="8e426-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="8e426-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="8e426-146">Report Refresh Date</span></span>
- <span data-ttu-id="8e426-147">"Site Type" (Тип сайта);</span><span class="sxs-lookup"><span data-stu-id="8e426-147">Site Type</span></span>
- <span data-ttu-id="8e426-148">"Total" (Всего);</span><span class="sxs-lookup"><span data-stu-id="8e426-148">Total</span></span>
- <span data-ttu-id="8e426-149">Active (активные)</span><span class="sxs-lookup"><span data-stu-id="8e426-149">Active</span></span>
- <span data-ttu-id="8e426-150">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="8e426-150">Report Date</span></span>
- <span data-ttu-id="8e426-151">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="8e426-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="8e426-152">JSON</span><span class="sxs-lookup"><span data-stu-id="8e426-152">JSON</span></span>

<span data-ttu-id="8e426-153">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[онедривеусажеаккаунткаунтс](../resources/onedriveusageaccountcounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8e426-153">If successful, this method returns a `200 OK` response code and a **[oneDriveUsageAccountCounts](../resources/onedriveusageaccountcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e426-154">Пример</span><span class="sxs-lookup"><span data-stu-id="8e426-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="8e426-155">CSV</span><span class="sxs-lookup"><span data-stu-id="8e426-155">CSV</span></span>

<span data-ttu-id="8e426-156">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="8e426-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="8e426-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e426-157">Request</span></span>

<span data-ttu-id="8e426-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e426-158">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8e426-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e426-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountcounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8e426-160">C#</span><span class="sxs-lookup"><span data-stu-id="8e426-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveusageaccountcounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8e426-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e426-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveusageaccountcounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8e426-162">Цель — C</span><span class="sxs-lookup"><span data-stu-id="8e426-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveusageaccountcounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8e426-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e426-163">Response</span></span>

<span data-ttu-id="8e426-164">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8e426-164">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="8e426-165">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="8e426-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="8e426-166">JSON</span><span class="sxs-lookup"><span data-stu-id="8e426-166">JSON</span></span>

<span data-ttu-id="8e426-167">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="8e426-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="8e426-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e426-168">Request</span></span>

<span data-ttu-id="8e426-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e426-169">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8e426-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e426-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountcounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8e426-171">C#</span><span class="sxs-lookup"><span data-stu-id="8e426-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveusageaccountcounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8e426-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e426-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveusageaccountcounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8e426-173">Цель — C</span><span class="sxs-lookup"><span data-stu-id="8e426-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveusageaccountcounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8e426-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e426-174">Response</span></span>

<span data-ttu-id="8e426-175">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8e426-175">The following is an example of the response.</span></span>

> <span data-ttu-id="8e426-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8e426-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oneDriveUsageAccountCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 249

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.oneDriveUsageAccountCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteType": "All", 
      "total": 207, 
      "active": 89, 
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
