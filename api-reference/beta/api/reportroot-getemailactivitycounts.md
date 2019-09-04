---
title: 'reportRoot: getEmailActivityCounts'
description: Позволяет понять динамику работы с электронной почтой (сколько писем было отправлено, прочитано и получено) в организации.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 0f7b5c5a471a0423f92e3a005b4bfeab20ac83a0
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36725376"
---
# <a name="reportroot-getemailactivitycounts"></a><span data-ttu-id="2f28c-103">reportRoot: getEmailActivityCounts</span><span class="sxs-lookup"><span data-stu-id="2f28c-103">reportRoot: getEmailActivityCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f28c-104">Позволяет понять динамику работы с электронной почтой (сколько писем было отправлено, прочитано и получено) в организации.</span><span class="sxs-lookup"><span data-stu-id="2f28c-104">Enables you to understand the trends of email activity (like how many were sent, read, and received) in your organization.</span></span>

> <span data-ttu-id="2f28c-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span><span class="sxs-lookup"><span data-stu-id="2f28c-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="permissions"></a><span data-ttu-id="2f28c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2f28c-106">Permissions</span></span>

<span data-ttu-id="2f28c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f28c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2f28c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2f28c-109">Permission type</span></span>                        | <span data-ttu-id="2f28c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2f28c-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="2f28c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2f28c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2f28c-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f28c-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="2f28c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2f28c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f28c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f28c-114">Not supported.</span></span>                           |
| <span data-ttu-id="2f28c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2f28c-115">Application</span></span>                            | <span data-ttu-id="2f28c-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f28c-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="2f28c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2f28c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="2f28c-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="2f28c-118">Function parameters</span></span>

<span data-ttu-id="2f28c-119">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="2f28c-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="2f28c-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="2f28c-120">Parameter</span></span> | <span data-ttu-id="2f28c-121">Тип</span><span class="sxs-lookup"><span data-stu-id="2f28c-121">Type</span></span>   | <span data-ttu-id="2f28c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="2f28c-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="2f28c-123">period</span><span class="sxs-lookup"><span data-stu-id="2f28c-123">period</span></span>    | <span data-ttu-id="2f28c-124">string</span><span class="sxs-lookup"><span data-stu-id="2f28c-124">string</span></span> | <span data-ttu-id="2f28c-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="2f28c-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="2f28c-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="2f28c-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="2f28c-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="2f28c-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="2f28c-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2f28c-128">Required.</span></span> |

<span data-ttu-id="2f28c-129">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="2f28c-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="2f28c-130">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="2f28c-130">The default output type is text/csv.</span></span> <span data-ttu-id="2f28c-131">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="2f28c-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2f28c-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2f28c-132">Request headers</span></span>

| <span data-ttu-id="2f28c-133">Имя</span><span class="sxs-lookup"><span data-stu-id="2f28c-133">Name</span></span>          | <span data-ttu-id="2f28c-134">Описание</span><span class="sxs-lookup"><span data-stu-id="2f28c-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="2f28c-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2f28c-135">Authorization</span></span> | <span data-ttu-id="2f28c-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2f28c-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="2f28c-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f28c-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="2f28c-139">CSV</span><span class="sxs-lookup"><span data-stu-id="2f28c-139">CSV</span></span>

<span data-ttu-id="2f28c-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="2f28c-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="2f28c-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="2f28c-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="2f28c-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="2f28c-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="2f28c-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="2f28c-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="2f28c-144">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="2f28c-144">Report Refresh Date</span></span>
- <span data-ttu-id="2f28c-145">Send (отправлено)</span><span class="sxs-lookup"><span data-stu-id="2f28c-145">Send</span></span>
- <span data-ttu-id="2f28c-146">Receive (получено)</span><span class="sxs-lookup"><span data-stu-id="2f28c-146">Receive</span></span>
- <span data-ttu-id="2f28c-147">Read (прочитано)</span><span class="sxs-lookup"><span data-stu-id="2f28c-147">Read</span></span>
- <span data-ttu-id="2f28c-148">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="2f28c-148">Report Date</span></span>
- <span data-ttu-id="2f28c-149">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="2f28c-149">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="2f28c-150">JSON</span><span class="sxs-lookup"><span data-stu-id="2f28c-150">JSON</span></span>

<span data-ttu-id="2f28c-151">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[емаилактивитисуммари](../resources/emailactivitysummary.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2f28c-151">If successful, this method returns a `200 OK` response code and an **[emailActivitySummary](../resources/emailactivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f28c-152">Пример</span><span class="sxs-lookup"><span data-stu-id="2f28c-152">Example</span></span>

### <a name="csv"></a><span data-ttu-id="2f28c-153">CSV</span><span class="sxs-lookup"><span data-stu-id="2f28c-153">CSV</span></span>

<span data-ttu-id="2f28c-154">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="2f28c-154">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="2f28c-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="2f28c-155">Request</span></span>

<span data-ttu-id="2f28c-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2f28c-156">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="2f28c-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="2f28c-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getemailactivitycounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getEmailActivityCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2f28c-158">C#</span><span class="sxs-lookup"><span data-stu-id="2f28c-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailactivitycounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2f28c-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2f28c-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailactivitycounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2f28c-160">Цель — C</span><span class="sxs-lookup"><span data-stu-id="2f28c-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailactivitycounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2f28c-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f28c-161">Response</span></span>

<span data-ttu-id="2f28c-162">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2f28c-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="2f28c-163">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="2f28c-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Send,Receive,Read,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="2f28c-164">JSON</span><span class="sxs-lookup"><span data-stu-id="2f28c-164">JSON</span></span>

<span data-ttu-id="2f28c-165">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="2f28c-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="2f28c-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="2f28c-166">Request</span></span>

<span data-ttu-id="2f28c-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2f28c-167">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="2f28c-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="2f28c-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getemailactivitycounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getEmailActivityCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2f28c-169">C#</span><span class="sxs-lookup"><span data-stu-id="2f28c-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailactivitycounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2f28c-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2f28c-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailactivitycounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2f28c-171">Цель — C</span><span class="sxs-lookup"><span data-stu-id="2f28c-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailactivitycounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2f28c-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f28c-172">Response</span></span>

<span data-ttu-id="2f28c-173">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2f28c-173">The following is an example of the response.</span></span>

> <span data-ttu-id="2f28c-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2f28c-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailActivitySummary"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 242

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailActivitySummary)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "send": 504, 
      "receive": 76506, 
      "read": 12161, 
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
