---
title: 'reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts'
description: Узнайте, сколько сотрудников организации используют уникальные устройства. В отчете будет показано количество пользователей устройств с Windows, телефонов с Windows, телефонов с Android, iPhone и iPad.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 94216c6afff294d7d1dbffb97896d095dc20b6e0
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36722869"
---
# <a name="reportroot-getskypeforbusinessdeviceusagedistributionusercounts"></a><span data-ttu-id="70212-104">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="70212-104">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70212-105">Узнайте, сколько сотрудников организации используют уникальные устройства.</span><span class="sxs-lookup"><span data-stu-id="70212-105">Get the number of users using unique devices in your organization.</span></span> <span data-ttu-id="70212-106">В отчете будет показано количество пользователей Windows, телефонов с Windows, телефонов с Android, iPhone и iPad.</span><span class="sxs-lookup"><span data-stu-id="70212-106">The report will show you the number of users per device including Windows, Windows phone, Android phone, iPhone, and iPad.</span></span>

> <span data-ttu-id="70212-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span><span class="sxs-lookup"><span data-stu-id="70212-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="70212-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="70212-108">Permissions</span></span>

<span data-ttu-id="70212-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70212-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="70212-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="70212-111">Permission type</span></span>                        | <span data-ttu-id="70212-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="70212-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="70212-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="70212-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="70212-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="70212-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="70212-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="70212-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70212-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70212-116">Not supported.</span></span>                           |
| <span data-ttu-id="70212-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="70212-117">Application</span></span>                            | <span data-ttu-id="70212-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="70212-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="70212-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="70212-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="70212-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="70212-120">Function parameters</span></span>

<span data-ttu-id="70212-121">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="70212-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="70212-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="70212-122">Parameter</span></span> | <span data-ttu-id="70212-123">Тип</span><span class="sxs-lookup"><span data-stu-id="70212-123">Type</span></span>   | <span data-ttu-id="70212-124">Описание</span><span class="sxs-lookup"><span data-stu-id="70212-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="70212-125">period</span><span class="sxs-lookup"><span data-stu-id="70212-125">period</span></span>    | <span data-ttu-id="70212-126">string</span><span class="sxs-lookup"><span data-stu-id="70212-126">string</span></span> | <span data-ttu-id="70212-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="70212-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="70212-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="70212-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="70212-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="70212-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="70212-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="70212-130">Required.</span></span> |

<span data-ttu-id="70212-131">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="70212-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="70212-132">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="70212-132">The default output type is text/csv.</span></span> <span data-ttu-id="70212-133">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="70212-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="70212-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="70212-134">Request headers</span></span>

| <span data-ttu-id="70212-135">Имя</span><span class="sxs-lookup"><span data-stu-id="70212-135">Name</span></span>          | <span data-ttu-id="70212-136">Описание</span><span class="sxs-lookup"><span data-stu-id="70212-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="70212-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="70212-137">Authorization</span></span> | <span data-ttu-id="70212-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="70212-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="70212-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="70212-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="70212-141">CSV</span><span class="sxs-lookup"><span data-stu-id="70212-141">CSV</span></span>

<span data-ttu-id="70212-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="70212-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="70212-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="70212-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="70212-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="70212-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="70212-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="70212-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="70212-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="70212-146">Report Refresh Date</span></span>
- <span data-ttu-id="70212-147">"Windows";</span><span class="sxs-lookup"><span data-stu-id="70212-147">Windows</span></span>
- <span data-ttu-id="70212-148">"Windows Phone";</span><span class="sxs-lookup"><span data-stu-id="70212-148">Windows Phone</span></span>
- <span data-ttu-id="70212-149">"Android Phone" (Телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="70212-149">Android Phone</span></span>
- <span data-ttu-id="70212-150">iPhone</span><span class="sxs-lookup"><span data-stu-id="70212-150">iPhone</span></span>
- <span data-ttu-id="70212-151">iPad</span><span class="sxs-lookup"><span data-stu-id="70212-151">iPad</span></span>
- <span data-ttu-id="70212-152">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="70212-152">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="70212-153">JSON</span><span class="sxs-lookup"><span data-stu-id="70212-153">JSON</span></span>

<span data-ttu-id="70212-154">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[скипефорбусинессдевицеусажедистрибутионусеркаунтс](../resources/skypeforbusinessdeviceusagedistributionusercounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="70212-154">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessDeviceUsageDistributionUserCounts](../resources/skypeforbusinessdeviceusagedistributionusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70212-155">Пример</span><span class="sxs-lookup"><span data-stu-id="70212-155">Example</span></span>

### <a name="csv"></a><span data-ttu-id="70212-156">CSV</span><span class="sxs-lookup"><span data-stu-id="70212-156">CSV</span></span>

<span data-ttu-id="70212-157">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="70212-157">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="70212-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="70212-158">Request</span></span>

<span data-ttu-id="70212-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="70212-159">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="70212-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="70212-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusagedistributionusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="70212-161">C#</span><span class="sxs-lookup"><span data-stu-id="70212-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessdeviceusagedistributionusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="70212-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="70212-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessdeviceusagedistributionusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="70212-163">Цель — C</span><span class="sxs-lookup"><span data-stu-id="70212-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessdeviceusagedistributionusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="70212-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="70212-164">Response</span></span>

<span data-ttu-id="70212-165">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="70212-165">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="70212-166">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="70212-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Windows,Windows Phone,Android Phone,iPhone,iPad,Report Period
```

### <a name="json"></a><span data-ttu-id="70212-167">JSON</span><span class="sxs-lookup"><span data-stu-id="70212-167">JSON</span></span>

<span data-ttu-id="70212-168">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="70212-168">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="70212-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="70212-169">Request</span></span>

<span data-ttu-id="70212-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="70212-170">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="70212-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="70212-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusagedistributionusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="70212-172">C#</span><span class="sxs-lookup"><span data-stu-id="70212-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessdeviceusagedistributionusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="70212-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="70212-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessdeviceusagedistributionusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="70212-174">Цель — C</span><span class="sxs-lookup"><span data-stu-id="70212-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessdeviceusagedistributionusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="70212-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="70212-175">Response</span></span>

<span data-ttu-id="70212-176">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="70212-176">The following is an example of the response.</span></span>

> <span data-ttu-id="70212-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="70212-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageDistributionUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 275

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessDeviceUsageDistributionUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "windows": 122, 
      "windowsPhone": 8, 
      "androidPhone": 19, 
      "iPhone": 28, 
      "iPad": 1, 
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
