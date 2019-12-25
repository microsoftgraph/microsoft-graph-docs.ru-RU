---
title: 'reportRoot: getOneDriveUsageStorage'
description: Получение сведений о том, как меняется используемый объем хранилища в OneDrive для бизнеса.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 871cbd1a2ccc8ddd02c7ec21e7ec9de896d935ce
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869061"
---
# <a name="reportroot-getonedriveusagestorage"></a><span data-ttu-id="46320-103">reportRoot: getOneDriveUsageStorage</span><span class="sxs-lookup"><span data-stu-id="46320-103">reportRoot: getOneDriveUsageStorage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46320-104">Получение сведений о том, как меняется используемый объем хранилища в OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="46320-104">Get the trend on the amount of storage you are using in OneDrive for Business.</span></span>

> <span data-ttu-id="46320-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: использование OneDrive для бизнеса](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span><span class="sxs-lookup"><span data-stu-id="46320-105">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="46320-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="46320-106">Permissions</span></span>

<span data-ttu-id="46320-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46320-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="46320-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="46320-109">Permission type</span></span>                        | <span data-ttu-id="46320-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="46320-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="46320-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="46320-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="46320-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="46320-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="46320-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="46320-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46320-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46320-114">Not supported.</span></span>                           |
| <span data-ttu-id="46320-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="46320-115">Application</span></span>                            | <span data-ttu-id="46320-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="46320-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="46320-117">**Примечание**. для делегированных разрешений, чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя, администратору клиента необходимо назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="46320-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="46320-118">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="46320-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="46320-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="46320-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageStorage(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="46320-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="46320-120">Function parameters</span></span>

<span data-ttu-id="46320-121">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="46320-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="46320-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="46320-122">Parameter</span></span> | <span data-ttu-id="46320-123">Тип</span><span class="sxs-lookup"><span data-stu-id="46320-123">Type</span></span>   | <span data-ttu-id="46320-124">Описание</span><span class="sxs-lookup"><span data-stu-id="46320-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="46320-125">period</span><span class="sxs-lookup"><span data-stu-id="46320-125">period</span></span>    | <span data-ttu-id="46320-126">string</span><span class="sxs-lookup"><span data-stu-id="46320-126">string</span></span> | <span data-ttu-id="46320-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="46320-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="46320-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="46320-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="46320-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="46320-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="46320-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="46320-130">Required.</span></span> |

<span data-ttu-id="46320-131">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="46320-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="46320-132">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="46320-132">The default output type is text/csv.</span></span> <span data-ttu-id="46320-133">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="46320-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="46320-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="46320-134">Request headers</span></span>

| <span data-ttu-id="46320-135">Имя</span><span class="sxs-lookup"><span data-stu-id="46320-135">Name</span></span>          | <span data-ttu-id="46320-136">Описание</span><span class="sxs-lookup"><span data-stu-id="46320-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="46320-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="46320-137">Authorization</span></span> | <span data-ttu-id="46320-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="46320-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="46320-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="46320-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="46320-141">CSV</span><span class="sxs-lookup"><span data-stu-id="46320-141">CSV</span></span>

<span data-ttu-id="46320-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="46320-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="46320-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="46320-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="46320-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="46320-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="46320-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="46320-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="46320-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="46320-146">Report Refresh Date</span></span>
- <span data-ttu-id="46320-147">"Site Type" (Тип сайта);</span><span class="sxs-lookup"><span data-stu-id="46320-147">Site Type</span></span>
- <span data-ttu-id="46320-148">"Storage Used (Byte)" (Используемый объем хранилища в байтах);</span><span class="sxs-lookup"><span data-stu-id="46320-148">Storage Used (Byte)</span></span>
- <span data-ttu-id="46320-149">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="46320-149">Report Date</span></span>
- <span data-ttu-id="46320-150">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="46320-150">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="46320-151">JSON</span><span class="sxs-lookup"><span data-stu-id="46320-151">JSON</span></span>

<span data-ttu-id="46320-152">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[ситеусажестораже](../resources/siteusagestorage.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="46320-152">If successful, this method returns a `200 OK` response code and a **[siteUsageStorage](../resources/siteusagestorage.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46320-153">Пример</span><span class="sxs-lookup"><span data-stu-id="46320-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="46320-154">CSV</span><span class="sxs-lookup"><span data-stu-id="46320-154">CSV</span></span>

<span data-ttu-id="46320-155">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="46320-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="46320-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="46320-156">Request</span></span>

<span data-ttu-id="46320-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="46320-157">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="46320-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="46320-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusagestorage_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageStorage(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="46320-159">C#</span><span class="sxs-lookup"><span data-stu-id="46320-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveusagestorage-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="46320-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="46320-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveusagestorage-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="46320-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="46320-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveusagestorage-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="46320-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="46320-162">Response</span></span>

<span data-ttu-id="46320-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="46320-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="46320-164">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="46320-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Storage Used (Byte),Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="46320-165">JSON</span><span class="sxs-lookup"><span data-stu-id="46320-165">JSON</span></span>

<span data-ttu-id="46320-166">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="46320-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="46320-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="46320-167">Request</span></span>

<span data-ttu-id="46320-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="46320-168">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="46320-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="46320-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusagestorage_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageStorage(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="46320-170">C#</span><span class="sxs-lookup"><span data-stu-id="46320-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveusagestorage-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="46320-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="46320-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveusagestorage-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="46320-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="46320-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveusagestorage-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="46320-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="46320-173">Response</span></span>

<span data-ttu-id="46320-174">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="46320-174">The following is an example of the response.</span></span>

> <span data-ttu-id="46320-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="46320-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.siteUsageStorage"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 248

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.siteUsageStorage)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteType": "All", 
      "storageUsedInBytes": 132654293197, 
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
