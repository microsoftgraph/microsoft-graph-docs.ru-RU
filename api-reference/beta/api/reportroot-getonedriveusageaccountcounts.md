---
title: 'reportRoot: getOneDriveUsageAccountCounts'
description: Отслеживайте, как меняется количество активных сайтов OneDrive для бизнеса. Активным считается сайт, на котором пользователи просматривали, изменяли, добавляли, скачивали, отправляли или синхронизировали файлы.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 57555639e2b4702d1408b76e0ce7ae35fc3dcb31
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867486"
---
# <a name="reportroot-getonedriveusageaccountcounts"></a><span data-ttu-id="23da6-104">reportRoot: getOneDriveUsageAccountCounts</span><span class="sxs-lookup"><span data-stu-id="23da6-104">reportRoot: getOneDriveUsageAccountCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23da6-105">Отслеживайте, как меняется количество активных сайтов OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="23da6-105">Get the trend in the number of active OneDrive for Business sites.</span></span> <span data-ttu-id="23da6-106">Активным считается сайт, на котором пользователи просматривали, изменяли, добавляли, скачивали, отправляли или синхронизировали файлы.</span><span class="sxs-lookup"><span data-stu-id="23da6-106">Any site on which users viewed, modified, uploaded, downloaded, shared, or synced files is considered an active site.</span></span>

> <span data-ttu-id="23da6-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span><span class="sxs-lookup"><span data-stu-id="23da6-107">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="23da6-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="23da6-108">Permissions</span></span>

<span data-ttu-id="23da6-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23da6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="23da6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="23da6-111">Permission type</span></span>                        | <span data-ttu-id="23da6-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="23da6-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="23da6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="23da6-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="23da6-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="23da6-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="23da6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="23da6-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23da6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23da6-116">Not supported.</span></span>                           |
| <span data-ttu-id="23da6-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="23da6-117">Application</span></span>                            | <span data-ttu-id="23da6-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="23da6-118">Reports.Read.All</span></span>                         |

<span data-ttu-id="23da6-119">**Примечание**. для делегированных разрешений, чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя, администратору клиента необходимо назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="23da6-119">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="23da6-120">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="23da6-120">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="23da6-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="23da6-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageAccountCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="23da6-122">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="23da6-122">Function parameters</span></span>

<span data-ttu-id="23da6-123">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="23da6-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="23da6-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="23da6-124">Parameter</span></span> | <span data-ttu-id="23da6-125">Тип</span><span class="sxs-lookup"><span data-stu-id="23da6-125">Type</span></span>   | <span data-ttu-id="23da6-126">Описание</span><span class="sxs-lookup"><span data-stu-id="23da6-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="23da6-127">period</span><span class="sxs-lookup"><span data-stu-id="23da6-127">period</span></span>    | <span data-ttu-id="23da6-128">string</span><span class="sxs-lookup"><span data-stu-id="23da6-128">string</span></span> | <span data-ttu-id="23da6-129">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="23da6-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="23da6-130">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="23da6-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="23da6-131">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="23da6-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="23da6-132">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="23da6-132">Required.</span></span> |

<span data-ttu-id="23da6-133">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="23da6-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="23da6-134">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="23da6-134">The default output type is text/csv.</span></span> <span data-ttu-id="23da6-135">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="23da6-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="23da6-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="23da6-136">Request headers</span></span>

| <span data-ttu-id="23da6-137">Имя</span><span class="sxs-lookup"><span data-stu-id="23da6-137">Name</span></span>          | <span data-ttu-id="23da6-138">Описание</span><span class="sxs-lookup"><span data-stu-id="23da6-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="23da6-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="23da6-139">Authorization</span></span> | <span data-ttu-id="23da6-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="23da6-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="23da6-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="23da6-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="23da6-143">CSV</span><span class="sxs-lookup"><span data-stu-id="23da6-143">CSV</span></span>

<span data-ttu-id="23da6-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="23da6-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="23da6-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="23da6-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="23da6-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="23da6-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="23da6-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="23da6-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="23da6-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="23da6-148">Report Refresh Date</span></span>
- <span data-ttu-id="23da6-149">"Site Type" (Тип сайта);</span><span class="sxs-lookup"><span data-stu-id="23da6-149">Site Type</span></span>
- <span data-ttu-id="23da6-150">"Total" (Всего);</span><span class="sxs-lookup"><span data-stu-id="23da6-150">Total</span></span>
- <span data-ttu-id="23da6-151">Active (активные)</span><span class="sxs-lookup"><span data-stu-id="23da6-151">Active</span></span>
- <span data-ttu-id="23da6-152">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="23da6-152">Report Date</span></span>
- <span data-ttu-id="23da6-153">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="23da6-153">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="23da6-154">JSON</span><span class="sxs-lookup"><span data-stu-id="23da6-154">JSON</span></span>

<span data-ttu-id="23da6-155">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[онедривеусажеаккаунткаунтс](../resources/onedriveusageaccountcounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="23da6-155">If successful, this method returns a `200 OK` response code and a **[oneDriveUsageAccountCounts](../resources/onedriveusageaccountcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23da6-156">Пример</span><span class="sxs-lookup"><span data-stu-id="23da6-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="23da6-157">CSV</span><span class="sxs-lookup"><span data-stu-id="23da6-157">CSV</span></span>

<span data-ttu-id="23da6-158">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="23da6-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="23da6-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="23da6-159">Request</span></span>

<span data-ttu-id="23da6-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23da6-160">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="23da6-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="23da6-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountcounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="23da6-162">C#</span><span class="sxs-lookup"><span data-stu-id="23da6-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveusageaccountcounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="23da6-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="23da6-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveusageaccountcounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="23da6-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="23da6-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveusageaccountcounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="23da6-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="23da6-165">Response</span></span>

<span data-ttu-id="23da6-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="23da6-166">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="23da6-167">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="23da6-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="23da6-168">JSON</span><span class="sxs-lookup"><span data-stu-id="23da6-168">JSON</span></span>

<span data-ttu-id="23da6-169">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="23da6-169">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="23da6-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="23da6-170">Request</span></span>

<span data-ttu-id="23da6-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23da6-171">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="23da6-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="23da6-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountcounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="23da6-173">C#</span><span class="sxs-lookup"><span data-stu-id="23da6-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveusageaccountcounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="23da6-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="23da6-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveusageaccountcounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="23da6-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="23da6-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveusageaccountcounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="23da6-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="23da6-176">Response</span></span>

<span data-ttu-id="23da6-177">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="23da6-177">The following is an example of the response.</span></span>

> <span data-ttu-id="23da6-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="23da6-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oneDriveUsageAccountCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 249

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.oneDriveUsageAccountCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteType": "All", 
      "total": 207, 
      "active": 89, 
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
