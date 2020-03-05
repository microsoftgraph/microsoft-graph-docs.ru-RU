---
title: 'reportRoot: getYammerActivityCounts'
description: Отслеживайте динамику активности пользователей в Yammer по количеству опубликованных, прочитанных и понравившихся сообщений.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: aa86597db27f2621f7a480cf7bc41229cb0737e6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453998"
---
# <a name="reportroot-getyammeractivitycounts"></a><span data-ttu-id="a8245-103">reportRoot: getYammerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="a8245-103">reportRoot: getYammerActivityCounts</span></span>

<span data-ttu-id="a8245-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a8245-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8245-105">Отслеживайте динамику активности пользователей в Yammer по количеству опубликованных, прочитанных и понравившихся сообщений.</span><span class="sxs-lookup"><span data-stu-id="a8245-105">Get the trends on the amount of Yammer activity in your organization by how many messages were posted, read, and liked.</span></span>

> <span data-ttu-id="a8245-106">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span><span class="sxs-lookup"><span data-stu-id="a8245-106">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="permissions"></a><span data-ttu-id="a8245-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a8245-107">Permissions</span></span>

<span data-ttu-id="a8245-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8245-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a8245-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a8245-110">Permission type</span></span>                        | <span data-ttu-id="a8245-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a8245-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="a8245-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a8245-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a8245-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8245-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="a8245-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a8245-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8245-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8245-115">Not supported.</span></span>                           |
| <span data-ttu-id="a8245-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a8245-116">Application</span></span>                            | <span data-ttu-id="a8245-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8245-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="a8245-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a8245-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="a8245-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="a8245-119">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="a8245-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a8245-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="a8245-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="a8245-121">Function parameters</span></span>

<span data-ttu-id="a8245-122">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="a8245-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="a8245-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="a8245-123">Parameter</span></span> | <span data-ttu-id="a8245-124">Тип</span><span class="sxs-lookup"><span data-stu-id="a8245-124">Type</span></span>   | <span data-ttu-id="a8245-125">Описание</span><span class="sxs-lookup"><span data-stu-id="a8245-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="a8245-126">period</span><span class="sxs-lookup"><span data-stu-id="a8245-126">period</span></span>    | <span data-ttu-id="a8245-127">string</span><span class="sxs-lookup"><span data-stu-id="a8245-127">string</span></span> | <span data-ttu-id="a8245-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="a8245-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="a8245-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="a8245-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="a8245-130">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="a8245-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="a8245-131">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a8245-131">Required.</span></span> |

<span data-ttu-id="a8245-132">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="a8245-132">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="a8245-133">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="a8245-133">The default output type is text/csv.</span></span> <span data-ttu-id="a8245-134">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="a8245-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a8245-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a8245-135">Request headers</span></span>

| <span data-ttu-id="a8245-136">Имя</span><span class="sxs-lookup"><span data-stu-id="a8245-136">Name</span></span>          | <span data-ttu-id="a8245-137">Описание</span><span class="sxs-lookup"><span data-stu-id="a8245-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="a8245-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a8245-138">Authorization</span></span> | <span data-ttu-id="a8245-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a8245-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="a8245-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="a8245-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="a8245-142">CSV</span><span class="sxs-lookup"><span data-stu-id="a8245-142">CSV</span></span>

<span data-ttu-id="a8245-143">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="a8245-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="a8245-144">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="a8245-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="a8245-145">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="a8245-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="a8245-146">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="a8245-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="a8245-147">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="a8245-147">Report Refresh Date</span></span>
- <span data-ttu-id="a8245-148">"Liked" (Понравилось);</span><span class="sxs-lookup"><span data-stu-id="a8245-148">Liked</span></span>
- <span data-ttu-id="a8245-149">"Posted" (Опубликовано);</span><span class="sxs-lookup"><span data-stu-id="a8245-149">Posted</span></span>
- <span data-ttu-id="a8245-150">"Read" (Чтение);</span><span class="sxs-lookup"><span data-stu-id="a8245-150">Read</span></span>
- <span data-ttu-id="a8245-151">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="a8245-151">Report Date</span></span>
- <span data-ttu-id="a8245-152">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="a8245-152">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="a8245-153">JSON</span><span class="sxs-lookup"><span data-stu-id="a8245-153">JSON</span></span>

<span data-ttu-id="a8245-154">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[яммерактивитисуммари](../resources/yammeractivitysummary.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a8245-154">If successful, this method returns a `200 OK` response code and a **[yammerActivitySummary](../resources/yammeractivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8245-155">Пример</span><span class="sxs-lookup"><span data-stu-id="a8245-155">Example</span></span>

### <a name="csv"></a><span data-ttu-id="a8245-156">CSV</span><span class="sxs-lookup"><span data-stu-id="a8245-156">CSV</span></span>

<span data-ttu-id="a8245-157">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="a8245-157">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="a8245-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="a8245-158">Request</span></span>

<span data-ttu-id="a8245-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a8245-159">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a8245-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="a8245-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivitycounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerActivityCounts(period='D7')?$format=text/csv
```
# <a name="c"></a>[<span data-ttu-id="a8245-161">C#</span><span class="sxs-lookup"><span data-stu-id="a8245-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammeractivitycounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a8245-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a8245-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammeractivitycounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a8245-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a8245-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammeractivitycounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a8245-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="a8245-164">Response</span></span>

<span data-ttu-id="a8245-165">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a8245-165">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="a8245-166">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="a8245-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Liked,Posted,Read,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="a8245-167">JSON</span><span class="sxs-lookup"><span data-stu-id="a8245-167">JSON</span></span>

<span data-ttu-id="a8245-168">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="a8245-168">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="a8245-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="a8245-169">Request</span></span>

<span data-ttu-id="a8245-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a8245-170">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a8245-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="a8245-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivitycounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerActivityCounts(period='D7')?$format=application/json
```
# <a name="c"></a>[<span data-ttu-id="a8245-172">C#</span><span class="sxs-lookup"><span data-stu-id="a8245-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammeractivitycounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a8245-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a8245-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammeractivitycounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a8245-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a8245-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammeractivitycounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a8245-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="a8245-175">Response</span></span>

<span data-ttu-id="a8245-176">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a8245-176">The following is an example of the response.</span></span>

> <span data-ttu-id="a8245-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a8245-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerActivitySummary"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 237

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerActivitySummary)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "liked": 47, 
      "posted": 59, 
      "read": 986, 
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
