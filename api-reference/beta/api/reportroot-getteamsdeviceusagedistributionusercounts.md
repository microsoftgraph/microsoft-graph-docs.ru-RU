---
title: 'reportRoot: getTeamsDeviceUsageDistributionUserCounts'
description: Получение количества уникальных пользователей Microsoft Teams с сортировкой по типам устройств за выбранный период.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: bd0a43c356a4922a2f648fd2eeacb47a7006a9be
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358903"
---
# <a name="reportroot-getteamsdeviceusagedistributionusercounts"></a><span data-ttu-id="4b6d9-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="4b6d9-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b6d9-104">Получение количества уникальных пользователей Microsoft Teams с сортировкой по типам устройств за выбранный период.</span><span class="sxs-lookup"><span data-stu-id="4b6d9-104">Get the number of Microsoft Teams unique users by device type over the selected time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="4b6d9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4b6d9-105">Permissions</span></span>

<span data-ttu-id="4b6d9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b6d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4b6d9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b6d9-108">Permission type</span></span>                        | <span data-ttu-id="4b6d9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b6d9-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="4b6d9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b6d9-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="4b6d9-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b6d9-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="4b6d9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b6d9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b6d9-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b6d9-113">Not supported.</span></span>                           |
| <span data-ttu-id="4b6d9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4b6d9-114">Application</span></span>                            | <span data-ttu-id="4b6d9-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b6d9-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="4b6d9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b6d9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="4b6d9-117">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="4b6d9-117">Function parameters</span></span>

<span data-ttu-id="4b6d9-118">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="4b6d9-118">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="4b6d9-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="4b6d9-119">Parameter</span></span> | <span data-ttu-id="4b6d9-120">Тип</span><span class="sxs-lookup"><span data-stu-id="4b6d9-120">Type</span></span>   | <span data-ttu-id="4b6d9-121">Описание</span><span class="sxs-lookup"><span data-stu-id="4b6d9-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="4b6d9-122">period</span><span class="sxs-lookup"><span data-stu-id="4b6d9-122">period</span></span>    | <span data-ttu-id="4b6d9-123">string</span><span class="sxs-lookup"><span data-stu-id="4b6d9-123">string</span></span> | <span data-ttu-id="4b6d9-124">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="4b6d9-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="4b6d9-125">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="4b6d9-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="4b6d9-126">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="4b6d9-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="4b6d9-127">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b6d9-127">Required.</span></span> |

<span data-ttu-id="4b6d9-128">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="4b6d9-128">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="4b6d9-129">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="4b6d9-129">The default output type is text/csv.</span></span> <span data-ttu-id="4b6d9-130">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="4b6d9-130">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4b6d9-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4b6d9-131">Request headers</span></span>

| <span data-ttu-id="4b6d9-132">Имя</span><span class="sxs-lookup"><span data-stu-id="4b6d9-132">Name</span></span>          | <span data-ttu-id="4b6d9-133">Описание</span><span class="sxs-lookup"><span data-stu-id="4b6d9-133">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="4b6d9-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4b6d9-134">Authorization</span></span> | <span data-ttu-id="4b6d9-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b6d9-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="4b6d9-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b6d9-137">Response</span></span>

### <a name="csv"></a><span data-ttu-id="4b6d9-138">CSV</span><span class="sxs-lookup"><span data-stu-id="4b6d9-138">CSV</span></span>

<span data-ttu-id="4b6d9-139">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="4b6d9-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="4b6d9-140">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="4b6d9-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="4b6d9-141">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="4b6d9-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="4b6d9-142">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="4b6d9-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="4b6d9-143">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="4b6d9-143">Report Refresh Date</span></span>
- <span data-ttu-id="4b6d9-144">"Web" (Интернет);</span><span class="sxs-lookup"><span data-stu-id="4b6d9-144">Web</span></span>
- <span data-ttu-id="4b6d9-145">"Windows Phone";</span><span class="sxs-lookup"><span data-stu-id="4b6d9-145">Windows Phone</span></span>
- <span data-ttu-id="4b6d9-146">"Android Phone" (Телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="4b6d9-146">Android Phone</span></span>
- <span data-ttu-id="4b6d9-147">"iOS";</span><span class="sxs-lookup"><span data-stu-id="4b6d9-147">iOS</span></span>
- <span data-ttu-id="4b6d9-148">"Mac";</span><span class="sxs-lookup"><span data-stu-id="4b6d9-148">Mac</span></span>
- <span data-ttu-id="4b6d9-149">"Windows";</span><span class="sxs-lookup"><span data-stu-id="4b6d9-149">Windows</span></span>
- <span data-ttu-id="4b6d9-150">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="4b6d9-150">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="4b6d9-151">JSON</span><span class="sxs-lookup"><span data-stu-id="4b6d9-151">JSON</span></span>

<span data-ttu-id="4b6d9-152">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[теамсдевицеусажедистрибутионусеркаунтс](../resources/teamsdeviceusagedistributionusercounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4b6d9-152">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b6d9-153">Пример</span><span class="sxs-lookup"><span data-stu-id="4b6d9-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="4b6d9-154">CSV</span><span class="sxs-lookup"><span data-stu-id="4b6d9-154">CSV</span></span>

<span data-ttu-id="4b6d9-155">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="4b6d9-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="4b6d9-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b6d9-156">Request</span></span>

<span data-ttu-id="4b6d9-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b6d9-157">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="4b6d9-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="4b6d9-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4b6d9-159">C#</span><span class="sxs-lookup"><span data-stu-id="4b6d9-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsdeviceusagedistributionusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4b6d9-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4b6d9-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsdeviceusagedistributionusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4b6d9-161">Цель — C</span><span class="sxs-lookup"><span data-stu-id="4b6d9-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsdeviceusagedistributionusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4b6d9-162">Java</span><span class="sxs-lookup"><span data-stu-id="4b6d9-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getteamsdeviceusagedistributionusercounts-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4b6d9-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b6d9-163">Response</span></span>

<span data-ttu-id="4b6d9-164">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4b6d9-164">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="4b6d9-165">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="4b6d9-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="4b6d9-166">JSON</span><span class="sxs-lookup"><span data-stu-id="4b6d9-166">JSON</span></span>

<span data-ttu-id="4b6d9-167">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="4b6d9-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="4b6d9-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b6d9-168">Request</span></span>

<span data-ttu-id="4b6d9-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b6d9-169">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="4b6d9-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="4b6d9-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4b6d9-171">C#</span><span class="sxs-lookup"><span data-stu-id="4b6d9-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsdeviceusagedistributionusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4b6d9-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4b6d9-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsdeviceusagedistributionusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4b6d9-173">Цель — C</span><span class="sxs-lookup"><span data-stu-id="4b6d9-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsdeviceusagedistributionusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4b6d9-174">Java</span><span class="sxs-lookup"><span data-stu-id="4b6d9-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getteamsdeviceusagedistributionusercounts-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4b6d9-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b6d9-175">Response</span></span>

<span data-ttu-id="4b6d9-176">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4b6d9-176">The following is an example of the response.</span></span>

> <span data-ttu-id="4b6d9-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4b6d9-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
