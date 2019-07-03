---
title: 'reportRoot: getTeamsDeviceUsageDistributionUserCounts'
description: Получение количества уникальных пользователей Microsoft Teams с сортировкой по типам устройств за выбранный период.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 316d785d920f138b5e409ece2a5d2fbeda71f7aa
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35446404"
---
# <a name="reportroot-getteamsdeviceusagedistributionusercounts"></a><span data-ttu-id="82c2f-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="82c2f-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82c2f-104">Получение количества уникальных пользователей Microsoft Teams с сортировкой по типам устройств за выбранный период.</span><span class="sxs-lookup"><span data-stu-id="82c2f-104">Get the number of Microsoft Teams unique users by device type over the selected time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="82c2f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="82c2f-105">Permissions</span></span>

<span data-ttu-id="82c2f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82c2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="82c2f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="82c2f-108">Permission type</span></span>                        | <span data-ttu-id="82c2f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="82c2f-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="82c2f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="82c2f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="82c2f-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="82c2f-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="82c2f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="82c2f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82c2f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82c2f-113">Not supported.</span></span>                           |
| <span data-ttu-id="82c2f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="82c2f-114">Application</span></span>                            | <span data-ttu-id="82c2f-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="82c2f-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="82c2f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="82c2f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="82c2f-117">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="82c2f-117">Function parameters</span></span>

<span data-ttu-id="82c2f-118">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="82c2f-118">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="82c2f-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="82c2f-119">Parameter</span></span> | <span data-ttu-id="82c2f-120">Тип</span><span class="sxs-lookup"><span data-stu-id="82c2f-120">Type</span></span>   | <span data-ttu-id="82c2f-121">Описание</span><span class="sxs-lookup"><span data-stu-id="82c2f-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="82c2f-122">period</span><span class="sxs-lookup"><span data-stu-id="82c2f-122">period</span></span>    | <span data-ttu-id="82c2f-123">string</span><span class="sxs-lookup"><span data-stu-id="82c2f-123">string</span></span> | <span data-ttu-id="82c2f-124">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="82c2f-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="82c2f-125">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="82c2f-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="82c2f-126">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="82c2f-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="82c2f-127">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="82c2f-127">Required.</span></span> |

<span data-ttu-id="82c2f-128">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="82c2f-128">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="82c2f-129">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="82c2f-129">The default output type is text/csv.</span></span> <span data-ttu-id="82c2f-130">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="82c2f-130">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="82c2f-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="82c2f-131">Request headers</span></span>

| <span data-ttu-id="82c2f-132">Имя</span><span class="sxs-lookup"><span data-stu-id="82c2f-132">Name</span></span>          | <span data-ttu-id="82c2f-133">Описание</span><span class="sxs-lookup"><span data-stu-id="82c2f-133">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="82c2f-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="82c2f-134">Authorization</span></span> | <span data-ttu-id="82c2f-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="82c2f-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="82c2f-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="82c2f-137">Response</span></span>

### <a name="csv"></a><span data-ttu-id="82c2f-138">CSV</span><span class="sxs-lookup"><span data-stu-id="82c2f-138">CSV</span></span>

<span data-ttu-id="82c2f-139">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="82c2f-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="82c2f-140">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="82c2f-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="82c2f-141">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="82c2f-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="82c2f-142">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="82c2f-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="82c2f-143">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="82c2f-143">Report Refresh Date</span></span>
- <span data-ttu-id="82c2f-144">"Web" (Интернет);</span><span class="sxs-lookup"><span data-stu-id="82c2f-144">Web</span></span>
- <span data-ttu-id="82c2f-145">"Windows Phone";</span><span class="sxs-lookup"><span data-stu-id="82c2f-145">Windows Phone</span></span>
- <span data-ttu-id="82c2f-146">"Android Phone" (Телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="82c2f-146">Android Phone</span></span>
- <span data-ttu-id="82c2f-147">"iOS";</span><span class="sxs-lookup"><span data-stu-id="82c2f-147">iOS</span></span>
- <span data-ttu-id="82c2f-148">"Mac";</span><span class="sxs-lookup"><span data-stu-id="82c2f-148">Mac</span></span>
- <span data-ttu-id="82c2f-149">"Windows";</span><span class="sxs-lookup"><span data-stu-id="82c2f-149">Windows</span></span>
- <span data-ttu-id="82c2f-150">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="82c2f-150">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="82c2f-151">JSON</span><span class="sxs-lookup"><span data-stu-id="82c2f-151">JSON</span></span>

<span data-ttu-id="82c2f-152">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[теамсдевицеусажедистрибутионусеркаунтс](../resources/teamsdeviceusagedistributionusercounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="82c2f-152">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82c2f-153">Пример</span><span class="sxs-lookup"><span data-stu-id="82c2f-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="82c2f-154">CSV</span><span class="sxs-lookup"><span data-stu-id="82c2f-154">CSV</span></span>

<span data-ttu-id="82c2f-155">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="82c2f-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="82c2f-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="82c2f-156">Request</span></span>

<span data-ttu-id="82c2f-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="82c2f-157">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="82c2f-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="82c2f-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="82c2f-159">C#</span><span class="sxs-lookup"><span data-stu-id="82c2f-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsdeviceusagedistributionusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="82c2f-160">Javascript</span><span class="sxs-lookup"><span data-stu-id="82c2f-160">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsdeviceusagedistributionusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="82c2f-161">Цель — C</span><span class="sxs-lookup"><span data-stu-id="82c2f-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsdeviceusagedistributionusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="82c2f-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="82c2f-162">Response</span></span>

<span data-ttu-id="82c2f-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="82c2f-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="82c2f-164">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="82c2f-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iOS,Mac,Windows,Report Period
```

### <a name="json"></a><span data-ttu-id="82c2f-165">JSON</span><span class="sxs-lookup"><span data-stu-id="82c2f-165">JSON</span></span>

<span data-ttu-id="82c2f-166">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="82c2f-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="82c2f-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="82c2f-167">Request</span></span>

<span data-ttu-id="82c2f-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="82c2f-168">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="82c2f-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="82c2f-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="82c2f-170">C#</span><span class="sxs-lookup"><span data-stu-id="82c2f-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsdeviceusagedistributionusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="82c2f-171">Javascript</span><span class="sxs-lookup"><span data-stu-id="82c2f-171">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsdeviceusagedistributionusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="82c2f-172">Цель — C</span><span class="sxs-lookup"><span data-stu-id="82c2f-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsdeviceusagedistributionusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="82c2f-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="82c2f-173">Response</span></span>

<span data-ttu-id="82c2f-174">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="82c2f-174">The following is an example of the response.</span></span>

> <span data-ttu-id="82c2f-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="82c2f-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsDeviceUsageDistributionUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 243

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsDeviceUsageDistributionUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "web": 51, 
      "windowsPhone": 2, 
      "androidPhone": 34, 
      "ios": 76, 
      "mac": 40, 
      "windows": 491, 
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
