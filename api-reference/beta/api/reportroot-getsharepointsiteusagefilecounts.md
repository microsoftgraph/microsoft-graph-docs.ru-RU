---
title: 'reportRoot: getSharePointSiteUsageFileCounts'
description: Узнайте, сколько всего файлов на всех сайтах и сколько из них активны. Файл (пользователь или система) считается активным, если он был сохранен, синхронизирован, изменен или отправлен в указанный период.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: c92f842326e2ea420ff4b2b0397e320c4bd0230a
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869040"
---
# <a name="reportroot-getsharepointsiteusagefilecounts"></a><span data-ttu-id="13e51-104">reportRoot: getSharePointSiteUsageFileCounts</span><span class="sxs-lookup"><span data-stu-id="13e51-104">reportRoot: getSharePointSiteUsageFileCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13e51-105">Узнайте, сколько всего файлов на всех сайтах и сколько из них активны.</span><span class="sxs-lookup"><span data-stu-id="13e51-105">Get the total number of files across all sites and the number of active files.</span></span> <span data-ttu-id="13e51-106">Файл (пользователь или система) считается активным, если он был сохранен, синхронизирован, изменен в указанный период или им поделились в указанный период.</span><span class="sxs-lookup"><span data-stu-id="13e51-106">A file (user or system) is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span>

> <span data-ttu-id="13e51-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: использование сайтов SharePoint](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span><span class="sxs-lookup"><span data-stu-id="13e51-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="13e51-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="13e51-108">Permissions</span></span>

<span data-ttu-id="13e51-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13e51-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="13e51-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="13e51-111">Permission type</span></span>                        | <span data-ttu-id="13e51-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="13e51-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="13e51-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="13e51-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="13e51-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="13e51-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="13e51-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="13e51-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13e51-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13e51-116">Not supported.</span></span>                           |
| <span data-ttu-id="13e51-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="13e51-117">Application</span></span>                            | <span data-ttu-id="13e51-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="13e51-118">Reports.Read.All</span></span>                         |

<span data-ttu-id="13e51-119">**Примечание**. для делегированных разрешений, чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя, администратору клиента необходимо назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="13e51-119">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="13e51-120">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="13e51-120">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="13e51-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="13e51-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="13e51-122">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="13e51-122">Function parameters</span></span>

<span data-ttu-id="13e51-123">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="13e51-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="13e51-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="13e51-124">Parameter</span></span> | <span data-ttu-id="13e51-125">Тип</span><span class="sxs-lookup"><span data-stu-id="13e51-125">Type</span></span>   | <span data-ttu-id="13e51-126">Описание</span><span class="sxs-lookup"><span data-stu-id="13e51-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="13e51-127">period</span><span class="sxs-lookup"><span data-stu-id="13e51-127">period</span></span>    | <span data-ttu-id="13e51-128">string</span><span class="sxs-lookup"><span data-stu-id="13e51-128">string</span></span> | <span data-ttu-id="13e51-129">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="13e51-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="13e51-130">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="13e51-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="13e51-131">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="13e51-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="13e51-132">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="13e51-132">Required.</span></span> |

<span data-ttu-id="13e51-133">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="13e51-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="13e51-134">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="13e51-134">The default output type is text/csv.</span></span> <span data-ttu-id="13e51-135">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="13e51-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="13e51-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="13e51-136">Request headers</span></span>

| <span data-ttu-id="13e51-137">Имя</span><span class="sxs-lookup"><span data-stu-id="13e51-137">Name</span></span>          | <span data-ttu-id="13e51-138">Описание</span><span class="sxs-lookup"><span data-stu-id="13e51-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="13e51-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="13e51-139">Authorization</span></span> | <span data-ttu-id="13e51-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="13e51-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="13e51-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="13e51-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="13e51-143">CSV</span><span class="sxs-lookup"><span data-stu-id="13e51-143">CSV</span></span>

<span data-ttu-id="13e51-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="13e51-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="13e51-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="13e51-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="13e51-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="13e51-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="13e51-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="13e51-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="13e51-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="13e51-148">Report Refresh Date</span></span>
- <span data-ttu-id="13e51-149">"Site Type" (Тип сайта);</span><span class="sxs-lookup"><span data-stu-id="13e51-149">Site Type</span></span>
- <span data-ttu-id="13e51-150">"Total" (Всего);</span><span class="sxs-lookup"><span data-stu-id="13e51-150">Total</span></span>
- <span data-ttu-id="13e51-151">Active (активные)</span><span class="sxs-lookup"><span data-stu-id="13e51-151">Active</span></span>
- <span data-ttu-id="13e51-152">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="13e51-152">Report Date</span></span>
- <span data-ttu-id="13e51-153">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="13e51-153">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="13e51-154">JSON</span><span class="sxs-lookup"><span data-stu-id="13e51-154">JSON</span></span>

<span data-ttu-id="13e51-155">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[шарепоинтситеусажефилекаунтс](../resources/sharepointsiteusagefilecounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="13e51-155">If successful, this method returns a `200 OK` response code and a **[sharePointSiteUsageFileCounts](../resources/sharepointsiteusagefilecounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13e51-156">Пример</span><span class="sxs-lookup"><span data-stu-id="13e51-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="13e51-157">CSV</span><span class="sxs-lookup"><span data-stu-id="13e51-157">CSV</span></span>

<span data-ttu-id="13e51-158">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="13e51-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="13e51-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="13e51-159">Request</span></span>

<span data-ttu-id="13e51-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="13e51-160">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="13e51-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="13e51-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagefilecounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageFileCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="13e51-162">C#</span><span class="sxs-lookup"><span data-stu-id="13e51-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointsiteusagefilecounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="13e51-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="13e51-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointsiteusagefilecounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="13e51-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="13e51-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointsiteusagefilecounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="13e51-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="13e51-165">Response</span></span>

<span data-ttu-id="13e51-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="13e51-166">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="13e51-167">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="13e51-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Total,Active,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="13e51-168">JSON</span><span class="sxs-lookup"><span data-stu-id="13e51-168">JSON</span></span>

<span data-ttu-id="13e51-169">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="13e51-169">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="13e51-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="13e51-170">Request</span></span>

<span data-ttu-id="13e51-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="13e51-171">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="13e51-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="13e51-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagefilecounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageFileCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="13e51-173">C#</span><span class="sxs-lookup"><span data-stu-id="13e51-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointsiteusagefilecounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="13e51-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="13e51-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointsiteusagefilecounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="13e51-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="13e51-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointsiteusagefilecounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="13e51-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="13e51-176">Response</span></span>

<span data-ttu-id="13e51-177">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="13e51-177">The following is an example of the response.</span></span>

> <span data-ttu-id="13e51-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="13e51-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointSiteUsageFileCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 255

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.sharePointSiteUsageFileCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteType": "All", 
      "total": 25687, 
      "active": 209, 
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
