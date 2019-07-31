---
title: 'reportRoot: getTeamsDeviceUsageDistributionUserCounts'
description: Получение количества уникальных пользователей Microsoft Teams с сортировкой по типам устройств за выбранный период.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 42f8d4f0d129ddaabc62ee22a9a37650d18ba32c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35991802"
---
# <a name="reportroot-getteamsdeviceusagedistributionusercounts"></a><span data-ttu-id="60056-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="60056-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60056-104">Получение количества уникальных пользователей Microsoft Teams с сортировкой по типам устройств за выбранный период.</span><span class="sxs-lookup"><span data-stu-id="60056-104">Get the number of Microsoft Teams unique users by device type over the selected time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="60056-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="60056-105">Permissions</span></span>

<span data-ttu-id="60056-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60056-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="60056-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="60056-108">Permission type</span></span>                        | <span data-ttu-id="60056-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="60056-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="60056-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="60056-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="60056-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="60056-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="60056-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="60056-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60056-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60056-113">Not supported.</span></span>                           |
| <span data-ttu-id="60056-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="60056-114">Application</span></span>                            | <span data-ttu-id="60056-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="60056-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="60056-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="60056-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="60056-117">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="60056-117">Function parameters</span></span>

<span data-ttu-id="60056-118">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="60056-118">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="60056-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="60056-119">Parameter</span></span> | <span data-ttu-id="60056-120">Тип</span><span class="sxs-lookup"><span data-stu-id="60056-120">Type</span></span>   | <span data-ttu-id="60056-121">Описание</span><span class="sxs-lookup"><span data-stu-id="60056-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="60056-122">period</span><span class="sxs-lookup"><span data-stu-id="60056-122">period</span></span>    | <span data-ttu-id="60056-123">string</span><span class="sxs-lookup"><span data-stu-id="60056-123">string</span></span> | <span data-ttu-id="60056-124">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="60056-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="60056-125">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="60056-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="60056-126">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="60056-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="60056-127">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="60056-127">Required.</span></span> |

<span data-ttu-id="60056-128">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="60056-128">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="60056-129">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="60056-129">The default output type is text/csv.</span></span> <span data-ttu-id="60056-130">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="60056-130">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="60056-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="60056-131">Request headers</span></span>

| <span data-ttu-id="60056-132">Имя</span><span class="sxs-lookup"><span data-stu-id="60056-132">Name</span></span>          | <span data-ttu-id="60056-133">Описание</span><span class="sxs-lookup"><span data-stu-id="60056-133">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="60056-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="60056-134">Authorization</span></span> | <span data-ttu-id="60056-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="60056-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="60056-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="60056-137">Response</span></span>

### <a name="csv"></a><span data-ttu-id="60056-138">CSV</span><span class="sxs-lookup"><span data-stu-id="60056-138">CSV</span></span>

<span data-ttu-id="60056-139">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="60056-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="60056-140">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="60056-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="60056-141">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="60056-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="60056-142">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="60056-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="60056-143">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="60056-143">Report Refresh Date</span></span>
- <span data-ttu-id="60056-144">"Web" (Интернет);</span><span class="sxs-lookup"><span data-stu-id="60056-144">Web</span></span>
- <span data-ttu-id="60056-145">"Windows Phone";</span><span class="sxs-lookup"><span data-stu-id="60056-145">Windows Phone</span></span>
- <span data-ttu-id="60056-146">"Android Phone" (Телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="60056-146">Android Phone</span></span>
- <span data-ttu-id="60056-147">"iOS";</span><span class="sxs-lookup"><span data-stu-id="60056-147">iOS</span></span>
- <span data-ttu-id="60056-148">"Mac";</span><span class="sxs-lookup"><span data-stu-id="60056-148">Mac</span></span>
- <span data-ttu-id="60056-149">"Windows";</span><span class="sxs-lookup"><span data-stu-id="60056-149">Windows</span></span>
- <span data-ttu-id="60056-150">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="60056-150">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="60056-151">JSON</span><span class="sxs-lookup"><span data-stu-id="60056-151">JSON</span></span>

<span data-ttu-id="60056-152">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[теамсдевицеусажедистрибутионусеркаунтс](../resources/teamsdeviceusagedistributionusercounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="60056-152">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60056-153">Пример</span><span class="sxs-lookup"><span data-stu-id="60056-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="60056-154">CSV</span><span class="sxs-lookup"><span data-stu-id="60056-154">CSV</span></span>

<span data-ttu-id="60056-155">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="60056-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="60056-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="60056-156">Request</span></span>

<span data-ttu-id="60056-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="60056-157">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="60056-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="60056-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="60056-159">C#</span><span class="sxs-lookup"><span data-stu-id="60056-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsdeviceusagedistributionusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="60056-160">Javascript</span><span class="sxs-lookup"><span data-stu-id="60056-160">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsdeviceusagedistributionusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="60056-161">Цель — C</span><span class="sxs-lookup"><span data-stu-id="60056-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsdeviceusagedistributionusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="60056-162">Java</span><span class="sxs-lookup"><span data-stu-id="60056-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getteamsdeviceusagedistributionusercounts-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="60056-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="60056-163">Response</span></span>

<span data-ttu-id="60056-164">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="60056-164">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="60056-165">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="60056-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="60056-166">JSON</span><span class="sxs-lookup"><span data-stu-id="60056-166">JSON</span></span>

<span data-ttu-id="60056-167">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="60056-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="60056-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="60056-168">Request</span></span>

<span data-ttu-id="60056-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="60056-169">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="60056-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="60056-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="60056-171">C#</span><span class="sxs-lookup"><span data-stu-id="60056-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsdeviceusagedistributionusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="60056-172">Javascript</span><span class="sxs-lookup"><span data-stu-id="60056-172">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsdeviceusagedistributionusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="60056-173">Цель — C</span><span class="sxs-lookup"><span data-stu-id="60056-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsdeviceusagedistributionusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="60056-174">Java</span><span class="sxs-lookup"><span data-stu-id="60056-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getteamsdeviceusagedistributionusercounts-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="60056-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="60056-175">Response</span></span>

<span data-ttu-id="60056-176">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="60056-176">The following is an example of the response.</span></span>

> <span data-ttu-id="60056-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="60056-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
