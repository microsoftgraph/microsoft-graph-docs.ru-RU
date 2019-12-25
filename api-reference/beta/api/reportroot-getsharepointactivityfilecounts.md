---
title: 'reportRoot: getSharePointActivityFileCounts'
description: Узнайте, сколько уникальных пользователей с лицензиями работали с хранящимися на сайтах SharePoint файлами.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 8cb2ac9a8c6eb84bf7ad59b0a34b79ab90039bfa
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867465"
---
# <a name="reportroot-getsharepointactivityfilecounts"></a><span data-ttu-id="e3855-103">reportRoot: getSharePointActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="e3855-103">reportRoot: getSharePointActivityFileCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3855-104">Узнайте, сколько уникальных пользователей с лицензиями работали с хранящимися на сайтах SharePoint файлами.</span><span class="sxs-lookup"><span data-stu-id="e3855-104">Get the number of unique, licensed users who interacted with files stored on SharePoint sites.</span></span>

> <span data-ttu-id="e3855-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="e3855-105">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="e3855-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e3855-106">Permissions</span></span>

<span data-ttu-id="e3855-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3855-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e3855-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e3855-109">Permission type</span></span>                        | <span data-ttu-id="e3855-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e3855-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e3855-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e3855-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e3855-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3855-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e3855-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e3855-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3855-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3855-114">Not supported.</span></span>                           |
| <span data-ttu-id="e3855-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e3855-115">Application</span></span>                            | <span data-ttu-id="e3855-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3855-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="e3855-117">**Примечание**. для делегированных разрешений, чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя, администратору клиента необходимо назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e3855-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="e3855-118">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="e3855-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="e3855-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e3855-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="e3855-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="e3855-120">Function parameters</span></span>

<span data-ttu-id="e3855-121">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="e3855-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="e3855-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="e3855-122">Parameter</span></span> | <span data-ttu-id="e3855-123">Тип</span><span class="sxs-lookup"><span data-stu-id="e3855-123">Type</span></span>   | <span data-ttu-id="e3855-124">Описание</span><span class="sxs-lookup"><span data-stu-id="e3855-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="e3855-125">period</span><span class="sxs-lookup"><span data-stu-id="e3855-125">period</span></span>    | <span data-ttu-id="e3855-126">string</span><span class="sxs-lookup"><span data-stu-id="e3855-126">string</span></span> | <span data-ttu-id="e3855-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="e3855-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="e3855-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="e3855-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="e3855-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="e3855-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="e3855-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e3855-130">Required.</span></span> |

<span data-ttu-id="e3855-131">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="e3855-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="e3855-132">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="e3855-132">The default output type is text/csv.</span></span> <span data-ttu-id="e3855-133">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="e3855-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e3855-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e3855-134">Request headers</span></span>

| <span data-ttu-id="e3855-135">Имя</span><span class="sxs-lookup"><span data-stu-id="e3855-135">Name</span></span>          | <span data-ttu-id="e3855-136">Описание</span><span class="sxs-lookup"><span data-stu-id="e3855-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="e3855-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e3855-137">Authorization</span></span> | <span data-ttu-id="e3855-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e3855-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="e3855-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3855-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="e3855-141">CSV</span><span class="sxs-lookup"><span data-stu-id="e3855-141">CSV</span></span>

<span data-ttu-id="e3855-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="e3855-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e3855-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="e3855-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e3855-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="e3855-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e3855-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="e3855-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="e3855-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="e3855-146">Report Refresh Date</span></span>
- <span data-ttu-id="e3855-147">"Viewed Or Edited" (Просмотрены или изменены);</span><span class="sxs-lookup"><span data-stu-id="e3855-147">Viewed Or Edited</span></span>
- <span data-ttu-id="e3855-148">"Synced" (Синхронизированы);</span><span class="sxs-lookup"><span data-stu-id="e3855-148">Synced</span></span>
- <span data-ttu-id="e3855-149">"Shared Internally" (К чему предоставлен доступ внутренним пользователям);</span><span class="sxs-lookup"><span data-stu-id="e3855-149">Shared Internally</span></span>
- <span data-ttu-id="e3855-150">"Shared Externally" (К чему предоставлен доступ внешним пользователям);</span><span class="sxs-lookup"><span data-stu-id="e3855-150">Shared Externally</span></span>
- <span data-ttu-id="e3855-151">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="e3855-151">Report Date</span></span>
- <span data-ttu-id="e3855-152">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="e3855-152">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="e3855-153">JSON</span><span class="sxs-lookup"><span data-stu-id="e3855-153">JSON</span></span>

<span data-ttu-id="e3855-154">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[ситеактивитисуммари](../resources/siteactivitysummary.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e3855-154">If successful, this method returns a `200 OK` response code and a **[siteActivitySummary](../resources/siteactivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3855-155">Пример</span><span class="sxs-lookup"><span data-stu-id="e3855-155">Example</span></span>

### <a name="csv"></a><span data-ttu-id="e3855-156">CSV</span><span class="sxs-lookup"><span data-stu-id="e3855-156">CSV</span></span>

<span data-ttu-id="e3855-157">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="e3855-157">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="e3855-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="e3855-158">Request</span></span>

<span data-ttu-id="e3855-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e3855-159">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e3855-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="e3855-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityfilecounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSharePointActivityFileCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e3855-161">C#</span><span class="sxs-lookup"><span data-stu-id="e3855-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointactivityfilecounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e3855-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e3855-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointactivityfilecounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e3855-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e3855-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointactivityfilecounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e3855-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3855-164">Response</span></span>

<span data-ttu-id="e3855-165">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e3855-165">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="e3855-166">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="e3855-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="e3855-167">JSON</span><span class="sxs-lookup"><span data-stu-id="e3855-167">JSON</span></span>

<span data-ttu-id="e3855-168">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="e3855-168">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="e3855-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="e3855-169">Request</span></span>

<span data-ttu-id="e3855-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e3855-170">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e3855-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="e3855-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e3855-172">C#</span><span class="sxs-lookup"><span data-stu-id="e3855-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activeusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e3855-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e3855-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activeusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e3855-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e3855-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activeusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e3855-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3855-175">Response</span></span>

<span data-ttu-id="e3855-176">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e3855-176">The following is an example of the response.</span></span>

> <span data-ttu-id="e3855-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e3855-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.siteActivitySummary"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 278

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.siteActivitySummary)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "viewedOrEdited": 2141, 
      "synced": 614, 
      "sharedInternally": 9, 
      "sharedExternally": 0, 
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
