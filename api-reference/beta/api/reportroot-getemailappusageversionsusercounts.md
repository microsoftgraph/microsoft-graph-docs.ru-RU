---
title: 'reportRoot: getEmailAppUsageVersionsUserCounts'
description: Узнайте, сколько уникальных пользователей у каждой версии Outlook для компьютера.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: c322df30fac9e528a9dff212886013c6c0da0ddd
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35456528"
---
# <a name="reportroot-getemailappusageversionsusercounts"></a><span data-ttu-id="2b11f-103">reportRoot: getEmailAppUsageVersionsUserCounts</span><span class="sxs-lookup"><span data-stu-id="2b11f-103">reportRoot: getEmailAppUsageVersionsUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b11f-104">Узнайте, сколько уникальных пользователей у каждой версии Outlook для компьютера.</span><span class="sxs-lookup"><span data-stu-id="2b11f-104">Get the count of unique users by Outlook desktop version.</span></span>

> <span data-ttu-id="2b11f-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span><span class="sxs-lookup"><span data-stu-id="2b11f-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="2b11f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2b11f-106">Permissions</span></span>

<span data-ttu-id="2b11f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b11f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2b11f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2b11f-109">Permission type</span></span>                        | <span data-ttu-id="2b11f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2b11f-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="2b11f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b11f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2b11f-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b11f-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="2b11f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b11f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b11f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b11f-114">Not supported.</span></span>                           |
| <span data-ttu-id="2b11f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2b11f-115">Application</span></span>                            | <span data-ttu-id="2b11f-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b11f-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="2b11f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b11f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageVersionsUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="2b11f-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="2b11f-118">Function parameters</span></span>

<span data-ttu-id="2b11f-119">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="2b11f-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="2b11f-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="2b11f-120">Parameter</span></span> | <span data-ttu-id="2b11f-121">Тип</span><span class="sxs-lookup"><span data-stu-id="2b11f-121">Type</span></span>   | <span data-ttu-id="2b11f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="2b11f-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="2b11f-123">period</span><span class="sxs-lookup"><span data-stu-id="2b11f-123">period</span></span>    | <span data-ttu-id="2b11f-124">string</span><span class="sxs-lookup"><span data-stu-id="2b11f-124">string</span></span> | <span data-ttu-id="2b11f-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="2b11f-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="2b11f-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="2b11f-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="2b11f-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="2b11f-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="2b11f-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2b11f-128">Required.</span></span> |

<span data-ttu-id="2b11f-129">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="2b11f-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="2b11f-130">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="2b11f-130">The default output type is text/csv.</span></span> <span data-ttu-id="2b11f-131">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="2b11f-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2b11f-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2b11f-132">Request headers</span></span>

| <span data-ttu-id="2b11f-133">Имя</span><span class="sxs-lookup"><span data-stu-id="2b11f-133">Name</span></span>          | <span data-ttu-id="2b11f-134">Описание</span><span class="sxs-lookup"><span data-stu-id="2b11f-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="2b11f-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2b11f-135">Authorization</span></span> | <span data-ttu-id="2b11f-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2b11f-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="2b11f-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b11f-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="2b11f-139">CSV</span><span class="sxs-lookup"><span data-stu-id="2b11f-139">CSV</span></span>

<span data-ttu-id="2b11f-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="2b11f-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="2b11f-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="2b11f-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="2b11f-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="2b11f-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="2b11f-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="2b11f-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="2b11f-144">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="2b11f-144">Report Refresh Date</span></span>
- <span data-ttu-id="2b11f-145">Outlook 2016</span><span class="sxs-lookup"><span data-stu-id="2b11f-145">Outlook 2016</span></span>
- <span data-ttu-id="2b11f-146">Outlook 2013</span><span class="sxs-lookup"><span data-stu-id="2b11f-146">Outlook 2013</span></span>
- <span data-ttu-id="2b11f-147">Outlook 2010</span><span class="sxs-lookup"><span data-stu-id="2b11f-147">Outlook 2010</span></span>
- <span data-ttu-id="2b11f-148">Outlook 2007</span><span class="sxs-lookup"><span data-stu-id="2b11f-148">Outlook 2007</span></span>
- <span data-ttu-id="2b11f-149">Undetermined (не определено)</span><span class="sxs-lookup"><span data-stu-id="2b11f-149">Undetermined</span></span>
- <span data-ttu-id="2b11f-150">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="2b11f-150">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="2b11f-151">JSON</span><span class="sxs-lookup"><span data-stu-id="2b11f-151">JSON</span></span>

<span data-ttu-id="2b11f-152">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[емаилаппусажеверсионсусеркаунтс](../resources/emailappusageversionsusercounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2b11f-152">If successful, this method returns a `200 OK` response code and an **[emailAppUsageVersionsUserCounts](../resources/emailappusageversionsusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b11f-153">Пример</span><span class="sxs-lookup"><span data-stu-id="2b11f-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="2b11f-154">CSV</span><span class="sxs-lookup"><span data-stu-id="2b11f-154">CSV</span></span>

<span data-ttu-id="2b11f-155">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="2b11f-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="2b11f-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b11f-156">Request</span></span>

<span data-ttu-id="2b11f-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b11f-157">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="2b11f-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="2b11f-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageversionsusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageVersionsUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2b11f-159">C#</span><span class="sxs-lookup"><span data-stu-id="2b11f-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailappusageversionsusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2b11f-160">Javascript</span><span class="sxs-lookup"><span data-stu-id="2b11f-160">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailappusageversionsusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2b11f-161">Цель — C</span><span class="sxs-lookup"><span data-stu-id="2b11f-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailappusageversionsusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2b11f-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b11f-162">Response</span></span>

<span data-ttu-id="2b11f-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2b11f-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="2b11f-164">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="2b11f-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Outlook 2016,Outlook 2013,Outlook 2010,Outlook 2007,Undetermined,Report Period
```

### <a name="json"></a><span data-ttu-id="2b11f-165">JSON</span><span class="sxs-lookup"><span data-stu-id="2b11f-165">JSON</span></span>

<span data-ttu-id="2b11f-166">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="2b11f-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="2b11f-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b11f-167">Request</span></span>

<span data-ttu-id="2b11f-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b11f-168">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="2b11f-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="2b11f-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageversionsusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageVersionsUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2b11f-170">C#</span><span class="sxs-lookup"><span data-stu-id="2b11f-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailappusageversionsusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2b11f-171">Javascript</span><span class="sxs-lookup"><span data-stu-id="2b11f-171">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailappusageversionsusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2b11f-172">Цель — C</span><span class="sxs-lookup"><span data-stu-id="2b11f-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailappusageversionsusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2b11f-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b11f-173">Response</span></span>

<span data-ttu-id="2b11f-174">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2b11f-174">The following is an example of the response.</span></span>

> <span data-ttu-id="2b11f-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2b11f-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAppUsageVersionsUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 275

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailAppUsageVersionsUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "outlook2016": 1554, 
      "outlook2013": 64, 
      "outlook2010": 1, 
      "outlook2007": 0, 
      "undetermined": 1259, 
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
