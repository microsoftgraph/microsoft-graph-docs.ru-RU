---
title: 'reportRoot: getOneDriveUsageFileCounts'
description: Получение общего количества файлов на всех сайтах и количества активных файлов. Файл считается активным, если он был сохранен, синхронизирован, изменен в указанный период или им поделились в указанный период.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 990a33b4d8a02132241cb2047426d7ecc8ca5687
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867483"
---
# <a name="reportroot-getonedriveusagefilecounts"></a><span data-ttu-id="79a7a-104">reportRoot: getOneDriveUsageFileCounts</span><span class="sxs-lookup"><span data-stu-id="79a7a-104">reportRoot: getOneDriveUsageFileCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79a7a-105">Получение общего количества файлов на всех сайтах и количества активных файлов.</span><span class="sxs-lookup"><span data-stu-id="79a7a-105">Get the total number of files across all sites and how many are active files.</span></span> <span data-ttu-id="79a7a-106">Файл считается активным, если он был сохранен, синхронизирован, изменен в указанный период или им поделились в указанный период.</span><span class="sxs-lookup"><span data-stu-id="79a7a-106">A file is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span>

> <span data-ttu-id="79a7a-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: использование OneDrive для бизнеса](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span><span class="sxs-lookup"><span data-stu-id="79a7a-107">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="79a7a-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="79a7a-108">Permissions</span></span>

<span data-ttu-id="79a7a-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79a7a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="79a7a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="79a7a-111">Permission type</span></span>                        | <span data-ttu-id="79a7a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="79a7a-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="79a7a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79a7a-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="79a7a-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="79a7a-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="79a7a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="79a7a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79a7a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79a7a-116">Not supported.</span></span>                           |
| <span data-ttu-id="79a7a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="79a7a-117">Application</span></span>                            | <span data-ttu-id="79a7a-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="79a7a-118">Reports.Read.All</span></span>                         |

<span data-ttu-id="79a7a-119">**Примечание**. для делегированных разрешений, чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя, администратору клиента необходимо назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="79a7a-119">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="79a7a-120">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="79a7a-120">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="79a7a-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="79a7a-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="79a7a-122">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="79a7a-122">Function parameters</span></span>

<span data-ttu-id="79a7a-123">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="79a7a-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="79a7a-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="79a7a-124">Parameter</span></span> | <span data-ttu-id="79a7a-125">Тип</span><span class="sxs-lookup"><span data-stu-id="79a7a-125">Type</span></span>   | <span data-ttu-id="79a7a-126">Описание</span><span class="sxs-lookup"><span data-stu-id="79a7a-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="79a7a-127">period</span><span class="sxs-lookup"><span data-stu-id="79a7a-127">period</span></span>    | <span data-ttu-id="79a7a-128">string</span><span class="sxs-lookup"><span data-stu-id="79a7a-128">string</span></span> | <span data-ttu-id="79a7a-129">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="79a7a-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="79a7a-130">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="79a7a-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="79a7a-131">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="79a7a-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="79a7a-132">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79a7a-132">Required.</span></span> |

<span data-ttu-id="79a7a-133">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="79a7a-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="79a7a-134">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="79a7a-134">The default output type is text/csv.</span></span> <span data-ttu-id="79a7a-135">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="79a7a-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="79a7a-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="79a7a-136">Request headers</span></span>

| <span data-ttu-id="79a7a-137">Имя</span><span class="sxs-lookup"><span data-stu-id="79a7a-137">Name</span></span>          | <span data-ttu-id="79a7a-138">Описание</span><span class="sxs-lookup"><span data-stu-id="79a7a-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="79a7a-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="79a7a-139">Authorization</span></span> | <span data-ttu-id="79a7a-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79a7a-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="79a7a-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="79a7a-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="79a7a-143">CSV</span><span class="sxs-lookup"><span data-stu-id="79a7a-143">CSV</span></span>

<span data-ttu-id="79a7a-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="79a7a-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="79a7a-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="79a7a-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="79a7a-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="79a7a-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="79a7a-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="79a7a-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="79a7a-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="79a7a-148">Report Refresh Date</span></span>
- <span data-ttu-id="79a7a-149">"Site Type" (Тип сайта);</span><span class="sxs-lookup"><span data-stu-id="79a7a-149">Site Type</span></span>
- <span data-ttu-id="79a7a-150">"Total" (Всего);</span><span class="sxs-lookup"><span data-stu-id="79a7a-150">Total</span></span>
- <span data-ttu-id="79a7a-151">Active (активные)</span><span class="sxs-lookup"><span data-stu-id="79a7a-151">Active</span></span>
- <span data-ttu-id="79a7a-152">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="79a7a-152">Report Date</span></span>
- <span data-ttu-id="79a7a-153">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="79a7a-153">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="79a7a-154">JSON</span><span class="sxs-lookup"><span data-stu-id="79a7a-154">JSON</span></span>

<span data-ttu-id="79a7a-155">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[онедривеусажефилекаунтс](../resources/onedriveusagefilecounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="79a7a-155">If successful, this method returns a `200 OK` response code and a **[oneDriveUsageFileCounts](../resources/onedriveusagefilecounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79a7a-156">Пример</span><span class="sxs-lookup"><span data-stu-id="79a7a-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="79a7a-157">CSV</span><span class="sxs-lookup"><span data-stu-id="79a7a-157">CSV</span></span>

<span data-ttu-id="79a7a-158">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="79a7a-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="79a7a-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="79a7a-159">Request</span></span>

<span data-ttu-id="79a7a-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="79a7a-160">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="79a7a-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="79a7a-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusagefilecounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageFileCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="79a7a-162">C#</span><span class="sxs-lookup"><span data-stu-id="79a7a-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveusagefilecounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="79a7a-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="79a7a-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveusagefilecounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="79a7a-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="79a7a-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveusagefilecounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="79a7a-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="79a7a-165">Response</span></span>

<span data-ttu-id="79a7a-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="79a7a-166">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="79a7a-167">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="79a7a-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="79a7a-168">JSON</span><span class="sxs-lookup"><span data-stu-id="79a7a-168">JSON</span></span>

<span data-ttu-id="79a7a-169">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="79a7a-169">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="79a7a-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="79a7a-170">Request</span></span>

<span data-ttu-id="79a7a-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="79a7a-171">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="79a7a-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="79a7a-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusagefilecounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageFileCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="79a7a-173">C#</span><span class="sxs-lookup"><span data-stu-id="79a7a-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveusagefilecounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="79a7a-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="79a7a-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveusagefilecounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="79a7a-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="79a7a-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveusagefilecounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="79a7a-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="79a7a-176">Response</span></span>

<span data-ttu-id="79a7a-177">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="79a7a-177">The following is an example of the response.</span></span>

> <span data-ttu-id="79a7a-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="79a7a-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oneDriveUsageFileCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 251

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.oneDriveUsageFileCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteType": "All", 
      "total": 297960, 
      "active": 4679, 
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
