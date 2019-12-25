---
title: 'reportRoot: getSharePointSiteUsagePages'
description: Узнайте, сколько страниц было просмотрено на всех сайтах.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 75e5393c20181b04bb4291761738d0a10f5dfb4e
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867409"
---
# <a name="reportroot-getsharepointsiteusagepages"></a><span data-ttu-id="22956-103">reportRoot: getSharePointSiteUsagePages</span><span class="sxs-lookup"><span data-stu-id="22956-103">reportRoot: getSharePointSiteUsagePages</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22956-104">Узнайте, сколько страниц было просмотрено на всех сайтах.</span><span class="sxs-lookup"><span data-stu-id="22956-104">Get the number of pages viewed across all sites.</span></span>

> <span data-ttu-id="22956-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: использование сайтов SharePoint](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span><span class="sxs-lookup"><span data-stu-id="22956-105">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="22956-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="22956-106">Permissions</span></span>

<span data-ttu-id="22956-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22956-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="22956-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="22956-109">Permission type</span></span>                        | <span data-ttu-id="22956-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="22956-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="22956-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="22956-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="22956-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="22956-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="22956-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="22956-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22956-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22956-114">Not supported.</span></span>                           |
| <span data-ttu-id="22956-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="22956-115">Application</span></span>                            | <span data-ttu-id="22956-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="22956-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="22956-117">**Примечание**. для делегированных разрешений, чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя, администратору клиента необходимо назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="22956-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="22956-118">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="22956-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="22956-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="22956-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsagePages(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="22956-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="22956-120">Function parameters</span></span>

<span data-ttu-id="22956-121">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="22956-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="22956-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="22956-122">Parameter</span></span> | <span data-ttu-id="22956-123">Тип</span><span class="sxs-lookup"><span data-stu-id="22956-123">Type</span></span>   | <span data-ttu-id="22956-124">Описание</span><span class="sxs-lookup"><span data-stu-id="22956-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="22956-125">period</span><span class="sxs-lookup"><span data-stu-id="22956-125">period</span></span>    | <span data-ttu-id="22956-126">string</span><span class="sxs-lookup"><span data-stu-id="22956-126">string</span></span> | <span data-ttu-id="22956-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="22956-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="22956-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="22956-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="22956-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="22956-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="22956-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="22956-130">Required.</span></span> |

<span data-ttu-id="22956-131">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="22956-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="22956-132">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="22956-132">The default output type is text/csv.</span></span> <span data-ttu-id="22956-133">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="22956-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="22956-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="22956-134">Request headers</span></span>

| <span data-ttu-id="22956-135">Имя</span><span class="sxs-lookup"><span data-stu-id="22956-135">Name</span></span>          | <span data-ttu-id="22956-136">Описание</span><span class="sxs-lookup"><span data-stu-id="22956-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="22956-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="22956-137">Authorization</span></span> | <span data-ttu-id="22956-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="22956-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="22956-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="22956-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="22956-141">CSV</span><span class="sxs-lookup"><span data-stu-id="22956-141">CSV</span></span>

<span data-ttu-id="22956-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="22956-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="22956-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="22956-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="22956-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="22956-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="22956-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="22956-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="22956-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="22956-146">Report Refresh Date</span></span>
- <span data-ttu-id="22956-147">"Site Type" (Тип сайта);</span><span class="sxs-lookup"><span data-stu-id="22956-147">Site Type</span></span>
- <span data-ttu-id="22956-148">"Page View Count" (Количество просмотров страницы);</span><span class="sxs-lookup"><span data-stu-id="22956-148">Page View Count</span></span>
- <span data-ttu-id="22956-149">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="22956-149">Report Date</span></span>
- <span data-ttu-id="22956-150">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="22956-150">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="22956-151">JSON</span><span class="sxs-lookup"><span data-stu-id="22956-151">JSON</span></span>

<span data-ttu-id="22956-152">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[шарепоинтситеусажепажес](../resources/sharepointsiteusagepages.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="22956-152">If successful, this method returns a `200 OK` response code and a **[sharePointSiteUsagePages](../resources/sharepointsiteusagepages.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22956-153">Пример</span><span class="sxs-lookup"><span data-stu-id="22956-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="22956-154">CSV</span><span class="sxs-lookup"><span data-stu-id="22956-154">CSV</span></span>

<span data-ttu-id="22956-155">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="22956-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="22956-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="22956-156">Request</span></span>

<span data-ttu-id="22956-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="22956-157">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="22956-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="22956-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagepages_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsagePages(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="22956-159">C#</span><span class="sxs-lookup"><span data-stu-id="22956-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointsiteusagepages-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="22956-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="22956-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointsiteusagepages-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="22956-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="22956-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointsiteusagepages-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="22956-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="22956-162">Response</span></span>

<span data-ttu-id="22956-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="22956-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="22956-164">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="22956-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Page View Count,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="22956-165">JSON</span><span class="sxs-lookup"><span data-stu-id="22956-165">JSON</span></span>

<span data-ttu-id="22956-166">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="22956-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="22956-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="22956-167">Request</span></span>

<span data-ttu-id="22956-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="22956-168">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="22956-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="22956-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagepages_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsagePages(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="22956-170">C#</span><span class="sxs-lookup"><span data-stu-id="22956-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointsiteusagepages-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="22956-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="22956-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointsiteusagepages-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="22956-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="22956-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointsiteusagepages-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="22956-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="22956-173">Response</span></span>

<span data-ttu-id="22956-174">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="22956-174">The following is an example of the response.</span></span>

> <span data-ttu-id="22956-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="22956-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointSiteUsagePages"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 243

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.sharePointSiteUsagePages)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteType": "All", 
      "pageViewCount": 183, 
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
