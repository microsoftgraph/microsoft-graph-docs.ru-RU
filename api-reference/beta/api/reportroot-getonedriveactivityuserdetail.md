---
title: 'reportRoot: getOneDriveActivityUserDetail'
description: Получите сведения о действиях в OneDrive с разбивкой по пользователям.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: ff70b8d4e37f39e11ea4ee2b4cfd7828be15a3a7
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35267335"
---
# <a name="reportroot-getonedriveactivityuserdetail"></a><span data-ttu-id="aeecc-103">reportRoot: getOneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="aeecc-103">reportRoot: getOneDriveActivityUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aeecc-104">Получите сведения о действиях в OneDrive с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="aeecc-104">Get details about OneDrive activity by user.</span></span>

> <span data-ttu-id="aeecc-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия в OneDrive для бизнеса](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span><span class="sxs-lookup"><span data-stu-id="aeecc-105">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="permissions"></a><span data-ttu-id="aeecc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aeecc-106">Permissions</span></span>

<span data-ttu-id="aeecc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aeecc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="aeecc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aeecc-109">Permission type</span></span>                        | <span data-ttu-id="aeecc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aeecc-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="aeecc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aeecc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="aeecc-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="aeecc-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="aeecc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aeecc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aeecc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aeecc-114">Not supported.</span></span>                           |
| <span data-ttu-id="aeecc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aeecc-115">Application</span></span>                            | <span data-ttu-id="aeecc-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="aeecc-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="aeecc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aeecc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveActivityUserDetail(period='{period_value}')
GET /reports/getOneDriveActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="aeecc-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="aeecc-118">Function parameters</span></span>

<span data-ttu-id="aeecc-119">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="aeecc-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="aeecc-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="aeecc-120">Parameter</span></span> | <span data-ttu-id="aeecc-121">Тип</span><span class="sxs-lookup"><span data-stu-id="aeecc-121">Type</span></span>   | <span data-ttu-id="aeecc-122">Описание</span><span class="sxs-lookup"><span data-stu-id="aeecc-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="aeecc-123">period</span><span class="sxs-lookup"><span data-stu-id="aeecc-123">period</span></span>    | <span data-ttu-id="aeecc-124">string</span><span class="sxs-lookup"><span data-stu-id="aeecc-124">string</span></span> | <span data-ttu-id="aeecc-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="aeecc-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="aeecc-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="aeecc-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="aeecc-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="aeecc-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="aeecc-128">date</span><span class="sxs-lookup"><span data-stu-id="aeecc-128">date</span></span>      | <span data-ttu-id="aeecc-129">Date</span><span class="sxs-lookup"><span data-stu-id="aeecc-129">Date</span></span>   | <span data-ttu-id="aeecc-130">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="aeecc-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="aeecc-131">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="aeecc-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="aeecc-132">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="aeecc-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="aeecc-133">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="aeecc-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="aeecc-134">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="aeecc-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="aeecc-135">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="aeecc-135">The default output type is text/csv.</span></span> <span data-ttu-id="aeecc-136">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="aeecc-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aeecc-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aeecc-137">Request headers</span></span>

| <span data-ttu-id="aeecc-138">Имя</span><span class="sxs-lookup"><span data-stu-id="aeecc-138">Name</span></span>          | <span data-ttu-id="aeecc-139">Описание</span><span class="sxs-lookup"><span data-stu-id="aeecc-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="aeecc-140">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aeecc-140">Authorization</span></span> | <span data-ttu-id="aeecc-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aeecc-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="aeecc-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="aeecc-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="aeecc-144">CSV</span><span class="sxs-lookup"><span data-stu-id="aeecc-144">CSV</span></span>

