---
title: 'reportRoot: getYammerActivityUserCounts'
description: Отслеживайте динамику по количеству уникальных пользователей, которые опубликовали, прочитали и оценили сообщения Yammer.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: fe885903afd321e0f76ba9c0e192912fb91762b4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35983107"
---
# <a name="reportroot-getyammeractivityusercounts"></a><span data-ttu-id="8f326-103">reportRoot: getYammerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="8f326-103">reportRoot: getYammerActivityUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f326-104">Отслеживайте динамику по количеству уникальных пользователей, которые опубликовали, прочитали и оценили сообщения Yammer.</span><span class="sxs-lookup"><span data-stu-id="8f326-104">Get the trends on the number of unique users who posted, read, and liked Yammer messages.</span></span>

> <span data-ttu-id="8f326-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span><span class="sxs-lookup"><span data-stu-id="8f326-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="permissions"></a><span data-ttu-id="8f326-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8f326-106">Permissions</span></span>

<span data-ttu-id="8f326-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f326-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8f326-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8f326-109">Permission type</span></span>                        | <span data-ttu-id="8f326-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8f326-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="8f326-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8f326-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8f326-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8f326-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="8f326-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8f326-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f326-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f326-114">Not supported.</span></span>                           |
| <span data-ttu-id="8f326-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8f326-115">Application</span></span>                            | <span data-ttu-id="8f326-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8f326-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="8f326-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8f326-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="8f326-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="8f326-118">Function parameters</span></span>

<span data-ttu-id="8f326-119">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="8f326-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="8f326-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="8f326-120">Parameter</span></span> | <span data-ttu-id="8f326-121">Тип</span><span class="sxs-lookup"><span data-stu-id="8f326-121">Type</span></span>   | <span data-ttu-id="8f326-122">Описание</span><span class="sxs-lookup"><span data-stu-id="8f326-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="8f326-123">period</span><span class="sxs-lookup"><span data-stu-id="8f326-123">period</span></span>    | <span data-ttu-id="8f326-124">string</span><span class="sxs-lookup"><span data-stu-id="8f326-124">string</span></span> | <span data-ttu-id="8f326-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="8f326-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="8f326-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="8f326-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="8f326-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="8f326-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="8f326-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8f326-128">Required.</span></span> |

<span data-ttu-id="8f326-129">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="8f326-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="8f326-130">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="8f326-130">The default output type is text/csv.</span></span> <span data-ttu-id="8f326-131">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="8f326-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8f326-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8f326-132">Request headers</span></span>

| <span data-ttu-id="8f326-133">Имя</span><span class="sxs-lookup"><span data-stu-id="8f326-133">Name</span></span>          | <span data-ttu-id="8f326-134">Описание</span><span class="sxs-lookup"><span data-stu-id="8f326-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="8f326-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8f326-135">Authorization</span></span> | <span data-ttu-id="8f326-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8f326-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="8f326-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f326-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="8f326-139">CSV</span><span class="sxs-lookup"><span data-stu-id="8f326-139">CSV</span></span>

<span data-ttu-id="8f326-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="8f326-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="8f326-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="8f326-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="8f326-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="8f326-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="8f326-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="8f326-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="8f326-144">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="8f326-144">Report Refresh Date</span></span>
- <span data-ttu-id="8f326-145">"Liked" (Понравилось);</span><span class="sxs-lookup"><span data-stu-id="8f326-145">Liked</span></span>
- <span data-ttu-id="8f326-146">"Posted" (Опубликовано);</span><span class="sxs-lookup"><span data-stu-id="8f326-146">Posted</span></span>
- <span data-ttu-id="8f326-147">"Read" (Чтение);</span><span class="sxs-lookup"><span data-stu-id="8f326-147">Read</span></span>
- <span data-ttu-id="8f326-148">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="8f326-148">Report Date</span></span>
- <span data-ttu-id="8f326-149">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="8f326-149">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="8f326-150">JSON</span><span class="sxs-lookup"><span data-stu-id="8f326-150">JSON</span></span>

<span data-ttu-id="8f326-151">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[яммерактивитисуммари](../resources/yammeractivitysummary.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8f326-151">If successful, this method returns a `200 OK` response code and a **[yammerActivitySummary](../resources/yammeractivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f326-152">Пример</span><span class="sxs-lookup"><span data-stu-id="8f326-152">Example</span></span>

### <a name="csv"></a><span data-ttu-id="8f326-153">CSV</span><span class="sxs-lookup"><span data-stu-id="8f326-153">CSV</span></span>

<span data-ttu-id="8f326-154">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="8f326-154">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="8f326-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f326-155">Request</span></span>

<span data-ttu-id="8f326-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8f326-156">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8f326-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="8f326-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerActivityUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8f326-158">C#</span><span class="sxs-lookup"><span data-stu-id="8f326-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammeractivityusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8f326-159">Javascript</span><span class="sxs-lookup"><span data-stu-id="8f326-159">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammeractivityusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8f326-160">Цель — C</span><span class="sxs-lookup"><span data-stu-id="8f326-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammeractivityusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8f326-161">Java</span><span class="sxs-lookup"><span data-stu-id="8f326-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getyammeractivityusercounts-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8f326-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f326-162">Response</span></span>

<span data-ttu-id="8f326-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8f326-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="8f326-164">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="8f326-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="8f326-165">JSON</span><span class="sxs-lookup"><span data-stu-id="8f326-165">JSON</span></span>

<span data-ttu-id="8f326-166">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="8f326-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="8f326-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f326-167">Request</span></span>

<span data-ttu-id="8f326-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8f326-168">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8f326-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="8f326-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerActivityUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8f326-170">C#</span><span class="sxs-lookup"><span data-stu-id="8f326-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammeractivityusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8f326-171">Javascript</span><span class="sxs-lookup"><span data-stu-id="8f326-171">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammeractivityusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8f326-172">Цель — C</span><span class="sxs-lookup"><span data-stu-id="8f326-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammeractivityusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8f326-173">Java</span><span class="sxs-lookup"><span data-stu-id="8f326-173">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getyammeractivityusercounts-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8f326-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f326-174">Response</span></span>

<span data-ttu-id="8f326-175">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8f326-175">The following is an example of the response.</span></span>

> <span data-ttu-id="8f326-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8f326-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerActivitySummary"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 236

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerActivitySummary)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "liked": 40, 
      "posted": 54, 
      "read": 28, 
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
