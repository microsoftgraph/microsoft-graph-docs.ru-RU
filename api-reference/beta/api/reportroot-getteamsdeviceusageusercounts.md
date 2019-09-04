---
title: 'reportRoot: getTeamsDeviceUsageUserCounts'
description: Получение сведений о количестве уникальных пользователей Microsoft Teams в день с сортировкой по типам устройств.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 320376ecc321cae34c331d6b4fef418abc45ffd3
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36722729"
---
# <a name="reportroot-getteamsdeviceusageusercounts"></a><span data-ttu-id="0801d-103">reportRoot: getTeamsDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="0801d-103">reportRoot: getTeamsDeviceUsageUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0801d-104">Получение сведений о количестве уникальных пользователей Microsoft Teams в день с сортировкой по типам устройств.</span><span class="sxs-lookup"><span data-stu-id="0801d-104">Get the number of Microsoft Teams daily unique users by device type.</span></span>

## <a name="permissions"></a><span data-ttu-id="0801d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0801d-105">Permissions</span></span>

<span data-ttu-id="0801d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0801d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0801d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0801d-108">Permission type</span></span>                        | <span data-ttu-id="0801d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0801d-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="0801d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0801d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0801d-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0801d-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="0801d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0801d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0801d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0801d-113">Not supported.</span></span>                           |
| <span data-ttu-id="0801d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0801d-114">Application</span></span>                            | <span data-ttu-id="0801d-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0801d-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="0801d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0801d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="0801d-117">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="0801d-117">Function parameters</span></span>

<span data-ttu-id="0801d-118">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="0801d-118">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="0801d-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="0801d-119">Parameter</span></span> | <span data-ttu-id="0801d-120">Тип</span><span class="sxs-lookup"><span data-stu-id="0801d-120">Type</span></span>   | <span data-ttu-id="0801d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="0801d-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="0801d-122">period</span><span class="sxs-lookup"><span data-stu-id="0801d-122">period</span></span>    | <span data-ttu-id="0801d-123">string</span><span class="sxs-lookup"><span data-stu-id="0801d-123">string</span></span> | <span data-ttu-id="0801d-124">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="0801d-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="0801d-125">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="0801d-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="0801d-126">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="0801d-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="0801d-127">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0801d-127">Required.</span></span> |

<span data-ttu-id="0801d-128">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="0801d-128">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="0801d-129">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="0801d-129">The default output type is text/csv.</span></span> <span data-ttu-id="0801d-130">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="0801d-130">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0801d-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0801d-131">Request headers</span></span>

| <span data-ttu-id="0801d-132">Имя</span><span class="sxs-lookup"><span data-stu-id="0801d-132">Name</span></span>          | <span data-ttu-id="0801d-133">Описание</span><span class="sxs-lookup"><span data-stu-id="0801d-133">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="0801d-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0801d-134">Authorization</span></span> | <span data-ttu-id="0801d-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0801d-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="0801d-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="0801d-137">Response</span></span>

### <a name="csv"></a><span data-ttu-id="0801d-138">CSV</span><span class="sxs-lookup"><span data-stu-id="0801d-138">CSV</span></span>

<span data-ttu-id="0801d-139">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="0801d-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="0801d-140">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="0801d-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="0801d-141">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="0801d-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="0801d-142">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="0801d-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="0801d-143">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="0801d-143">Report Refresh Date</span></span>
- <span data-ttu-id="0801d-144">"Web" (Интернет);</span><span class="sxs-lookup"><span data-stu-id="0801d-144">Web</span></span>
- <span data-ttu-id="0801d-145">"Windows Phone";</span><span class="sxs-lookup"><span data-stu-id="0801d-145">Windows Phone</span></span>
- <span data-ttu-id="0801d-146">"Android Phone" (Телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="0801d-146">Android Phone</span></span>
- <span data-ttu-id="0801d-147">"iOS";</span><span class="sxs-lookup"><span data-stu-id="0801d-147">iOS</span></span>
- <span data-ttu-id="0801d-148">"Mac";</span><span class="sxs-lookup"><span data-stu-id="0801d-148">Mac</span></span>
- <span data-ttu-id="0801d-149">"Windows";</span><span class="sxs-lookup"><span data-stu-id="0801d-149">Windows</span></span>
- <span data-ttu-id="0801d-150">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="0801d-150">Report Date</span></span>
- <span data-ttu-id="0801d-151">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="0801d-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="0801d-152">JSON</span><span class="sxs-lookup"><span data-stu-id="0801d-152">JSON</span></span>

<span data-ttu-id="0801d-153">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[теамсдевицеусажеусеркаунтс](../resources/teamsdeviceusageusercounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0801d-153">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageUserCounts](../resources/teamsdeviceusageusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0801d-154">Пример</span><span class="sxs-lookup"><span data-stu-id="0801d-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="0801d-155">CSV</span><span class="sxs-lookup"><span data-stu-id="0801d-155">CSV</span></span>

<span data-ttu-id="0801d-156">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="0801d-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="0801d-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="0801d-157">Request</span></span>

<span data-ttu-id="0801d-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0801d-158">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0801d-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="0801d-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0801d-160">C#</span><span class="sxs-lookup"><span data-stu-id="0801d-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsdeviceusageusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0801d-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0801d-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsdeviceusageusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0801d-162">Цель — C</span><span class="sxs-lookup"><span data-stu-id="0801d-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsdeviceusageusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0801d-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="0801d-163">Response</span></span>

<span data-ttu-id="0801d-164">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0801d-164">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="0801d-165">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="0801d-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iOS,Mac,Windows,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="0801d-166">JSON</span><span class="sxs-lookup"><span data-stu-id="0801d-166">JSON</span></span>

<span data-ttu-id="0801d-167">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="0801d-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="0801d-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="0801d-168">Request</span></span>

<span data-ttu-id="0801d-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0801d-169">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0801d-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="0801d-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0801d-171">C#</span><span class="sxs-lookup"><span data-stu-id="0801d-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsdeviceusageusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0801d-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0801d-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsdeviceusageusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0801d-173">Цель — C</span><span class="sxs-lookup"><span data-stu-id="0801d-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsdeviceusageusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0801d-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="0801d-174">Response</span></span>

<span data-ttu-id="0801d-175">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0801d-175">The following is an example of the response.</span></span>

> <span data-ttu-id="0801d-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0801d-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 269

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsDeviceUsageUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "web": 13, 
      "windowsPhone": 0, 
      "androidPhone": 22, 
      "ios": 75, 
      "mac": 16, 
      "windows": 257, 
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
