---
title: 'reportRoot: getYammerDeviceUsageUserCounts'
description: Получите сведения о количестве пользователей в день с разбивкой по типам устройств.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 3f1179bfd5e4c587743bda856d5eccd298a7c9bb
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867052"
---
# <a name="reportroot-getyammerdeviceusageusercounts"></a><span data-ttu-id="ef3a1-103">reportRoot: getYammerDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="ef3a1-103">reportRoot: getYammerDeviceUsageUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef3a1-104">Получите сведения о количестве пользователей в день с разбивкой по типам устройств.</span><span class="sxs-lookup"><span data-stu-id="ef3a1-104">Get the number of daily users by device type.</span></span>

> <span data-ttu-id="ef3a1-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="ef3a1-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="ef3a1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ef3a1-106">Permissions</span></span>

<span data-ttu-id="ef3a1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef3a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ef3a1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ef3a1-109">Permission type</span></span>                        | <span data-ttu-id="ef3a1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ef3a1-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ef3a1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ef3a1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ef3a1-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ef3a1-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ef3a1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ef3a1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef3a1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef3a1-114">Not supported.</span></span>                           |
| <span data-ttu-id="ef3a1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ef3a1-115">Application</span></span>                            | <span data-ttu-id="ef3a1-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ef3a1-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="ef3a1-117">**Примечание**. для делегированных разрешений, чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя, администратору клиента необходимо назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ef3a1-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="ef3a1-118">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="ef3a1-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="ef3a1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ef3a1-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="ef3a1-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="ef3a1-120">Function parameters</span></span>

<span data-ttu-id="ef3a1-121">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="ef3a1-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="ef3a1-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="ef3a1-122">Parameter</span></span> | <span data-ttu-id="ef3a1-123">Тип</span><span class="sxs-lookup"><span data-stu-id="ef3a1-123">Type</span></span>   | <span data-ttu-id="ef3a1-124">Описание</span><span class="sxs-lookup"><span data-stu-id="ef3a1-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="ef3a1-125">period</span><span class="sxs-lookup"><span data-stu-id="ef3a1-125">period</span></span>    | <span data-ttu-id="ef3a1-126">string</span><span class="sxs-lookup"><span data-stu-id="ef3a1-126">string</span></span> | <span data-ttu-id="ef3a1-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="ef3a1-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="ef3a1-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="ef3a1-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="ef3a1-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="ef3a1-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="ef3a1-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ef3a1-130">Required.</span></span> |

<span data-ttu-id="ef3a1-131">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="ef3a1-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="ef3a1-132">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="ef3a1-132">The default output type is text/csv.</span></span> <span data-ttu-id="ef3a1-133">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="ef3a1-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ef3a1-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ef3a1-134">Request headers</span></span>

| <span data-ttu-id="ef3a1-135">Имя</span><span class="sxs-lookup"><span data-stu-id="ef3a1-135">Name</span></span>          | <span data-ttu-id="ef3a1-136">Описание</span><span class="sxs-lookup"><span data-stu-id="ef3a1-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="ef3a1-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ef3a1-137">Authorization</span></span> | <span data-ttu-id="ef3a1-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ef3a1-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="ef3a1-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef3a1-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="ef3a1-141">CSV</span><span class="sxs-lookup"><span data-stu-id="ef3a1-141">CSV</span></span>

<span data-ttu-id="ef3a1-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="ef3a1-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ef3a1-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="ef3a1-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ef3a1-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="ef3a1-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ef3a1-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="ef3a1-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="ef3a1-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="ef3a1-146">Report Refresh Date</span></span>
- <span data-ttu-id="ef3a1-147">"Web" (Интернет);</span><span class="sxs-lookup"><span data-stu-id="ef3a1-147">Web</span></span>
- <span data-ttu-id="ef3a1-148">"Windows Phone";</span><span class="sxs-lookup"><span data-stu-id="ef3a1-148">Windows Phone</span></span>
- <span data-ttu-id="ef3a1-149">"Android Phone" (Телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="ef3a1-149">Android Phone</span></span>
- <span data-ttu-id="ef3a1-150">iPhone</span><span class="sxs-lookup"><span data-stu-id="ef3a1-150">iPhone</span></span>
- <span data-ttu-id="ef3a1-151">iPad</span><span class="sxs-lookup"><span data-stu-id="ef3a1-151">iPad</span></span>
- <span data-ttu-id="ef3a1-152">Other (другие)</span><span class="sxs-lookup"><span data-stu-id="ef3a1-152">Other</span></span>
- <span data-ttu-id="ef3a1-153">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="ef3a1-153">Report Date</span></span>
- <span data-ttu-id="ef3a1-154">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="ef3a1-154">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="ef3a1-155">JSON</span><span class="sxs-lookup"><span data-stu-id="ef3a1-155">JSON</span></span>

<span data-ttu-id="ef3a1-156">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[яммердевицеусажеусеркаунтс](../resources/yammerdeviceusageusercounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ef3a1-156">If successful, this method returns a `200 OK` response code and a **[yammerDeviceUsageUserCounts](../resources/yammerdeviceusageusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef3a1-157">Пример</span><span class="sxs-lookup"><span data-stu-id="ef3a1-157">Example</span></span>

### <a name="csv"></a><span data-ttu-id="ef3a1-158">CSV</span><span class="sxs-lookup"><span data-stu-id="ef3a1-158">CSV</span></span>

<span data-ttu-id="ef3a1-159">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="ef3a1-159">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="ef3a1-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef3a1-160">Request</span></span>

<span data-ttu-id="ef3a1-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ef3a1-161">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ef3a1-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="ef3a1-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusageusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ef3a1-163">C#</span><span class="sxs-lookup"><span data-stu-id="ef3a1-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammerdeviceusageusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ef3a1-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ef3a1-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammerdeviceusageusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ef3a1-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ef3a1-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammerdeviceusageusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ef3a1-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef3a1-166">Response</span></span>

<span data-ttu-id="ef3a1-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ef3a1-167">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="ef3a1-168">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="ef3a1-168">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iPhone,iPad,Other,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="ef3a1-169">JSON</span><span class="sxs-lookup"><span data-stu-id="ef3a1-169">JSON</span></span>

<span data-ttu-id="ef3a1-170">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="ef3a1-170">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="ef3a1-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef3a1-171">Request</span></span>

<span data-ttu-id="ef3a1-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ef3a1-172">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ef3a1-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="ef3a1-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusageusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ef3a1-174">C#</span><span class="sxs-lookup"><span data-stu-id="ef3a1-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammerdeviceusageusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ef3a1-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ef3a1-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammerdeviceusageusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ef3a1-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ef3a1-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammerdeviceusageusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ef3a1-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef3a1-177">Response</span></span>

<span data-ttu-id="ef3a1-178">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ef3a1-178">The following is an example of the response.</span></span>

> <span data-ttu-id="ef3a1-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ef3a1-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerDeviceUsageUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 284

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerDeviceUsageUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "web": 63, 
      "windowsPhone": 1, 
      "androidPhone": 17, 
      "iPhone": 23, 
      "iPad": 1, 
      "other": 2, 
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
