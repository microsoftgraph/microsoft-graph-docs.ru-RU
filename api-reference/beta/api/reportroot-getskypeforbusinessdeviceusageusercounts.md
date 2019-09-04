---
title: 'reportRoot: getSkypeForBusinessDeviceUsageUserCounts'
description: Отследите динамику использования по количеству пользователей в организации, подключавшихся с помощью приложения Skype для бизнеса. Кроме того, вы получите статистические данные с разбивкой по типу устройства (устройство с Windows, телефон с Windows, телефон с Android, iPhone или iPad), на котором установлено клиентское приложение Skype для бизнеса, используемое в организации.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: e816f37e0bedbbbfa176fc2a8d6fac1c879bdec5
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36724988"
---
# <a name="reportroot-getskypeforbusinessdeviceusageusercounts"></a><span data-ttu-id="c4058-104">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="c4058-104">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4058-105">Отследите динамику использования по количеству пользователей в организации, подключавшихся с помощью приложения Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="c4058-105">Get the usage trends on how many users in your organization have connected using the Skype for Business app.</span></span> <span data-ttu-id="c4058-106">Кроме того, вы получите статистические данные с разбивкой по типу устройства (Windows, телефон с Windows, телефон с Android, iPhone или iPad), на котором установлено клиентское приложение Skype для бизнеса, используемое в организации.</span><span class="sxs-lookup"><span data-stu-id="c4058-106">You will also get a breakdown by the type of device (Windows, Windows phone, Android phone, iPhone, or iPad) on which the Skype for Business client app is installed and used across your organization.</span></span>

> <span data-ttu-id="c4058-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: используемые клиенты Skype для бизнеса](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span><span class="sxs-lookup"><span data-stu-id="c4058-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="c4058-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c4058-108">Permissions</span></span>

<span data-ttu-id="c4058-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4058-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c4058-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c4058-111">Permission type</span></span>                        | <span data-ttu-id="c4058-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c4058-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="c4058-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c4058-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="c4058-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c4058-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="c4058-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c4058-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4058-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4058-116">Not supported.</span></span>                           |
| <span data-ttu-id="c4058-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c4058-117">Application</span></span>                            | <span data-ttu-id="c4058-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c4058-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="c4058-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c4058-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="c4058-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="c4058-120">Function parameters</span></span>

<span data-ttu-id="c4058-121">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="c4058-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="c4058-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="c4058-122">Parameter</span></span> | <span data-ttu-id="c4058-123">Тип</span><span class="sxs-lookup"><span data-stu-id="c4058-123">Type</span></span>   | <span data-ttu-id="c4058-124">Описание</span><span class="sxs-lookup"><span data-stu-id="c4058-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="c4058-125">period</span><span class="sxs-lookup"><span data-stu-id="c4058-125">period</span></span>    | <span data-ttu-id="c4058-126">string</span><span class="sxs-lookup"><span data-stu-id="c4058-126">string</span></span> | <span data-ttu-id="c4058-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="c4058-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="c4058-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="c4058-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="c4058-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="c4058-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="c4058-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c4058-130">Required.</span></span> |

<span data-ttu-id="c4058-131">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="c4058-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="c4058-132">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="c4058-132">The default output type is text/csv.</span></span> <span data-ttu-id="c4058-133">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="c4058-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c4058-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c4058-134">Request headers</span></span>

| <span data-ttu-id="c4058-135">Имя</span><span class="sxs-lookup"><span data-stu-id="c4058-135">Name</span></span>          | <span data-ttu-id="c4058-136">Описание</span><span class="sxs-lookup"><span data-stu-id="c4058-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="c4058-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c4058-137">Authorization</span></span> | <span data-ttu-id="c4058-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c4058-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="c4058-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4058-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="c4058-141">CSV</span><span class="sxs-lookup"><span data-stu-id="c4058-141">CSV</span></span>

<span data-ttu-id="c4058-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="c4058-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="c4058-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="c4058-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="c4058-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="c4058-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="c4058-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="c4058-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="c4058-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="c4058-146">Report Refresh Date</span></span>
- <span data-ttu-id="c4058-147">"Windows";</span><span class="sxs-lookup"><span data-stu-id="c4058-147">Windows</span></span>
- <span data-ttu-id="c4058-148">"Windows Phone";</span><span class="sxs-lookup"><span data-stu-id="c4058-148">Windows Phone</span></span>
- <span data-ttu-id="c4058-149">"Android Phone" (Телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="c4058-149">Android Phone</span></span>
- <span data-ttu-id="c4058-150">iPhone</span><span class="sxs-lookup"><span data-stu-id="c4058-150">iPhone</span></span>
- <span data-ttu-id="c4058-151">iPad</span><span class="sxs-lookup"><span data-stu-id="c4058-151">iPad</span></span>
- <span data-ttu-id="c4058-152">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="c4058-152">Report Date</span></span>
- <span data-ttu-id="c4058-153">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="c4058-153">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="c4058-154">JSON</span><span class="sxs-lookup"><span data-stu-id="c4058-154">JSON</span></span>

<span data-ttu-id="c4058-155">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[скипефорбусинессдевицеусажеусеркаунтс](../resources/skypeforbusinessdeviceusageusercounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c4058-155">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessDeviceUsageUserCounts](../resources/skypeforbusinessdeviceusageusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4058-156">Пример</span><span class="sxs-lookup"><span data-stu-id="c4058-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="c4058-157">CSV</span><span class="sxs-lookup"><span data-stu-id="c4058-157">CSV</span></span>

<span data-ttu-id="c4058-158">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="c4058-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="c4058-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4058-159">Request</span></span>

<span data-ttu-id="c4058-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c4058-160">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c4058-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4058-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusageusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c4058-162">C#</span><span class="sxs-lookup"><span data-stu-id="c4058-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessdeviceusageusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c4058-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4058-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessdeviceusageusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c4058-164">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c4058-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessdeviceusageusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c4058-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4058-165">Response</span></span>

<span data-ttu-id="c4058-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c4058-166">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="c4058-167">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="c4058-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Windows,Windows Phone,Android Phone,iPhone,iPad,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="c4058-168">JSON</span><span class="sxs-lookup"><span data-stu-id="c4058-168">JSON</span></span>

<span data-ttu-id="c4058-169">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="c4058-169">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="c4058-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4058-170">Request</span></span>

<span data-ttu-id="c4058-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c4058-171">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c4058-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4058-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusageusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c4058-173">C#</span><span class="sxs-lookup"><span data-stu-id="c4058-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessdeviceusageusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c4058-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4058-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessdeviceusageusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c4058-175">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c4058-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessdeviceusageusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c4058-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4058-176">Response</span></span>

<span data-ttu-id="c4058-177">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c4058-177">The following is an example of the response.</span></span>

> <span data-ttu-id="c4058-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c4058-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 289

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessDeviceUsageUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "windows": 403, 
      "windowsPhone": 2, 
      "androidPhone": 13, 
      "iPhone": 26, 
      "iPad": 0, 
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
