---
title: 'reportRoot: getYammerDeviceUsageDistributionUserCounts'
description: Получите сведения о количестве пользователей с разбивкой по типам устройств.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 5dd9011b73bd8bd3905a109d33aac36466b0c1a5
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33639070"
---
# <a name="reportroot-getyammerdeviceusagedistributionusercounts"></a><span data-ttu-id="987ed-103">reportRoot: getYammerDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="987ed-103">reportRoot: getYammerDeviceUsageDistributionUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="987ed-104">Получите сведения о количестве пользователей с разбивкой по типам устройств.</span><span class="sxs-lookup"><span data-stu-id="987ed-104">Get the number of users by device type.</span></span>

> <span data-ttu-id="987ed-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="987ed-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="987ed-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="987ed-106">Permissions</span></span>

<span data-ttu-id="987ed-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="987ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="987ed-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="987ed-109">Permission type</span></span>                        | <span data-ttu-id="987ed-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="987ed-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="987ed-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="987ed-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="987ed-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="987ed-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="987ed-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="987ed-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="987ed-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="987ed-114">Not supported.</span></span>                           |
| <span data-ttu-id="987ed-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="987ed-115">Application</span></span>                            | <span data-ttu-id="987ed-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="987ed-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="987ed-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="987ed-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="987ed-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="987ed-118">Function parameters</span></span>

<span data-ttu-id="987ed-119">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="987ed-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="987ed-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="987ed-120">Parameter</span></span> | <span data-ttu-id="987ed-121">Тип</span><span class="sxs-lookup"><span data-stu-id="987ed-121">Type</span></span>   | <span data-ttu-id="987ed-122">Описание</span><span class="sxs-lookup"><span data-stu-id="987ed-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="987ed-123">period</span><span class="sxs-lookup"><span data-stu-id="987ed-123">period</span></span>    | <span data-ttu-id="987ed-124">string</span><span class="sxs-lookup"><span data-stu-id="987ed-124">string</span></span> | <span data-ttu-id="987ed-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="987ed-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="987ed-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="987ed-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="987ed-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="987ed-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="987ed-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="987ed-128">Required.</span></span> |

<span data-ttu-id="987ed-129">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="987ed-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="987ed-130">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="987ed-130">The default output type is text/csv.</span></span> <span data-ttu-id="987ed-131">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="987ed-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="987ed-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="987ed-132">Request headers</span></span>

| <span data-ttu-id="987ed-133">Имя</span><span class="sxs-lookup"><span data-stu-id="987ed-133">Name</span></span>          | <span data-ttu-id="987ed-134">Описание</span><span class="sxs-lookup"><span data-stu-id="987ed-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="987ed-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="987ed-135">Authorization</span></span> | <span data-ttu-id="987ed-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="987ed-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="987ed-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="987ed-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="987ed-139">CSV</span><span class="sxs-lookup"><span data-stu-id="987ed-139">CSV</span></span>

<span data-ttu-id="987ed-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="987ed-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="987ed-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="987ed-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="987ed-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="987ed-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="987ed-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="987ed-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="987ed-144">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="987ed-144">Report Refresh Date</span></span>
- <span data-ttu-id="987ed-145">"Web" (Интернет);</span><span class="sxs-lookup"><span data-stu-id="987ed-145">Web</span></span>
- <span data-ttu-id="987ed-146">"Windows Phone";</span><span class="sxs-lookup"><span data-stu-id="987ed-146">Windows Phone</span></span>
- <span data-ttu-id="987ed-147">"Android Phone" (Телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="987ed-147">Android Phone</span></span>
- <span data-ttu-id="987ed-148">iPhone</span><span class="sxs-lookup"><span data-stu-id="987ed-148">iPhone</span></span>
- <span data-ttu-id="987ed-149">iPad</span><span class="sxs-lookup"><span data-stu-id="987ed-149">iPad</span></span>
- <span data-ttu-id="987ed-150">Other (другие)</span><span class="sxs-lookup"><span data-stu-id="987ed-150">Other</span></span>
- <span data-ttu-id="987ed-151">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="987ed-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="987ed-152">JSON</span><span class="sxs-lookup"><span data-stu-id="987ed-152">JSON</span></span>

<span data-ttu-id="987ed-153">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[яммердевицеусажедистрибутионусеркаунтс](../resources/yammerdeviceusagedistributionusercounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="987ed-153">If successful, this method returns a `200 OK` response code and a **[yammerDeviceUsageDistributionUserCounts](../resources/yammerdeviceusagedistributionusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="987ed-154">Пример</span><span class="sxs-lookup"><span data-stu-id="987ed-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="987ed-155">CSV</span><span class="sxs-lookup"><span data-stu-id="987ed-155">CSV</span></span>

<span data-ttu-id="987ed-156">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="987ed-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="987ed-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="987ed-157">Request</span></span>

<span data-ttu-id="987ed-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="987ed-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusagedistributionusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="987ed-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="987ed-159">Response</span></span>

<span data-ttu-id="987ed-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="987ed-160">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="987ed-161">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="987ed-161">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="987ed-162">Языках</span><span class="sxs-lookup"><span data-stu-id="987ed-162">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getyammerdeviceusagedistributionusercounts_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="987ed-163">Язык</span><span class="sxs-lookup"><span data-stu-id="987ed-163">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getyammerdeviceusagedistributionusercounts_csv-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="987ed-164">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="987ed-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iPhone,iPad,Other,Report Period
```

### <a name="json"></a><span data-ttu-id="987ed-165">JSON</span><span class="sxs-lookup"><span data-stu-id="987ed-165">JSON</span></span>

<span data-ttu-id="987ed-166">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="987ed-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="987ed-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="987ed-167">Request</span></span>

<span data-ttu-id="987ed-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="987ed-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusagedistributionusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageDistributionUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="987ed-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="987ed-169">Response</span></span>

<span data-ttu-id="987ed-170">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="987ed-170">The following is an example of the response.</span></span>

> <span data-ttu-id="987ed-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="987ed-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerDeviceUsageDistributionUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 271

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerDeviceUsageDistributionUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "web": 138, 
      "windowsPhone": 1, 
      "androidPhone": 29, 
      "iPhone": 40, 
      "iPad": 2, 
      "other": 2, 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="987ed-173">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="987ed-173">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="987ed-174">Языках</span><span class="sxs-lookup"><span data-stu-id="987ed-174">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getyammerdeviceusagedistributionusercounts_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="987ed-175">Язык</span><span class="sxs-lookup"><span data-stu-id="987ed-175">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getyammerdeviceusagedistributionusercounts_json-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/reportroot-getyammerdeviceusagedistributionusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getyammerdeviceusagedistributionusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getyammerdeviceusagedistributionusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getyammerdeviceusagedistributionusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
