---
title: 'reportRoot: getOneDriveActivityFileCounts'
description: Получение количества уникальных пользователей с лицензией, которые работали с файлами в любой учетной записи OneDrive.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: e5a7a40e8b1dbbae0031286a89712e7a6729da12
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35267328"
---
# <a name="reportroot-getonedriveactivityfilecounts"></a><span data-ttu-id="cd9c9-103">reportRoot: getOneDriveActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="cd9c9-103">reportRoot: getOneDriveActivityFileCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd9c9-104">Получение количества уникальных пользователей с лицензией, которые работали с файлами в любой учетной записи OneDrive.</span><span class="sxs-lookup"><span data-stu-id="cd9c9-104">Get the number of unique, licensed users that performed file interactions against any OneDrive account.</span></span>

> <span data-ttu-id="cd9c9-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия в OneDrive для бизнеса](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span><span class="sxs-lookup"><span data-stu-id="cd9c9-105">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="permissions"></a><span data-ttu-id="cd9c9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cd9c9-106">Permissions</span></span>

<span data-ttu-id="cd9c9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd9c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cd9c9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cd9c9-109">Permission type</span></span>                        | <span data-ttu-id="cd9c9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cd9c9-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="cd9c9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cd9c9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cd9c9-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="cd9c9-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="cd9c9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cd9c9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd9c9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd9c9-114">Not supported.</span></span>                           |
| <span data-ttu-id="cd9c9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cd9c9-115">Application</span></span>                            | <span data-ttu-id="cd9c9-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="cd9c9-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="cd9c9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cd9c9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveActivityFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="cd9c9-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="cd9c9-118">Function parameters</span></span>

<span data-ttu-id="cd9c9-119">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="cd9c9-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="cd9c9-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="cd9c9-120">Parameter</span></span> | <span data-ttu-id="cd9c9-121">Тип</span><span class="sxs-lookup"><span data-stu-id="cd9c9-121">Type</span></span>   | <span data-ttu-id="cd9c9-122">Описание</span><span class="sxs-lookup"><span data-stu-id="cd9c9-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="cd9c9-123">period</span><span class="sxs-lookup"><span data-stu-id="cd9c9-123">period</span></span>    | <span data-ttu-id="cd9c9-124">string</span><span class="sxs-lookup"><span data-stu-id="cd9c9-124">string</span></span> | <span data-ttu-id="cd9c9-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="cd9c9-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="cd9c9-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="cd9c9-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="cd9c9-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="cd9c9-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="cd9c9-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cd9c9-128">Required.</span></span> |

<span data-ttu-id="cd9c9-129">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="cd9c9-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="cd9c9-130">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="cd9c9-130">The default output type is text/csv.</span></span> <span data-ttu-id="cd9c9-131">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="cd9c9-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cd9c9-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cd9c9-132">Request headers</span></span>

| <span data-ttu-id="cd9c9-133">Имя</span><span class="sxs-lookup"><span data-stu-id="cd9c9-133">Name</span></span>          | <span data-ttu-id="cd9c9-134">Описание</span><span class="sxs-lookup"><span data-stu-id="cd9c9-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="cd9c9-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cd9c9-135">Authorization</span></span> | <span data-ttu-id="cd9c9-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cd9c9-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="cd9c9-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="cd9c9-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="cd9c9-139">CSV</span><span class="sxs-lookup"><span data-stu-id="cd9c9-139">CSV</span></span>

