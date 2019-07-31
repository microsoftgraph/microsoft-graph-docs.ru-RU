---
title: 'reportRoot: getYammerActivityCounts'
description: Отслеживайте динамику активности пользователей в Yammer по количеству опубликованных, прочитанных и понравившихся сообщений.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 14e608eed82d75a32ddf6195d76bbf6ca6dc8c72
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35991795"
---
# <a name="reportroot-getyammeractivitycounts"></a><span data-ttu-id="c38bd-103">reportRoot: getYammerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="c38bd-103">reportRoot: getYammerActivityCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c38bd-104">Отслеживайте динамику активности пользователей в Yammer по количеству опубликованных, прочитанных и понравившихся сообщений.</span><span class="sxs-lookup"><span data-stu-id="c38bd-104">Get the trends on the amount of Yammer activity in your organization by how many messages were posted, read, and liked.</span></span>

> <span data-ttu-id="c38bd-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span><span class="sxs-lookup"><span data-stu-id="c38bd-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="permissions"></a><span data-ttu-id="c38bd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c38bd-106">Permissions</span></span>

<span data-ttu-id="c38bd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c38bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c38bd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c38bd-109">Permission type</span></span>                        | <span data-ttu-id="c38bd-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c38bd-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="c38bd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c38bd-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c38bd-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c38bd-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="c38bd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c38bd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c38bd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c38bd-114">Not supported.</span></span>                           |
| <span data-ttu-id="c38bd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c38bd-115">Application</span></span>                            | <span data-ttu-id="c38bd-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c38bd-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="c38bd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c38bd-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="c38bd-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="c38bd-118">Function parameters</span></span>

<span data-ttu-id="c38bd-119">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="c38bd-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="c38bd-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="c38bd-120">Parameter</span></span> | <span data-ttu-id="c38bd-121">Тип</span><span class="sxs-lookup"><span data-stu-id="c38bd-121">Type</span></span>   | <span data-ttu-id="c38bd-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c38bd-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="c38bd-123">period</span><span class="sxs-lookup"><span data-stu-id="c38bd-123">period</span></span>    | <span data-ttu-id="c38bd-124">string</span><span class="sxs-lookup"><span data-stu-id="c38bd-124">string</span></span> | <span data-ttu-id="c38bd-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="c38bd-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="c38bd-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="c38bd-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="c38bd-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="c38bd-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="c38bd-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c38bd-128">Required.</span></span> |

<span data-ttu-id="c38bd-129">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="c38bd-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="c38bd-130">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="c38bd-130">The default output type is text/csv.</span></span> <span data-ttu-id="c38bd-131">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="c38bd-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c38bd-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c38bd-132">Request headers</span></span>

| <span data-ttu-id="c38bd-133">Имя</span><span class="sxs-lookup"><span data-stu-id="c38bd-133">Name</span></span>          | <span data-ttu-id="c38bd-134">Описание</span><span class="sxs-lookup"><span data-stu-id="c38bd-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="c38bd-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c38bd-135">Authorization</span></span> | <span data-ttu-id="c38bd-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c38bd-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="c38bd-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="c38bd-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="c38bd-139">CSV</span><span class="sxs-lookup"><span data-stu-id="c38bd-139">CSV</span></span>

<span data-ttu-id="c38bd-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="c38bd-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="c38bd-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="c38bd-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="c38bd-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="c38bd-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="c38bd-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="c38bd-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="c38bd-144">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="c38bd-144">Report Refresh Date</span></span>
- <span data-ttu-id="c38bd-145">"Liked" (Понравилось);</span><span class="sxs-lookup"><span data-stu-id="c38bd-145">Liked</span></span>
- <span data-ttu-id="c38bd-146">"Posted" (Опубликовано);</span><span class="sxs-lookup"><span data-stu-id="c38bd-146">Posted</span></span>
- <span data-ttu-id="c38bd-147">"Read" (Чтение);</span><span class="sxs-lookup"><span data-stu-id="c38bd-147">Read</span></span>
- <span data-ttu-id="c38bd-148">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="c38bd-148">Report Date</span></span>
- <span data-ttu-id="c38bd-149">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="c38bd-149">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="c38bd-150">JSON</span><span class="sxs-lookup"><span data-stu-id="c38bd-150">JSON</span></span>

<span data-ttu-id="c38bd-151">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[яммерактивитисуммари](../resources/yammeractivitysummary.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c38bd-151">If successful, this method returns a `200 OK` response code and a **[yammerActivitySummary](../resources/yammeractivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c38bd-152">Пример</span><span class="sxs-lookup"><span data-stu-id="c38bd-152">Example</span></span>

### <a name="csv"></a><span data-ttu-id="c38bd-153">CSV</span><span class="sxs-lookup"><span data-stu-id="c38bd-153">CSV</span></span>

<span data-ttu-id="c38bd-154">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="c38bd-154">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="c38bd-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="c38bd-155">Request</span></span>

<span data-ttu-id="c38bd-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c38bd-156">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c38bd-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="c38bd-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerActivityCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c38bd-158">C#</span><span class="sxs-lookup"><span data-stu-id="c38bd-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammeractivitycounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c38bd-159">Javascript</span><span class="sxs-lookup"><span data-stu-id="c38bd-159">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammeractivitycounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c38bd-160">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c38bd-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammeractivitycounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c38bd-161">Java</span><span class="sxs-lookup"><span data-stu-id="c38bd-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getyammeractivitycounts-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c38bd-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="c38bd-162">Response</span></span>

<span data-ttu-id="c38bd-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c38bd-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="c38bd-164">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="c38bd-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Liked,Posted,Read,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="c38bd-165">JSON</span><span class="sxs-lookup"><span data-stu-id="c38bd-165">JSON</span></span>

<span data-ttu-id="c38bd-166">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="c38bd-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="c38bd-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="c38bd-167">Request</span></span>

<span data-ttu-id="c38bd-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c38bd-168">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c38bd-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="c38bd-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerActivityCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c38bd-170">C#</span><span class="sxs-lookup"><span data-stu-id="c38bd-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammeractivitycounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c38bd-171">Javascript</span><span class="sxs-lookup"><span data-stu-id="c38bd-171">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammeractivitycounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c38bd-172">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c38bd-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammeractivitycounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c38bd-173">Java</span><span class="sxs-lookup"><span data-stu-id="c38bd-173">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getyammeractivitycounts-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c38bd-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="c38bd-174">Response</span></span>

<span data-ttu-id="c38bd-175">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c38bd-175">The following is an example of the response.</span></span>

> <span data-ttu-id="c38bd-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c38bd-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerActivitySummary"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 237

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerActivitySummary)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "liked": 47, 
      "posted": 59, 
      "read": 986, 
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
