---
title: 'reportRoot: getOffice365GroupsActivityCounts'
description: Узнайте, сколько различных действий было в группах.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 8826e5af9752185a3668cbe45c40d6423f0f7030
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35267356"
---
# <a name="reportroot-getoffice365groupsactivitycounts"></a><span data-ttu-id="02fdf-103">reportRoot: getOffice365GroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="02fdf-103">reportRoot: getOffice365GroupsActivityCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02fdf-104">Узнайте, сколько различных действий было в группах.</span><span class="sxs-lookup"><span data-stu-id="02fdf-104">Get the number of group activities across group workloads.</span></span>

> <span data-ttu-id="02fdf-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="02fdf-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="02fdf-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="02fdf-106">Permissions</span></span>

<span data-ttu-id="02fdf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02fdf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="02fdf-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="02fdf-109">Permission type</span></span>                        | <span data-ttu-id="02fdf-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="02fdf-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="02fdf-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="02fdf-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="02fdf-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="02fdf-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="02fdf-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="02fdf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02fdf-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02fdf-114">Not supported.</span></span>                           |
| <span data-ttu-id="02fdf-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="02fdf-115">Application</span></span>                            | <span data-ttu-id="02fdf-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="02fdf-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="02fdf-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="02fdf-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="02fdf-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="02fdf-118">Function parameters</span></span>

<span data-ttu-id="02fdf-119">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="02fdf-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="02fdf-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="02fdf-120">Parameter</span></span> | <span data-ttu-id="02fdf-121">Тип</span><span class="sxs-lookup"><span data-stu-id="02fdf-121">Type</span></span>   | <span data-ttu-id="02fdf-122">Описание</span><span class="sxs-lookup"><span data-stu-id="02fdf-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="02fdf-123">period</span><span class="sxs-lookup"><span data-stu-id="02fdf-123">period</span></span>    | <span data-ttu-id="02fdf-124">string</span><span class="sxs-lookup"><span data-stu-id="02fdf-124">string</span></span> | <span data-ttu-id="02fdf-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="02fdf-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="02fdf-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="02fdf-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="02fdf-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="02fdf-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="02fdf-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="02fdf-128">Required.</span></span> |

<span data-ttu-id="02fdf-129">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="02fdf-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="02fdf-130">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="02fdf-130">The default output type is text/csv.</span></span> <span data-ttu-id="02fdf-131">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="02fdf-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="02fdf-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="02fdf-132">Request headers</span></span>

| <span data-ttu-id="02fdf-133">Имя</span><span class="sxs-lookup"><span data-stu-id="02fdf-133">Name</span></span>          | <span data-ttu-id="02fdf-134">Описание</span><span class="sxs-lookup"><span data-stu-id="02fdf-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="02fdf-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="02fdf-135">Authorization</span></span> | <span data-ttu-id="02fdf-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="02fdf-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="02fdf-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="02fdf-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="02fdf-139">CSV</span><span class="sxs-lookup"><span data-stu-id="02fdf-139">CSV</span></span>

