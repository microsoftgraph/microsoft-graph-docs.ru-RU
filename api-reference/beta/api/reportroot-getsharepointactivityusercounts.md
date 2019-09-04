---
title: 'reportRoot: getSharePointActivityUserCounts'
description: Отслеживайте, как меняется количество активных пользователей. Пользователь считается активным, если он выполнил действие с файлом (сохранение, синхронизация, изменение или предоставление общего доступа) или посетил страницу в указанный период.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 05914e235162bdf9eec5ef8c49432717abb2c90f
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36722939"
---
# <a name="reportroot-getsharepointactivityusercounts"></a><span data-ttu-id="4fe71-104">reportRoot: getSharePointActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="4fe71-104">reportRoot: getSharePointActivityUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4fe71-105">Отслеживайте, как меняется количество активных пользователей.</span><span class="sxs-lookup"><span data-stu-id="4fe71-105">Get the trend in the number of active users.</span></span> <span data-ttu-id="4fe71-106">Пользователь считается активным, если он сохранил, синхронизировал, изменил или отправил файл или посетил страницу в указанный период.</span><span class="sxs-lookup"><span data-stu-id="4fe71-106">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span>

> <span data-ttu-id="4fe71-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="4fe71-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="4fe71-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4fe71-108">Permissions</span></span>

<span data-ttu-id="4fe71-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4fe71-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4fe71-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4fe71-111">Permission type</span></span>                        | <span data-ttu-id="4fe71-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4fe71-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="4fe71-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4fe71-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="4fe71-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4fe71-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="4fe71-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4fe71-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4fe71-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4fe71-116">Not supported.</span></span>                           |
| <span data-ttu-id="4fe71-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4fe71-117">Application</span></span>                            | <span data-ttu-id="4fe71-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4fe71-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="4fe71-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4fe71-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="4fe71-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="4fe71-120">Function parameters</span></span>

<span data-ttu-id="4fe71-121">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="4fe71-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="4fe71-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="4fe71-122">Parameter</span></span> | <span data-ttu-id="4fe71-123">Тип</span><span class="sxs-lookup"><span data-stu-id="4fe71-123">Type</span></span>   | <span data-ttu-id="4fe71-124">Описание</span><span class="sxs-lookup"><span data-stu-id="4fe71-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="4fe71-125">period</span><span class="sxs-lookup"><span data-stu-id="4fe71-125">period</span></span>    | <span data-ttu-id="4fe71-126">string</span><span class="sxs-lookup"><span data-stu-id="4fe71-126">string</span></span> | <span data-ttu-id="4fe71-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="4fe71-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="4fe71-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="4fe71-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="4fe71-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="4fe71-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="4fe71-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4fe71-130">Required.</span></span> |

<span data-ttu-id="4fe71-131">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="4fe71-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="4fe71-132">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="4fe71-132">The default output type is text/csv.</span></span> <span data-ttu-id="4fe71-133">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="4fe71-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4fe71-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4fe71-134">Request headers</span></span>

| <span data-ttu-id="4fe71-135">Имя</span><span class="sxs-lookup"><span data-stu-id="4fe71-135">Name</span></span>          | <span data-ttu-id="4fe71-136">Описание</span><span class="sxs-lookup"><span data-stu-id="4fe71-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="4fe71-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4fe71-137">Authorization</span></span> | <span data-ttu-id="4fe71-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4fe71-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="4fe71-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="4fe71-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="4fe71-141">CSV</span><span class="sxs-lookup"><span data-stu-id="4fe71-141">CSV</span></span>

<span data-ttu-id="4fe71-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="4fe71-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="4fe71-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="4fe71-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="4fe71-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="4fe71-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="4fe71-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="4fe71-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="4fe71-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="4fe71-146">Report Refresh Date</span></span>
- <span data-ttu-id="4fe71-147">Visited Page (посетило страницу)</span><span class="sxs-lookup"><span data-stu-id="4fe71-147">Visited Page</span></span>
- <span data-ttu-id="4fe71-148">Viewed Or Edited (просмотрело или изменило)</span><span class="sxs-lookup"><span data-stu-id="4fe71-148">Viewed Or Edited</span></span>
- <span data-ttu-id="4fe71-149">"Synced" (Синхронизированы);</span><span class="sxs-lookup"><span data-stu-id="4fe71-149">Synced</span></span>
- <span data-ttu-id="4fe71-150">"Shared Internally" (К чему предоставлен доступ внутренним пользователям);</span><span class="sxs-lookup"><span data-stu-id="4fe71-150">Shared Internally</span></span>
- <span data-ttu-id="4fe71-151">"Shared Externally" (К чему предоставлен доступ внешним пользователям);</span><span class="sxs-lookup"><span data-stu-id="4fe71-151">Shared Externally</span></span>
- <span data-ttu-id="4fe71-152">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="4fe71-152">Report Date</span></span>
- <span data-ttu-id="4fe71-153">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="4fe71-153">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="4fe71-154">JSON</span><span class="sxs-lookup"><span data-stu-id="4fe71-154">JSON</span></span>

<span data-ttu-id="4fe71-155">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[шарепоинтактивитюсеркаунтс](../resources/sharepointactivityusercounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4fe71-155">If successful, this method returns a `200 OK` response code and a **[sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4fe71-156">Пример</span><span class="sxs-lookup"><span data-stu-id="4fe71-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="4fe71-157">CSV</span><span class="sxs-lookup"><span data-stu-id="4fe71-157">CSV</span></span>

<span data-ttu-id="4fe71-158">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="4fe71-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="4fe71-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="4fe71-159">Request</span></span>

<span data-ttu-id="4fe71-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4fe71-160">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="4fe71-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="4fe71-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4fe71-162">C#</span><span class="sxs-lookup"><span data-stu-id="4fe71-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointactivityusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4fe71-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4fe71-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointactivityusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4fe71-164">Цель — C</span><span class="sxs-lookup"><span data-stu-id="4fe71-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointactivityusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4fe71-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="4fe71-165">Response</span></span>

<span data-ttu-id="4fe71-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4fe71-166">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="4fe71-167">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="4fe71-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Visited Page,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="4fe71-168">JSON</span><span class="sxs-lookup"><span data-stu-id="4fe71-168">JSON</span></span>

<span data-ttu-id="4fe71-169">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="4fe71-169">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="4fe71-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="4fe71-170">Request</span></span>

<span data-ttu-id="4fe71-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4fe71-171">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="4fe71-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="4fe71-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4fe71-173">C#</span><span class="sxs-lookup"><span data-stu-id="4fe71-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointactivityusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4fe71-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4fe71-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointactivityusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4fe71-175">Цель — C</span><span class="sxs-lookup"><span data-stu-id="4fe71-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointactivityusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4fe71-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="4fe71-176">Response</span></span>

<span data-ttu-id="4fe71-177">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4fe71-177">The following is an example of the response.</span></span>

> <span data-ttu-id="4fe71-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4fe71-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointActivityUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 302

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.sharePointActivityUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "visitedPage": 56, 
      "viewedOrEdited": 163, 
      "synced": 7, 
      "sharedInternally": 10, 
      "sharedExternally": 1, 
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
