---
title: 'reportRoot: getYammerActivityUserDetail'
description: Получите сведения об активности пользователей в Yammer.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: d86d297207cc0a1457c1d9fd26a7a71e60323717
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36411069"
---
# <a name="reportroot-getyammeractivityuserdetail"></a><span data-ttu-id="23e53-103">reportRoot: getYammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="23e53-103">reportRoot: getYammerActivityUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23e53-104">Получите сведения об активности пользователей в Yammer.</span><span class="sxs-lookup"><span data-stu-id="23e53-104">Get details about Yammer activity by user.</span></span>

> <span data-ttu-id="23e53-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span><span class="sxs-lookup"><span data-stu-id="23e53-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="permissions"></a><span data-ttu-id="23e53-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="23e53-106">Permissions</span></span>

<span data-ttu-id="23e53-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23e53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="23e53-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="23e53-109">Permission type</span></span>                        | <span data-ttu-id="23e53-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="23e53-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="23e53-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="23e53-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="23e53-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="23e53-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="23e53-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="23e53-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23e53-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23e53-114">Not supported.</span></span>                           |
| <span data-ttu-id="23e53-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="23e53-115">Application</span></span>                            | <span data-ttu-id="23e53-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="23e53-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="23e53-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="23e53-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerActivityUserDetail(period='{period_value}')
GET /reports/getYammerActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="23e53-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="23e53-118">Function parameters</span></span>

<span data-ttu-id="23e53-119">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="23e53-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="23e53-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="23e53-120">Parameter</span></span> | <span data-ttu-id="23e53-121">Тип</span><span class="sxs-lookup"><span data-stu-id="23e53-121">Type</span></span>   | <span data-ttu-id="23e53-122">Описание</span><span class="sxs-lookup"><span data-stu-id="23e53-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="23e53-123">period</span><span class="sxs-lookup"><span data-stu-id="23e53-123">period</span></span>    | <span data-ttu-id="23e53-124">string</span><span class="sxs-lookup"><span data-stu-id="23e53-124">string</span></span> | <span data-ttu-id="23e53-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="23e53-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="23e53-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="23e53-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="23e53-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="23e53-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="23e53-128">date</span><span class="sxs-lookup"><span data-stu-id="23e53-128">date</span></span>      | <span data-ttu-id="23e53-129">Date</span><span class="sxs-lookup"><span data-stu-id="23e53-129">Date</span></span>   | <span data-ttu-id="23e53-130">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="23e53-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="23e53-131">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="23e53-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="23e53-132">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="23e53-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="23e53-133">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="23e53-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="23e53-134">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="23e53-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="23e53-135">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="23e53-135">The default output type is text/csv.</span></span> <span data-ttu-id="23e53-136">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="23e53-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="23e53-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="23e53-137">Request headers</span></span>

| <span data-ttu-id="23e53-138">Имя</span><span class="sxs-lookup"><span data-stu-id="23e53-138">Name</span></span>          | <span data-ttu-id="23e53-139">Описание</span><span class="sxs-lookup"><span data-stu-id="23e53-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="23e53-140">Авторизация</span><span class="sxs-lookup"><span data-stu-id="23e53-140">Authorization</span></span> | <span data-ttu-id="23e53-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="23e53-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="23e53-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="23e53-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="23e53-144">CSV</span><span class="sxs-lookup"><span data-stu-id="23e53-144">CSV</span></span>