<span data-ttu-id="02fdf-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="02fdf-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="02fdf-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="02fdf-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="02fdf-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="02fdf-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="02fdf-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="02fdf-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="02fdf-144">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="02fdf-144">Report Refresh Date</span></span>
- <span data-ttu-id="02fdf-145">Exchange Emails Received (получено писем Exchange)</span><span class="sxs-lookup"><span data-stu-id="02fdf-145">Exchange Emails Received</span></span>
- <span data-ttu-id="02fdf-146">Yammer Messages Posted (опубликовано сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="02fdf-146">Yammer Messages Posted</span></span>
- <span data-ttu-id="02fdf-147">Yammer Messages Read (прочитано сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="02fdf-147">Yammer Messages Read</span></span>
- <span data-ttu-id="02fdf-148">Yammer Messages Liked (понравилось сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="02fdf-148">Yammer Messages Liked</span></span>
- <span data-ttu-id="02fdf-149">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="02fdf-149">Report Date</span></span>
- <span data-ttu-id="02fdf-150">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="02fdf-150">Report Period</span></span>

<span data-ttu-id="02fdf-151">Следующие столбцы не поддерживаются в Китае Microsoft Graph, предоставляемом компанией 21Vianet:</span><span class="sxs-lookup"><span data-stu-id="02fdf-151">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="02fdf-152">Yammer Messages Posted (опубликовано сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="02fdf-152">Yammer Messages Posted</span></span>
- <span data-ttu-id="02fdf-153">Yammer Messages Read (прочитано сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="02fdf-153">Yammer Messages Read</span></span>
- <span data-ttu-id="02fdf-154">Yammer Messages Liked (понравилось сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="02fdf-154">Yammer Messages Liked</span></span>

### <a name="json"></a><span data-ttu-id="02fdf-155">JSON</span><span class="sxs-lookup"><span data-stu-id="02fdf-155">JSON</span></span>

<span data-ttu-id="02fdf-156">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="02fdf-156">If successful, this method returns a `200 OK` response code and an **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** object in the response body.</span></span>

<span data-ttu-id="02fdf-157">Следующие свойства в объекте **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** не поддерживаются в Китае Microsoft Graph, предоставляемом компанией 21vianet:</span><span class="sxs-lookup"><span data-stu-id="02fdf-157">The following properties in **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="02fdf-158">Яммермессажеспостед</span><span class="sxs-lookup"><span data-stu-id="02fdf-158">yammerMessagesPosted</span></span>
- <span data-ttu-id="02fdf-159">Яммермессажесреад</span><span class="sxs-lookup"><span data-stu-id="02fdf-159">yammerMessagesRead</span></span>
- <span data-ttu-id="02fdf-160">Яммермессажесликед</span><span class="sxs-lookup"><span data-stu-id="02fdf-160">yammerMessagesLiked</span></span>

## <a name="example"></a><span data-ttu-id="02fdf-161">Пример</span><span class="sxs-lookup"><span data-stu-id="02fdf-161">Example</span></span>

### <a name="csv"></a><span data-ttu-id="02fdf-162">CSV</span><span class="sxs-lookup"><span data-stu-id="02fdf-162">CSV</span></span>

<span data-ttu-id="02fdf-163">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="02fdf-163">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="02fdf-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="02fdf-164">Request</span></span>

<span data-ttu-id="02fdf-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="02fdf-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitycounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="02fdf-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="02fdf-166">Response</span></span>

<span data-ttu-id="02fdf-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="02fdf-167">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="02fdf-168">Образец кода SDK</span><span class="sxs-lookup"><span data-stu-id="02fdf-168">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="02fdf-169">C#</span><span class="sxs-lookup"><span data-stu-id="02fdf-169">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365groupsactivitycounts_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="02fdf-170">Javascript</span><span class="sxs-lookup"><span data-stu-id="02fdf-170">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365groupsactivitycounts_csv-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="02fdf-171">Цель — C</span><span class="sxs-lookup"><span data-stu-id="02fdf-171">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365groupsactivitycounts_csv-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="02fdf-172">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="02fdf-172">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Exchange Emails Received,Yammer Messages Posted,Yammer Messages Read,Yammer Messages Liked,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="02fdf-173">JSON</span><span class="sxs-lookup"><span data-stu-id="02fdf-173">JSON</span></span>

<span data-ttu-id="02fdf-174">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="02fdf-174">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="02fdf-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="02fdf-175">Request</span></span>

<span data-ttu-id="02fdf-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="02fdf-176">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitycounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="02fdf-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="02fdf-177">Response</span></span>

<span data-ttu-id="02fdf-178">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="02fdf-178">The following is an example of the response.</span></span>

> <span data-ttu-id="02fdf-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="02fdf-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365GroupsActivityCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 310

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365GroupsActivityCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "exchangeEmailsReceived": 0, 
      "yammerMessagesPosted": 0, 
      "yammerMessagesRead": 0, 
      "yammerMessagesLiked": 0, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="02fdf-181">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="02fdf-181">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="02fdf-182">C#</span><span class="sxs-lookup"><span data-stu-id="02fdf-182">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365groupsactivitycounts_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="02fdf-183">Javascript</span><span class="sxs-lookup"><span data-stu-id="02fdf-183">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365groupsactivitycounts_json-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="02fdf-184">Цель — C</span><span class="sxs-lookup"><span data-stu-id="02fdf-184">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365groupsactivitycounts_json-Objective-C-snippets.md)]
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
    "Error: /api-reference/beta/api/reportroot-getoffice365groupsactivitycounts.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getoffice365groupsactivitycounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getoffice365groupsactivitycounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getoffice365groupsactivitycounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getoffice365groupsactivitycounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