<span data-ttu-id="aeecc-145">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="aeecc-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="aeecc-146">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="aeecc-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="aeecc-147">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="aeecc-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="aeecc-148">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="aeecc-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="aeecc-149">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="aeecc-149">Report Refresh Date</span></span>
- <span data-ttu-id="aeecc-150">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="aeecc-150">User Principal Name</span></span>
- <span data-ttu-id="aeecc-151">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="aeecc-151">Is Deleted</span></span>
- <span data-ttu-id="aeecc-152">"Deleted Date" (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="aeecc-152">Deleted Date</span></span>
- <span data-ttu-id="aeecc-153">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="aeecc-153">Last Activity Date</span></span>
- <span data-ttu-id="aeecc-154">"Viewed Or Edited File Count" (Количество просмотренных или измененных файлов);</span><span class="sxs-lookup"><span data-stu-id="aeecc-154">Viewed Or Edited File Count</span></span>
- <span data-ttu-id="aeecc-155">"Synced File Count" (Количество синхронизированных файлов);</span><span class="sxs-lookup"><span data-stu-id="aeecc-155">Synced File Count</span></span>
- <span data-ttu-id="aeecc-156">"Shared Internally File Count" (Количество файлов, к которым предоставлен доступ внутренним пользователям);</span><span class="sxs-lookup"><span data-stu-id="aeecc-156">Shared Internally File Count</span></span>
- <span data-ttu-id="aeecc-157">"Shared Externally File Count" (Количество файлов, к которым предоставлен доступ внешним пользователям);</span><span class="sxs-lookup"><span data-stu-id="aeecc-157">Shared Externally File Count</span></span>
- <span data-ttu-id="aeecc-158">Assigned Products (назначенные продукты)</span><span class="sxs-lookup"><span data-stu-id="aeecc-158">Assigned Products</span></span>
- <span data-ttu-id="aeecc-159">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="aeecc-159">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="aeecc-160">JSON</span><span class="sxs-lookup"><span data-stu-id="aeecc-160">JSON</span></span>

<span data-ttu-id="aeecc-161">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[онедривеактивитюсердетаил](../resources/onedriveactivityuserdetail.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="aeecc-161">If successful, this method returns a `200 OK` response code and a **[oneDriveActivityUserDetail](../resources/onedriveactivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="aeecc-162">Размер страницы по умолчанию для этого запроса составляет 200 элементов.</span><span class="sxs-lookup"><span data-stu-id="aeecc-162">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="aeecc-163">Пример</span><span class="sxs-lookup"><span data-stu-id="aeecc-163">Example</span></span>

### <a name="csv"></a><span data-ttu-id="aeecc-164">CSV</span><span class="sxs-lookup"><span data-stu-id="aeecc-164">CSV</span></span>

<span data-ttu-id="aeecc-165">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="aeecc-165">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="aeecc-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="aeecc-166">Request</span></span>

<span data-ttu-id="aeecc-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aeecc-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveactivityuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveActivityUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="aeecc-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="aeecc-168">Response</span></span>

<span data-ttu-id="aeecc-169">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="aeecc-169">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="aeecc-170">Образец кода SDK</span><span class="sxs-lookup"><span data-stu-id="aeecc-170">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="aeecc-171">C#</span><span class="sxs-lookup"><span data-stu-id="aeecc-171">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveactivityuserdetail_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="aeecc-172">Javascript</span><span class="sxs-lookup"><span data-stu-id="aeecc-172">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveactivityuserdetail_csv-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="aeecc-173">Цель — C</span><span class="sxs-lookup"><span data-stu-id="aeecc-173">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveactivityuserdetail_csv-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="aeecc-174">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="aeecc-174">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Viewed Or Edited File Count,Synced File Count,Shared Internally File Count,Shared Externally File Count,Assigned Products,Report Period
```

### <a name="json"></a><span data-ttu-id="aeecc-175">JSON</span><span class="sxs-lookup"><span data-stu-id="aeecc-175">JSON</span></span>

<span data-ttu-id="aeecc-176">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="aeecc-176">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="aeecc-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="aeecc-177">Request</span></span>

<span data-ttu-id="aeecc-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aeecc-178">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveactivityuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveActivityUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="aeecc-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="aeecc-179">Response</span></span>

<span data-ttu-id="aeecc-180">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="aeecc-180">The following is an example of the response.</span></span>

> <span data-ttu-id="aeecc-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aeecc-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oneDriveActivityUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 450

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.oneDriveActivityUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "isDeleted": false, 
      "deletedDate": null, 
      "lastActivityDate": "2017-09-01", 
      "viewedOrEditedFileCount": 1, 
      "syncedFileCount": 0, 
      "sharedInternallyFileCount": 0, 
      "sharedExternallyFileCount": 0, 
      "assignedProducts": [
        "OFFICE 365 ENTERPRISE E5"
      ], 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="aeecc-183">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="aeecc-183">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="aeecc-184">C#</span><span class="sxs-lookup"><span data-stu-id="aeecc-184">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveactivityuserdetail_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="aeecc-185">Javascript</span><span class="sxs-lookup"><span data-stu-id="aeecc-185">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveactivityuserdetail_json-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="aeecc-186">Цель — C</span><span class="sxs-lookup"><span data-stu-id="aeecc-186">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveactivityuserdetail_json-Objective-C-snippets.md)]
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
    "Error: /api-reference/beta/api/reportroot-getonedriveactivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getonedriveactivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getonedriveactivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getonedriveactivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getonedriveactivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
