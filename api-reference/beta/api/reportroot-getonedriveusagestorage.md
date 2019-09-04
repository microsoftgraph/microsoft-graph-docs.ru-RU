---
title: 'reportRoot: getOneDriveUsageStorage'
description: Получение сведений о том, как меняется используемый объем хранилища в OneDrive для бизнеса.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: a8f4e5ed3bc333e584b72e2e5a439d750d74dc88
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36725159"
---
# <a name="reportroot-getonedriveusagestorage"></a><span data-ttu-id="90936-103">reportRoot: getOneDriveUsageStorage</span><span class="sxs-lookup"><span data-stu-id="90936-103">reportRoot: getOneDriveUsageStorage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90936-104">Получение сведений о том, как меняется используемый объем хранилища в OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="90936-104">Get the trend on the amount of storage you are using in OneDrive for Business.</span></span>

> <span data-ttu-id="90936-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: использование OneDrive для бизнеса](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span><span class="sxs-lookup"><span data-stu-id="90936-105">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="90936-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="90936-106">Permissions</span></span>

<span data-ttu-id="90936-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90936-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="90936-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="90936-109">Permission type</span></span>                        | <span data-ttu-id="90936-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="90936-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="90936-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="90936-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="90936-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="90936-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="90936-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="90936-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90936-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90936-114">Not supported.</span></span>                           |
| <span data-ttu-id="90936-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="90936-115">Application</span></span>                            | <span data-ttu-id="90936-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="90936-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="90936-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="90936-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageStorage(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="90936-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="90936-118">Function parameters</span></span>

<span data-ttu-id="90936-119">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="90936-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="90936-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="90936-120">Parameter</span></span> | <span data-ttu-id="90936-121">Тип</span><span class="sxs-lookup"><span data-stu-id="90936-121">Type</span></span>   | <span data-ttu-id="90936-122">Описание</span><span class="sxs-lookup"><span data-stu-id="90936-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="90936-123">period</span><span class="sxs-lookup"><span data-stu-id="90936-123">period</span></span>    | <span data-ttu-id="90936-124">string</span><span class="sxs-lookup"><span data-stu-id="90936-124">string</span></span> | <span data-ttu-id="90936-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="90936-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="90936-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="90936-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="90936-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="90936-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="90936-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="90936-128">Required.</span></span> |

<span data-ttu-id="90936-129">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="90936-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="90936-130">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="90936-130">The default output type is text/csv.</span></span> <span data-ttu-id="90936-131">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="90936-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="90936-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="90936-132">Request headers</span></span>

| <span data-ttu-id="90936-133">Имя</span><span class="sxs-lookup"><span data-stu-id="90936-133">Name</span></span>          | <span data-ttu-id="90936-134">Описание</span><span class="sxs-lookup"><span data-stu-id="90936-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="90936-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="90936-135">Authorization</span></span> | <span data-ttu-id="90936-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="90936-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="90936-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="90936-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="90936-139">CSV</span><span class="sxs-lookup"><span data-stu-id="90936-139">CSV</span></span>

<span data-ttu-id="90936-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="90936-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="90936-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="90936-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="90936-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="90936-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="90936-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="90936-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="90936-144">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="90936-144">Report Refresh Date</span></span>
- <span data-ttu-id="90936-145">"Site Type" (Тип сайта);</span><span class="sxs-lookup"><span data-stu-id="90936-145">Site Type</span></span>
- <span data-ttu-id="90936-146">"Storage Used (Byte)" (Используемый объем хранилища в байтах);</span><span class="sxs-lookup"><span data-stu-id="90936-146">Storage Used (Byte)</span></span>
- <span data-ttu-id="90936-147">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="90936-147">Report Date</span></span>
- <span data-ttu-id="90936-148">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="90936-148">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="90936-149">JSON</span><span class="sxs-lookup"><span data-stu-id="90936-149">JSON</span></span>

<span data-ttu-id="90936-150">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[ситеусажестораже](../resources/siteusagestorage.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="90936-150">If successful, this method returns a `200 OK` response code and a **[siteUsageStorage](../resources/siteusagestorage.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90936-151">Пример</span><span class="sxs-lookup"><span data-stu-id="90936-151">Example</span></span>

### <a name="csv"></a><span data-ttu-id="90936-152">CSV</span><span class="sxs-lookup"><span data-stu-id="90936-152">CSV</span></span>

<span data-ttu-id="90936-153">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="90936-153">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="90936-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="90936-154">Request</span></span>

<span data-ttu-id="90936-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="90936-155">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="90936-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="90936-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusagestorage_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageStorage(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="90936-157">C#</span><span class="sxs-lookup"><span data-stu-id="90936-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveusagestorage-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="90936-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="90936-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveusagestorage-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="90936-159">Цель — C</span><span class="sxs-lookup"><span data-stu-id="90936-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveusagestorage-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="90936-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="90936-160">Response</span></span>

<span data-ttu-id="90936-161">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="90936-161">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="90936-162">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="90936-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="90936-163">JSON</span><span class="sxs-lookup"><span data-stu-id="90936-163">JSON</span></span>

<span data-ttu-id="90936-164">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="90936-164">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="90936-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="90936-165">Request</span></span>

<span data-ttu-id="90936-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="90936-166">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="90936-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="90936-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusagestorage_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageStorage(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="90936-168">C#</span><span class="sxs-lookup"><span data-stu-id="90936-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveusagestorage-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="90936-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="90936-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveusagestorage-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="90936-170">Цель — C</span><span class="sxs-lookup"><span data-stu-id="90936-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveusagestorage-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="90936-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="90936-171">Response</span></span>

<span data-ttu-id="90936-172">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="90936-172">The following is an example of the response.</span></span>

> <span data-ttu-id="90936-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="90936-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "storageUsedInBytes": 132654293197, 
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