<span data-ttu-id="cd9c9-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="cd9c9-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="cd9c9-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="cd9c9-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="cd9c9-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="cd9c9-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="cd9c9-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="cd9c9-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="cd9c9-144">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="cd9c9-144">Report Refresh Date</span></span>
- <span data-ttu-id="cd9c9-145">"Viewed Or Edited" (Просмотрены или изменены);</span><span class="sxs-lookup"><span data-stu-id="cd9c9-145">Viewed Or Edited</span></span>
- <span data-ttu-id="cd9c9-146">"Synced" (Синхронизированы);</span><span class="sxs-lookup"><span data-stu-id="cd9c9-146">Synced</span></span>
- <span data-ttu-id="cd9c9-147">"Shared Internally" (К чему предоставлен доступ внутренним пользователям);</span><span class="sxs-lookup"><span data-stu-id="cd9c9-147">Shared Internally</span></span>
- <span data-ttu-id="cd9c9-148">"Shared Externally" (К чему предоставлен доступ внешним пользователям);</span><span class="sxs-lookup"><span data-stu-id="cd9c9-148">Shared Externally</span></span>
- <span data-ttu-id="cd9c9-149">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="cd9c9-149">Report Date</span></span>
- <span data-ttu-id="cd9c9-150">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="cd9c9-150">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="cd9c9-151">JSON</span><span class="sxs-lookup"><span data-stu-id="cd9c9-151">JSON</span></span>

<span data-ttu-id="cd9c9-152">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[ситеактивитисуммари](../resources/siteactivitysummary.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cd9c9-152">If successful, this method returns a `200 OK` response code and a **[siteActivitySummary](../resources/siteactivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd9c9-153">Пример</span><span class="sxs-lookup"><span data-stu-id="cd9c9-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="cd9c9-154">CSV</span><span class="sxs-lookup"><span data-stu-id="cd9c9-154">CSV</span></span>

<span data-ttu-id="cd9c9-155">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="cd9c9-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="cd9c9-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="cd9c9-156">Request</span></span>

<span data-ttu-id="cd9c9-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cd9c9-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveactivityfilecounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveActivityFileCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="cd9c9-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="cd9c9-158">Response</span></span>

<span data-ttu-id="cd9c9-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cd9c9-159">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="cd9c9-160">Образец кода SDK</span><span class="sxs-lookup"><span data-stu-id="cd9c9-160">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="cd9c9-161">C#</span><span class="sxs-lookup"><span data-stu-id="cd9c9-161">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveactivityfilecounts_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cd9c9-162">Javascript</span><span class="sxs-lookup"><span data-stu-id="cd9c9-162">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveactivityfilecounts_csv-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="cd9c9-163">Цель — C</span><span class="sxs-lookup"><span data-stu-id="cd9c9-163">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveactivityfilecounts_csv-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="cd9c9-164">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="cd9c9-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="cd9c9-165">JSON</span><span class="sxs-lookup"><span data-stu-id="cd9c9-165">JSON</span></span>

<span data-ttu-id="cd9c9-166">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="cd9c9-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="cd9c9-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="cd9c9-167">Request</span></span>

<span data-ttu-id="cd9c9-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cd9c9-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveactivityfilecounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveActivityFileCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="cd9c9-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="cd9c9-169">Response</span></span>

<span data-ttu-id="cd9c9-170">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="cd9c9-170">The following is an example of the response.</span></span>

> <span data-ttu-id="cd9c9-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cd9c9-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.siteActivitySummary"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 280

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.siteActivitySummary)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "viewedOrEdited": 1997, 
      "synced": 24756, 
      "sharedInternally": 7, 
      "sharedExternally": 0, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="cd9c9-173">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="cd9c9-173">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="cd9c9-174">C#</span><span class="sxs-lookup"><span data-stu-id="cd9c9-174">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveactivityfilecounts_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cd9c9-175">Javascript</span><span class="sxs-lookup"><span data-stu-id="cd9c9-175">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveactivityfilecounts_json-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="cd9c9-176">Цель — C</span><span class="sxs-lookup"><span data-stu-id="cd9c9-176">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveactivityfilecounts_json-Objective-C-snippets.md)]
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
    "Error: /api-reference/beta/api/reportroot-getonedriveactivityfilecounts.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getonedriveactivityfilecounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getonedriveactivityfilecounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getonedriveactivityfilecounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getonedriveactivityfilecounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
