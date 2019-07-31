---
title: 'reportRoot: getTeamsDeviceUsageUserCounts'
description: Получение сведений о количестве уникальных пользователей Microsoft Teams в день с сортировкой по типам устройств.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 88fad03f7599831fcc17d38e8563bb7464bcf552
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35983112"
---
# <a name="reportroot-getteamsdeviceusageusercounts"></a><span data-ttu-id="46936-103">reportRoot: getTeamsDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="46936-103">reportRoot: getTeamsDeviceUsageUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46936-104">Получение сведений о количестве уникальных пользователей Microsoft Teams в день с сортировкой по типам устройств.</span><span class="sxs-lookup"><span data-stu-id="46936-104">Get the number of Microsoft Teams daily unique users by device type.</span></span>

## <a name="permissions"></a><span data-ttu-id="46936-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="46936-105">Permissions</span></span>

<span data-ttu-id="46936-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46936-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="46936-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="46936-108">Permission type</span></span>                        | <span data-ttu-id="46936-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="46936-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="46936-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="46936-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="46936-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="46936-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="46936-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="46936-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46936-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46936-113">Not supported.</span></span>                           |
| <span data-ttu-id="46936-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="46936-114">Application</span></span>                            | <span data-ttu-id="46936-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="46936-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="46936-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="46936-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="46936-117">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="46936-117">Function parameters</span></span>

<span data-ttu-id="46936-118">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="46936-118">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="46936-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="46936-119">Parameter</span></span> | <span data-ttu-id="46936-120">Тип</span><span class="sxs-lookup"><span data-stu-id="46936-120">Type</span></span>   | <span data-ttu-id="46936-121">Описание</span><span class="sxs-lookup"><span data-stu-id="46936-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="46936-122">period</span><span class="sxs-lookup"><span data-stu-id="46936-122">period</span></span>    | <span data-ttu-id="46936-123">string</span><span class="sxs-lookup"><span data-stu-id="46936-123">string</span></span> | <span data-ttu-id="46936-124">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="46936-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="46936-125">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="46936-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="46936-126">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="46936-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="46936-127">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="46936-127">Required.</span></span> |

<span data-ttu-id="46936-128">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="46936-128">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="46936-129">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="46936-129">The default output type is text/csv.</span></span> <span data-ttu-id="46936-130">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="46936-130">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="46936-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="46936-131">Request headers</span></span>

| <span data-ttu-id="46936-132">Имя</span><span class="sxs-lookup"><span data-stu-id="46936-132">Name</span></span>          | <span data-ttu-id="46936-133">Описание</span><span class="sxs-lookup"><span data-stu-id="46936-133">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="46936-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="46936-134">Authorization</span></span> | <span data-ttu-id="46936-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="46936-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="46936-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="46936-137">Response</span></span>

### <a name="csv"></a><span data-ttu-id="46936-138">CSV</span><span class="sxs-lookup"><span data-stu-id="46936-138">CSV</span></span>

<span data-ttu-id="46936-139">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="46936-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="46936-140">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="46936-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="46936-141">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="46936-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="46936-142">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="46936-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="46936-143">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="46936-143">Report Refresh Date</span></span>
- <span data-ttu-id="46936-144">"Web" (Интернет);</span><span class="sxs-lookup"><span data-stu-id="46936-144">Web</span></span>
- <span data-ttu-id="46936-145">"Windows Phone";</span><span class="sxs-lookup"><span data-stu-id="46936-145">Windows Phone</span></span>
- <span data-ttu-id="46936-146">"Android Phone" (Телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="46936-146">Android Phone</span></span>
- <span data-ttu-id="46936-147">"iOS";</span><span class="sxs-lookup"><span data-stu-id="46936-147">iOS</span></span>
- <span data-ttu-id="46936-148">"Mac";</span><span class="sxs-lookup"><span data-stu-id="46936-148">Mac</span></span>
- <span data-ttu-id="46936-149">"Windows";</span><span class="sxs-lookup"><span data-stu-id="46936-149">Windows</span></span>
- <span data-ttu-id="46936-150">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="46936-150">Report Date</span></span>
- <span data-ttu-id="46936-151">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="46936-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="46936-152">JSON</span><span class="sxs-lookup"><span data-stu-id="46936-152">JSON</span></span>

<span data-ttu-id="46936-153">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[теамсдевицеусажеусеркаунтс](../resources/teamsdeviceusageusercounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="46936-153">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageUserCounts](../resources/teamsdeviceusageusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46936-154">Пример</span><span class="sxs-lookup"><span data-stu-id="46936-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="46936-155">CSV</span><span class="sxs-lookup"><span data-stu-id="46936-155">CSV</span></span>

<span data-ttu-id="46936-156">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="46936-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="46936-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="46936-157">Request</span></span>

<span data-ttu-id="46936-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="46936-158">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="46936-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="46936-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="46936-160">C#</span><span class="sxs-lookup"><span data-stu-id="46936-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsdeviceusageusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="46936-161">Javascript</span><span class="sxs-lookup"><span data-stu-id="46936-161">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsdeviceusageusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="46936-162">Цель — C</span><span class="sxs-lookup"><span data-stu-id="46936-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsdeviceusageusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="46936-163">Java</span><span class="sxs-lookup"><span data-stu-id="46936-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getteamsdeviceusageusercounts-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="46936-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="46936-164">Response</span></span>

<span data-ttu-id="46936-165">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="46936-165">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="46936-166">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="46936-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="46936-167">JSON</span><span class="sxs-lookup"><span data-stu-id="46936-167">JSON</span></span>

<span data-ttu-id="46936-168">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="46936-168">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="46936-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="46936-169">Request</span></span>

<span data-ttu-id="46936-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="46936-170">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="46936-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="46936-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="46936-172">C#</span><span class="sxs-lookup"><span data-stu-id="46936-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsdeviceusageusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="46936-173">Javascript</span><span class="sxs-lookup"><span data-stu-id="46936-173">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsdeviceusageusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="46936-174">Цель — C</span><span class="sxs-lookup"><span data-stu-id="46936-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsdeviceusageusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="46936-175">Java</span><span class="sxs-lookup"><span data-stu-id="46936-175">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getteamsdeviceusageusercounts-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="46936-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="46936-176">Response</span></span>

<span data-ttu-id="46936-177">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="46936-177">The following is an example of the response.</span></span>

> <span data-ttu-id="46936-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="46936-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