<span data-ttu-id="23e53-145">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="23e53-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="23e53-146">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="23e53-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="23e53-147">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="23e53-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="23e53-148">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="23e53-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="23e53-149">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="23e53-149">Report Refresh Date</span></span>
- <span data-ttu-id="23e53-150">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="23e53-150">User Principal Name</span></span>
- <span data-ttu-id="23e53-151">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="23e53-151">Display Name</span></span>
- <span data-ttu-id="23e53-152">"User State" (Состояние пользователя);</span><span class="sxs-lookup"><span data-stu-id="23e53-152">User State</span></span>
- <span data-ttu-id="23e53-153">"State Change Date" (Дата изменения состояния);</span><span class="sxs-lookup"><span data-stu-id="23e53-153">State Change Date</span></span>
- <span data-ttu-id="23e53-154">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="23e53-154">Last Activity Date</span></span>
- <span data-ttu-id="23e53-155">Posted Count (количество опубликованных сообщений)</span><span class="sxs-lookup"><span data-stu-id="23e53-155">Posted Count</span></span>
- <span data-ttu-id="23e53-156">Read Count (количество прочитанных сообщений)</span><span class="sxs-lookup"><span data-stu-id="23e53-156">Read Count</span></span>
- <span data-ttu-id="23e53-157">Liked Count (количество понравившихся сообщений)</span><span class="sxs-lookup"><span data-stu-id="23e53-157">Liked Count</span></span>
- <span data-ttu-id="23e53-158">Assigned Products (назначенные продукты)</span><span class="sxs-lookup"><span data-stu-id="23e53-158">Assigned Products</span></span>
- <span data-ttu-id="23e53-159">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="23e53-159">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="23e53-160">JSON</span><span class="sxs-lookup"><span data-stu-id="23e53-160">JSON</span></span>

<span data-ttu-id="23e53-161">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[яммерактивитюсердетаил](../resources/yammeractivityuserdetail.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="23e53-161">If successful, this method returns a `200 OK` response code and a **[yammerActivityUserDetail](../resources/yammeractivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="23e53-162">Размер страницы по умолчанию для этого запроса составляет 200 элементов.</span><span class="sxs-lookup"><span data-stu-id="23e53-162">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="23e53-163">Пример</span><span class="sxs-lookup"><span data-stu-id="23e53-163">Example</span></span>

### <a name="csv"></a><span data-ttu-id="23e53-164">CSV</span><span class="sxs-lookup"><span data-stu-id="23e53-164">CSV</span></span>

<span data-ttu-id="23e53-165">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="23e53-165">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="23e53-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="23e53-166">Request</span></span>

<span data-ttu-id="23e53-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23e53-167">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="23e53-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="23e53-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivityuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerActivityUserDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="23e53-169">C#</span><span class="sxs-lookup"><span data-stu-id="23e53-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammeractivityuserdetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="23e53-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="23e53-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammeractivityuserdetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="23e53-171">Цель — C</span><span class="sxs-lookup"><span data-stu-id="23e53-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammeractivityuserdetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="23e53-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="23e53-172">Response</span></span>

<span data-ttu-id="23e53-173">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="23e53-173">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="23e53-174">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="23e53-174">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,User State,State Change Date,Last Activity Date,Posted Count,Read Count,Liked Count,Assigned Products,Report Period
```

### <a name="json"></a><span data-ttu-id="23e53-175">JSON</span><span class="sxs-lookup"><span data-stu-id="23e53-175">JSON</span></span>

<span data-ttu-id="23e53-176">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="23e53-176">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="23e53-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="23e53-177">Request</span></span>

<span data-ttu-id="23e53-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23e53-178">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="23e53-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="23e53-179">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivityuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerActivityUserDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="23e53-180">C#</span><span class="sxs-lookup"><span data-stu-id="23e53-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammeractivityuserdetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="23e53-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="23e53-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammeractivityuserdetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="23e53-182">Цель — C</span><span class="sxs-lookup"><span data-stu-id="23e53-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammeractivityuserdetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="23e53-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="23e53-183">Response</span></span>

<span data-ttu-id="23e53-184">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="23e53-184">The following is an example of the response.</span></span>

> <span data-ttu-id="23e53-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="23e53-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerActivityUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 434

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerActivityUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "displayName": "displayName-value", 
      "userState": "active", 
      "stateChangeDate": "2015-08-26", 
      "lastActivityDate": "2017-09-01", 
      "postedCount": 2, 
      "readCount": 5, 
      "likedCount": 0, 
      "assignedProducts": [
        "OFFICE 365 ENTERPRISE E5"
      ], 
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
