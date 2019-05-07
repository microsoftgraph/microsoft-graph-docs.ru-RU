---
title: 'reportRoot: getOffice365GroupsActivityGroupCounts'
description: Узнайте, сколько всего групп в организации и сколько из них были активны на основе цепочек сообщений, публикаций в Yammer и действий с файлами SharePoint за день.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 755363513fb916e2f2125dd665dc6e0032966289
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33639406"
---
# <a name="reportroot-getoffice365groupsactivitygroupcounts"></a><span data-ttu-id="fd7bf-103">reportRoot: getOffice365GroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="fd7bf-103">reportRoot: getOffice365GroupsActivityGroupCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd7bf-104">Узнайте, сколько всего групп в организации и сколько из них были активны на основе цепочек сообщений, публикаций в Yammer и действий с файлами SharePoint за день.</span><span class="sxs-lookup"><span data-stu-id="fd7bf-104">Get the daily total number of groups and how many of them were active based on email conversations, Yammer posts, and SharePoint file activities.</span></span>

> <span data-ttu-id="fd7bf-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="fd7bf-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="fd7bf-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fd7bf-106">Permissions</span></span>

<span data-ttu-id="fd7bf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd7bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fd7bf-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fd7bf-109">Permission type</span></span>                        | <span data-ttu-id="fd7bf-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fd7bf-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="fd7bf-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fd7bf-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="fd7bf-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fd7bf-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="fd7bf-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fd7bf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd7bf-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd7bf-114">Not supported.</span></span>                           |
| <span data-ttu-id="fd7bf-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fd7bf-115">Application</span></span>                            | <span data-ttu-id="fd7bf-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fd7bf-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="fd7bf-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fd7bf-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityGroupCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="fd7bf-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="fd7bf-118">Function parameters</span></span>

<span data-ttu-id="fd7bf-119">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="fd7bf-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="fd7bf-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="fd7bf-120">Parameter</span></span> | <span data-ttu-id="fd7bf-121">Тип</span><span class="sxs-lookup"><span data-stu-id="fd7bf-121">Type</span></span>   | <span data-ttu-id="fd7bf-122">Описание</span><span class="sxs-lookup"><span data-stu-id="fd7bf-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="fd7bf-123">period</span><span class="sxs-lookup"><span data-stu-id="fd7bf-123">period</span></span>    | <span data-ttu-id="fd7bf-124">string</span><span class="sxs-lookup"><span data-stu-id="fd7bf-124">string</span></span> | <span data-ttu-id="fd7bf-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="fd7bf-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="fd7bf-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="fd7bf-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="fd7bf-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="fd7bf-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="fd7bf-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fd7bf-128">Required.</span></span> |

<span data-ttu-id="fd7bf-129">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="fd7bf-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="fd7bf-130">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="fd7bf-130">The default output type is text/csv.</span></span> <span data-ttu-id="fd7bf-131">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="fd7bf-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fd7bf-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fd7bf-132">Request headers</span></span>

| <span data-ttu-id="fd7bf-133">Имя</span><span class="sxs-lookup"><span data-stu-id="fd7bf-133">Name</span></span>          | <span data-ttu-id="fd7bf-134">Описание</span><span class="sxs-lookup"><span data-stu-id="fd7bf-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="fd7bf-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fd7bf-135">Authorization</span></span> | <span data-ttu-id="fd7bf-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fd7bf-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="fd7bf-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd7bf-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="fd7bf-139">CSV</span><span class="sxs-lookup"><span data-stu-id="fd7bf-139">CSV</span></span>

<span data-ttu-id="fd7bf-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="fd7bf-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="fd7bf-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="fd7bf-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="fd7bf-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="fd7bf-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="fd7bf-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="fd7bf-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="fd7bf-144">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="fd7bf-144">Report Refresh Date</span></span>
- <span data-ttu-id="fd7bf-145">Total (всего)</span><span class="sxs-lookup"><span data-stu-id="fd7bf-145">Total</span></span>
- <span data-ttu-id="fd7bf-146">Active (активные)</span><span class="sxs-lookup"><span data-stu-id="fd7bf-146">Active</span></span>
- <span data-ttu-id="fd7bf-147">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="fd7bf-147">Report Date</span></span>
- <span data-ttu-id="fd7bf-148">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="fd7bf-148">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="fd7bf-149">JSON</span><span class="sxs-lookup"><span data-stu-id="fd7bf-149">JSON</span></span>

<span data-ttu-id="fd7bf-150">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[office365GroupsActivityGroupCounts](../resources/office365groupsactivitygroupcounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fd7bf-150">If successful, this method returns a `200 OK` response code and an **[office365GroupsActivityGroupCounts](../resources/office365groupsactivitygroupcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd7bf-151">Пример</span><span class="sxs-lookup"><span data-stu-id="fd7bf-151">Example</span></span>

### <a name="csv"></a><span data-ttu-id="fd7bf-152">CSV</span><span class="sxs-lookup"><span data-stu-id="fd7bf-152">CSV</span></span>

<span data-ttu-id="fd7bf-153">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="fd7bf-153">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="fd7bf-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="fd7bf-154">Request</span></span>

<span data-ttu-id="fd7bf-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fd7bf-155">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitygroupcounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityGroupCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="fd7bf-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd7bf-156">Response</span></span>

<span data-ttu-id="fd7bf-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fd7bf-157">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="fd7bf-158">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="fd7bf-158">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="fd7bf-159">Языках</span><span class="sxs-lookup"><span data-stu-id="fd7bf-159">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365groupsactivitygroupcounts_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fd7bf-160">Язык</span><span class="sxs-lookup"><span data-stu-id="fd7bf-160">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365groupsactivitygroupcounts_csv-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="fd7bf-161">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="fd7bf-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="fd7bf-162">JSON</span><span class="sxs-lookup"><span data-stu-id="fd7bf-162">JSON</span></span>

<span data-ttu-id="fd7bf-163">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="fd7bf-163">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="fd7bf-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="fd7bf-164">Request</span></span>

<span data-ttu-id="fd7bf-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fd7bf-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitygroupcounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityGroupCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="fd7bf-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd7bf-166">Response</span></span>

<span data-ttu-id="fd7bf-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fd7bf-167">The following is an example of the response.</span></span>

> <span data-ttu-id="fd7bf-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fd7bf-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365GroupsActivityGroupCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 240

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365GroupsActivityGroupCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "total": 5344, 
      "active": 0, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="fd7bf-170">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="fd7bf-170">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="fd7bf-171">Языках</span><span class="sxs-lookup"><span data-stu-id="fd7bf-171">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365groupsactivitygroupcounts_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fd7bf-172">Язык</span><span class="sxs-lookup"><span data-stu-id="fd7bf-172">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365groupsactivitygroupcounts_json-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getoffice365groupsactivitygroupcounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getoffice365groupsactivitygroupcounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getoffice365groupsactivitygroupcounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getoffice365groupsactivitygroupcounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
