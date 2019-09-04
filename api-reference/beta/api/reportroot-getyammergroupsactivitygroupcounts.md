---
title: 'reportRoot: getYammerGroupsActivityGroupCounts'
description: Узнайте, сколько всего существовало групп и в скольких из них выполнялись действия с беседами.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 1421771cbfcb6b75cae72b9aa32f414eb2110958
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36724836"
---
# <a name="reportroot-getyammergroupsactivitygroupcounts"></a><span data-ttu-id="92644-103">reportRoot: getYammerGroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="92644-103">reportRoot: getYammerGroupsActivityGroupCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92644-104">Узнайте, сколько всего существовало групп и в скольких из них выполнялись действия с беседами.</span><span class="sxs-lookup"><span data-stu-id="92644-104">Get the total number of groups that existed and how many included group conversation activity.</span></span>

> <span data-ttu-id="92644-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия в группах Yammer](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span><span class="sxs-lookup"><span data-stu-id="92644-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="92644-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="92644-106">Permissions</span></span>

<span data-ttu-id="92644-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92644-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="92644-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="92644-109">Permission type</span></span>                        | <span data-ttu-id="92644-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="92644-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="92644-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="92644-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="92644-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="92644-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="92644-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="92644-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92644-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92644-114">Not supported.</span></span>                           |
| <span data-ttu-id="92644-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="92644-115">Application</span></span>                            | <span data-ttu-id="92644-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="92644-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="92644-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="92644-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityGroupCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="92644-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="92644-118">Function parameters</span></span>

<span data-ttu-id="92644-119">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="92644-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="92644-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="92644-120">Parameter</span></span> | <span data-ttu-id="92644-121">Тип</span><span class="sxs-lookup"><span data-stu-id="92644-121">Type</span></span>   | <span data-ttu-id="92644-122">Описание</span><span class="sxs-lookup"><span data-stu-id="92644-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="92644-123">period</span><span class="sxs-lookup"><span data-stu-id="92644-123">period</span></span>    | <span data-ttu-id="92644-124">string</span><span class="sxs-lookup"><span data-stu-id="92644-124">string</span></span> | <span data-ttu-id="92644-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="92644-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="92644-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="92644-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="92644-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="92644-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="92644-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="92644-128">Required.</span></span> |

<span data-ttu-id="92644-129">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="92644-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="92644-130">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="92644-130">The default output type is text/csv.</span></span> <span data-ttu-id="92644-131">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="92644-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="92644-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="92644-132">Request headers</span></span>

| <span data-ttu-id="92644-133">Имя</span><span class="sxs-lookup"><span data-stu-id="92644-133">Name</span></span>          | <span data-ttu-id="92644-134">Описание</span><span class="sxs-lookup"><span data-stu-id="92644-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="92644-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="92644-135">Authorization</span></span> | <span data-ttu-id="92644-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="92644-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="92644-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="92644-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="92644-139">CSV</span><span class="sxs-lookup"><span data-stu-id="92644-139">CSV</span></span>

<span data-ttu-id="92644-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="92644-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="92644-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="92644-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="92644-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="92644-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="92644-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="92644-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="92644-144">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="92644-144">Report Refresh Date</span></span>
- <span data-ttu-id="92644-145">Total (всего)</span><span class="sxs-lookup"><span data-stu-id="92644-145">Total</span></span>
- <span data-ttu-id="92644-146">Active (активные)</span><span class="sxs-lookup"><span data-stu-id="92644-146">Active</span></span>
- <span data-ttu-id="92644-147">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="92644-147">Report Date</span></span>
- <span data-ttu-id="92644-148">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="92644-148">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="92644-149">JSON</span><span class="sxs-lookup"><span data-stu-id="92644-149">JSON</span></span>

<span data-ttu-id="92644-150">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[яммерграупсактивитиграупкаунтс](../resources/yammergroupsactivitygroupcounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="92644-150">If successful, this method returns a `200 OK` response code and a **[yammerGroupsActivityGroupCounts](../resources/yammergroupsactivitygroupcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92644-151">Пример</span><span class="sxs-lookup"><span data-stu-id="92644-151">Example</span></span>

### <a name="csv"></a><span data-ttu-id="92644-152">CSV</span><span class="sxs-lookup"><span data-stu-id="92644-152">CSV</span></span>

<span data-ttu-id="92644-153">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="92644-153">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="92644-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="92644-154">Request</span></span>

<span data-ttu-id="92644-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="92644-155">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="92644-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="92644-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitygroupcounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityGroupCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="92644-157">C#</span><span class="sxs-lookup"><span data-stu-id="92644-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammergroupsactivitygroupcounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="92644-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92644-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammergroupsactivitygroupcounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="92644-159">Цель — C</span><span class="sxs-lookup"><span data-stu-id="92644-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammergroupsactivitygroupcounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="92644-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="92644-160">Response</span></span>

<span data-ttu-id="92644-161">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="92644-161">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="92644-162">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="92644-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Total,Active,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="92644-163">JSON</span><span class="sxs-lookup"><span data-stu-id="92644-163">JSON</span></span>

<span data-ttu-id="92644-164">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="92644-164">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="92644-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="92644-165">Request</span></span>

<span data-ttu-id="92644-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="92644-166">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="92644-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="92644-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitygroupcounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityGroupCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="92644-168">C#</span><span class="sxs-lookup"><span data-stu-id="92644-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammergroupsactivitygroupcounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="92644-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92644-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammergroupsactivitygroupcounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="92644-170">Цель — C</span><span class="sxs-lookup"><span data-stu-id="92644-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammergroupsactivitygroupcounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="92644-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="92644-171">Response</span></span>

<span data-ttu-id="92644-172">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="92644-172">The following is an example of the response.</span></span>

> <span data-ttu-id="92644-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="92644-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerGroupsActivityGroupCounts",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 236

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerGroupsActivityGroupCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01",
      "total": 50, 
      "active": 41, 
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
