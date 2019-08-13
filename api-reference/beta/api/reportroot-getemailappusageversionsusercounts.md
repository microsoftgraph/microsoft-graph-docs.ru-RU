---
title: 'reportRoot: getEmailAppUsageVersionsUserCounts'
description: Узнайте, сколько уникальных пользователей у каждой версии Outlook для компьютера.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 2e1661ad5c4fabc3165436ee3ab96835322b40d4
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36360698"
---
# <a name="reportroot-getemailappusageversionsusercounts"></a><span data-ttu-id="a7659-103">reportRoot: getEmailAppUsageVersionsUserCounts</span><span class="sxs-lookup"><span data-stu-id="a7659-103">reportRoot: getEmailAppUsageVersionsUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7659-104">Узнайте, сколько уникальных пользователей у каждой версии Outlook для компьютера.</span><span class="sxs-lookup"><span data-stu-id="a7659-104">Get the count of unique users by Outlook desktop version.</span></span>

> <span data-ttu-id="a7659-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span><span class="sxs-lookup"><span data-stu-id="a7659-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="a7659-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a7659-106">Permissions</span></span>

<span data-ttu-id="a7659-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7659-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a7659-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a7659-109">Permission type</span></span>                        | <span data-ttu-id="a7659-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a7659-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="a7659-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a7659-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a7659-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a7659-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="a7659-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a7659-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7659-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7659-114">Not supported.</span></span>                           |
| <span data-ttu-id="a7659-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a7659-115">Application</span></span>                            | <span data-ttu-id="a7659-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a7659-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="a7659-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a7659-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageVersionsUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="a7659-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="a7659-118">Function parameters</span></span>

<span data-ttu-id="a7659-119">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="a7659-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="a7659-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="a7659-120">Parameter</span></span> | <span data-ttu-id="a7659-121">Тип</span><span class="sxs-lookup"><span data-stu-id="a7659-121">Type</span></span>   | <span data-ttu-id="a7659-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a7659-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="a7659-123">period</span><span class="sxs-lookup"><span data-stu-id="a7659-123">period</span></span>    | <span data-ttu-id="a7659-124">string</span><span class="sxs-lookup"><span data-stu-id="a7659-124">string</span></span> | <span data-ttu-id="a7659-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="a7659-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="a7659-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="a7659-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="a7659-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="a7659-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="a7659-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a7659-128">Required.</span></span> |

<span data-ttu-id="a7659-129">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="a7659-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="a7659-130">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="a7659-130">The default output type is text/csv.</span></span> <span data-ttu-id="a7659-131">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="a7659-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a7659-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a7659-132">Request headers</span></span>

| <span data-ttu-id="a7659-133">Имя</span><span class="sxs-lookup"><span data-stu-id="a7659-133">Name</span></span>          | <span data-ttu-id="a7659-134">Описание</span><span class="sxs-lookup"><span data-stu-id="a7659-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="a7659-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a7659-135">Authorization</span></span> | <span data-ttu-id="a7659-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a7659-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="a7659-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7659-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="a7659-139">CSV</span><span class="sxs-lookup"><span data-stu-id="a7659-139">CSV</span></span>

<span data-ttu-id="a7659-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="a7659-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="a7659-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="a7659-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="a7659-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="a7659-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="a7659-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="a7659-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="a7659-144">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="a7659-144">Report Refresh Date</span></span>
- <span data-ttu-id="a7659-145">Outlook 2016</span><span class="sxs-lookup"><span data-stu-id="a7659-145">Outlook 2016</span></span>
- <span data-ttu-id="a7659-146">Outlook 2013</span><span class="sxs-lookup"><span data-stu-id="a7659-146">Outlook 2013</span></span>
- <span data-ttu-id="a7659-147">Outlook 2010</span><span class="sxs-lookup"><span data-stu-id="a7659-147">Outlook 2010</span></span>
- <span data-ttu-id="a7659-148">Outlook 2007</span><span class="sxs-lookup"><span data-stu-id="a7659-148">Outlook 2007</span></span>
- <span data-ttu-id="a7659-149">Undetermined (не определено)</span><span class="sxs-lookup"><span data-stu-id="a7659-149">Undetermined</span></span>
- <span data-ttu-id="a7659-150">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="a7659-150">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="a7659-151">JSON</span><span class="sxs-lookup"><span data-stu-id="a7659-151">JSON</span></span>

<span data-ttu-id="a7659-152">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[емаилаппусажеверсионсусеркаунтс](../resources/emailappusageversionsusercounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a7659-152">If successful, this method returns a `200 OK` response code and an **[emailAppUsageVersionsUserCounts](../resources/emailappusageversionsusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7659-153">Пример</span><span class="sxs-lookup"><span data-stu-id="a7659-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="a7659-154">CSV</span><span class="sxs-lookup"><span data-stu-id="a7659-154">CSV</span></span>

<span data-ttu-id="a7659-155">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="a7659-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="a7659-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="a7659-156">Request</span></span>

<span data-ttu-id="a7659-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a7659-157">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a7659-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="a7659-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageversionsusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageVersionsUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a7659-159">C#</span><span class="sxs-lookup"><span data-stu-id="a7659-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailappusageversionsusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a7659-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a7659-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailappusageversionsusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a7659-161">Цель — C</span><span class="sxs-lookup"><span data-stu-id="a7659-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailappusageversionsusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a7659-162">Java</span><span class="sxs-lookup"><span data-stu-id="a7659-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getemailappusageversionsusercounts-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a7659-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7659-163">Response</span></span>

<span data-ttu-id="a7659-164">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a7659-164">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="a7659-165">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="a7659-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="a7659-166">JSON</span><span class="sxs-lookup"><span data-stu-id="a7659-166">JSON</span></span>

<span data-ttu-id="a7659-167">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="a7659-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="a7659-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="a7659-168">Request</span></span>

<span data-ttu-id="a7659-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a7659-169">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a7659-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="a7659-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageversionsusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageVersionsUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a7659-171">C#</span><span class="sxs-lookup"><span data-stu-id="a7659-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailappusageversionsusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a7659-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a7659-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailappusageversionsusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a7659-173">Цель — C</span><span class="sxs-lookup"><span data-stu-id="a7659-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailappusageversionsusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a7659-174">Java</span><span class="sxs-lookup"><span data-stu-id="a7659-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getemailappusageversionsusercounts-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a7659-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7659-175">Response</span></span>

<span data-ttu-id="a7659-176">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a7659-176">The following is an example of the response.</span></span>

> <span data-ttu-id="a7659-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a7659-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
