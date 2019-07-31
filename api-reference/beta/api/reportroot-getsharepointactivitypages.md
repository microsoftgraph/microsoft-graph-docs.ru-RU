---
title: 'reportRoot: getSharePointActivityPages'
description: Узнайте, сколько уникальных страниц посетили пользователи.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 676d23d813488a2c1741027badd0154731d35bf4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35983182"
---
# <a name="reportroot-getsharepointactivitypages"></a><span data-ttu-id="b5208-103">reportRoot: getSharePointActivityPages</span><span class="sxs-lookup"><span data-stu-id="b5208-103">reportRoot: getSharePointActivityPages</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5208-104">Узнайте, сколько уникальных страниц посетили пользователи.</span><span class="sxs-lookup"><span data-stu-id="b5208-104">Get the number of unique pages visited by users.</span></span>

> <span data-ttu-id="b5208-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="b5208-105">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="b5208-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b5208-106">Permissions</span></span>

<span data-ttu-id="b5208-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5208-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b5208-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b5208-109">Permission type</span></span>                        | <span data-ttu-id="b5208-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b5208-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b5208-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b5208-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b5208-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b5208-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b5208-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b5208-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5208-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5208-114">Not supported.</span></span>                           |
| <span data-ttu-id="b5208-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b5208-115">Application</span></span>                            | <span data-ttu-id="b5208-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b5208-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="b5208-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b5208-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityPages(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="b5208-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="b5208-118">Function parameters</span></span>

<span data-ttu-id="b5208-119">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="b5208-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="b5208-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="b5208-120">Parameter</span></span> | <span data-ttu-id="b5208-121">Тип</span><span class="sxs-lookup"><span data-stu-id="b5208-121">Type</span></span>   | <span data-ttu-id="b5208-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b5208-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b5208-123">period</span><span class="sxs-lookup"><span data-stu-id="b5208-123">period</span></span>    | <span data-ttu-id="b5208-124">string</span><span class="sxs-lookup"><span data-stu-id="b5208-124">string</span></span> | <span data-ttu-id="b5208-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="b5208-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b5208-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="b5208-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b5208-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="b5208-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="b5208-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b5208-128">Required.</span></span> |

<span data-ttu-id="b5208-129">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="b5208-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="b5208-130">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="b5208-130">The default output type is text/csv.</span></span> <span data-ttu-id="b5208-131">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="b5208-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b5208-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b5208-132">Request headers</span></span>

| <span data-ttu-id="b5208-133">Имя</span><span class="sxs-lookup"><span data-stu-id="b5208-133">Name</span></span>          | <span data-ttu-id="b5208-134">Описание</span><span class="sxs-lookup"><span data-stu-id="b5208-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="b5208-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b5208-135">Authorization</span></span> | <span data-ttu-id="b5208-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b5208-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="b5208-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5208-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="b5208-139">CSV</span><span class="sxs-lookup"><span data-stu-id="b5208-139">CSV</span></span>

<span data-ttu-id="b5208-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="b5208-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b5208-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="b5208-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b5208-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="b5208-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b5208-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="b5208-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b5208-144">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="b5208-144">Report Refresh Date</span></span>
- <span data-ttu-id="b5208-145">Visited Page Count (количество посещенных страниц)</span><span class="sxs-lookup"><span data-stu-id="b5208-145">Visited Page Count</span></span>
- <span data-ttu-id="b5208-146">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="b5208-146">Report Date</span></span>
- <span data-ttu-id="b5208-147">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="b5208-147">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="b5208-148">JSON</span><span class="sxs-lookup"><span data-stu-id="b5208-148">JSON</span></span>

<span data-ttu-id="b5208-149">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[шарепоинтактивитипажес](../resources/sharepointactivitypages.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b5208-149">If successful, this method returns a `200 OK` response code and a **[sharePointActivityPages](../resources/sharepointactivitypages.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5208-150">Пример</span><span class="sxs-lookup"><span data-stu-id="b5208-150">Example</span></span>

### <a name="csv"></a><span data-ttu-id="b5208-151">CSV</span><span class="sxs-lookup"><span data-stu-id="b5208-151">CSV</span></span>

<span data-ttu-id="b5208-152">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="b5208-152">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="b5208-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5208-153">Request</span></span>

<span data-ttu-id="b5208-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b5208-154">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b5208-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="b5208-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivitypages_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityPages(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b5208-156">C#</span><span class="sxs-lookup"><span data-stu-id="b5208-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointactivitypages-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b5208-157">Javascript</span><span class="sxs-lookup"><span data-stu-id="b5208-157">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointactivitypages-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b5208-158">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b5208-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointactivitypages-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b5208-159">Java</span><span class="sxs-lookup"><span data-stu-id="b5208-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getsharepointactivitypages-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b5208-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5208-160">Response</span></span>

<span data-ttu-id="b5208-161">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b5208-161">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="b5208-162">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="b5208-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Visited Page Count,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="b5208-163">JSON</span><span class="sxs-lookup"><span data-stu-id="b5208-163">JSON</span></span>

<span data-ttu-id="b5208-164">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="b5208-164">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="b5208-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5208-165">Request</span></span>

<span data-ttu-id="b5208-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b5208-166">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b5208-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="b5208-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivitypages_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityPages(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b5208-168">C#</span><span class="sxs-lookup"><span data-stu-id="b5208-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointactivitypages-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b5208-169">Javascript</span><span class="sxs-lookup"><span data-stu-id="b5208-169">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointactivitypages-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b5208-170">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b5208-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointactivitypages-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b5208-171">Java</span><span class="sxs-lookup"><span data-stu-id="b5208-171">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getsharepointactivitypages-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b5208-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5208-172">Response</span></span>

<span data-ttu-id="b5208-173">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b5208-173">The following is an example of the response.</span></span>

> <span data-ttu-id="b5208-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b5208-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointActivityPages"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 228

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.sharePointActivityPages)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "visitedPageCount": 195, 
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
