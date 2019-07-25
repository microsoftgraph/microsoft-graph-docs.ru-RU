---
title: 'reportRoot: getYammerGroupsActivityCounts'
description: Узнайте, сколько сообщений Yammer было опубликовано, прочитано и оценено в группах.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 8e072f72b8262beed85761269c544de7df2a5806
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871364"
---
# <a name="reportroot-getyammergroupsactivitycounts"></a><span data-ttu-id="fc0d6-103">reportRoot: getYammerGroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="fc0d6-103">reportRoot: getYammerGroupsActivityCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc0d6-104">Узнайте, сколько сообщений Yammer было опубликовано, прочитано и оценено в группах.</span><span class="sxs-lookup"><span data-stu-id="fc0d6-104">Get the number of Yammer messages posted, read, and liked in groups.</span></span>

> <span data-ttu-id="fc0d6-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия в группах Yammer](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span><span class="sxs-lookup"><span data-stu-id="fc0d6-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="fc0d6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fc0d6-106">Permissions</span></span>

<span data-ttu-id="fc0d6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc0d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fc0d6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fc0d6-109">Permission type</span></span>                        | <span data-ttu-id="fc0d6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fc0d6-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="fc0d6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fc0d6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="fc0d6-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fc0d6-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="fc0d6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fc0d6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc0d6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc0d6-114">Not supported.</span></span>                           |
| <span data-ttu-id="fc0d6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fc0d6-115">Application</span></span>                            | <span data-ttu-id="fc0d6-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fc0d6-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="fc0d6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fc0d6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="fc0d6-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="fc0d6-118">Function parameters</span></span>

<span data-ttu-id="fc0d6-119">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="fc0d6-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="fc0d6-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="fc0d6-120">Parameter</span></span> | <span data-ttu-id="fc0d6-121">Тип</span><span class="sxs-lookup"><span data-stu-id="fc0d6-121">Type</span></span>   | <span data-ttu-id="fc0d6-122">Описание</span><span class="sxs-lookup"><span data-stu-id="fc0d6-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="fc0d6-123">period</span><span class="sxs-lookup"><span data-stu-id="fc0d6-123">period</span></span>    | <span data-ttu-id="fc0d6-124">string</span><span class="sxs-lookup"><span data-stu-id="fc0d6-124">string</span></span> | <span data-ttu-id="fc0d6-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="fc0d6-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="fc0d6-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="fc0d6-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="fc0d6-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="fc0d6-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="fc0d6-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fc0d6-128">Required.</span></span> |

<span data-ttu-id="fc0d6-129">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="fc0d6-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="fc0d6-130">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="fc0d6-130">The default output type is text/csv.</span></span> <span data-ttu-id="fc0d6-131">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="fc0d6-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fc0d6-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fc0d6-132">Request headers</span></span>

| <span data-ttu-id="fc0d6-133">Имя</span><span class="sxs-lookup"><span data-stu-id="fc0d6-133">Name</span></span>          | <span data-ttu-id="fc0d6-134">Описание</span><span class="sxs-lookup"><span data-stu-id="fc0d6-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="fc0d6-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fc0d6-135">Authorization</span></span> | <span data-ttu-id="fc0d6-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fc0d6-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="fc0d6-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc0d6-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="fc0d6-139">CSV</span><span class="sxs-lookup"><span data-stu-id="fc0d6-139">CSV</span></span>

<span data-ttu-id="fc0d6-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="fc0d6-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="fc0d6-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="fc0d6-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="fc0d6-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="fc0d6-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="fc0d6-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="fc0d6-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="fc0d6-144">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="fc0d6-144">Report Refresh Date</span></span>
- <span data-ttu-id="fc0d6-145">"Liked" (Понравилось);</span><span class="sxs-lookup"><span data-stu-id="fc0d6-145">Liked</span></span>
- <span data-ttu-id="fc0d6-146">"Posted" (Опубликовано);</span><span class="sxs-lookup"><span data-stu-id="fc0d6-146">Posted</span></span>
- <span data-ttu-id="fc0d6-147">"Read" (Чтение);</span><span class="sxs-lookup"><span data-stu-id="fc0d6-147">Read</span></span>
- <span data-ttu-id="fc0d6-148">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="fc0d6-148">Report Date</span></span>
- <span data-ttu-id="fc0d6-149">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="fc0d6-149">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="fc0d6-150">JSON</span><span class="sxs-lookup"><span data-stu-id="fc0d6-150">JSON</span></span>

<span data-ttu-id="fc0d6-151">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[яммерграупсактивитикаунтс](../resources/yammergroupsactivitycounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fc0d6-151">If successful, this method returns a `200 OK` response code and a **[yammerGroupsActivityCounts](../resources/yammergroupsactivitycounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc0d6-152">Пример</span><span class="sxs-lookup"><span data-stu-id="fc0d6-152">Example</span></span>

### <a name="csv"></a><span data-ttu-id="fc0d6-153">CSV</span><span class="sxs-lookup"><span data-stu-id="fc0d6-153">CSV</span></span>

<span data-ttu-id="fc0d6-154">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="fc0d6-154">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="fc0d6-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc0d6-155">Request</span></span>

<span data-ttu-id="fc0d6-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fc0d6-156">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="fc0d6-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="fc0d6-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fc0d6-158">C#</span><span class="sxs-lookup"><span data-stu-id="fc0d6-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammergroupsactivitycounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fc0d6-159">Javascript</span><span class="sxs-lookup"><span data-stu-id="fc0d6-159">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammergroupsactivitycounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fc0d6-160">Цель — C</span><span class="sxs-lookup"><span data-stu-id="fc0d6-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammergroupsactivitycounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="fc0d6-161">Java</span><span class="sxs-lookup"><span data-stu-id="fc0d6-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getyammergroupsactivitycounts-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fc0d6-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc0d6-162">Response</span></span>

<span data-ttu-id="fc0d6-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fc0d6-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="fc0d6-164">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="fc0d6-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="fc0d6-165">JSON</span><span class="sxs-lookup"><span data-stu-id="fc0d6-165">JSON</span></span>

<span data-ttu-id="fc0d6-166">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="fc0d6-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="fc0d6-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc0d6-167">Request</span></span>

<span data-ttu-id="fc0d6-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fc0d6-168">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="fc0d6-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="fc0d6-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fc0d6-170">C#</span><span class="sxs-lookup"><span data-stu-id="fc0d6-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammergroupsactivitycounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fc0d6-171">Javascript</span><span class="sxs-lookup"><span data-stu-id="fc0d6-171">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammergroupsactivitycounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fc0d6-172">Цель — C</span><span class="sxs-lookup"><span data-stu-id="fc0d6-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammergroupsactivitycounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="fc0d6-173">Java</span><span class="sxs-lookup"><span data-stu-id="fc0d6-173">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getyammergroupsactivitycounts-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fc0d6-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc0d6-174">Response</span></span>

<span data-ttu-id="fc0d6-175">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="fc0d6-175">The following is an example of the response.</span></span>

> <span data-ttu-id="fc0d6-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fc0d6-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerGroupsActivityCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 241

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerGroupsActivityCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "liked": 13, 
      "posted": 50, 
      "read": 69, 
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
