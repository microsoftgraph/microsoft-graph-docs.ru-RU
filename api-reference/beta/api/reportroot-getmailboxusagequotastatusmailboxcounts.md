---
title: 'reportRoot: getMailboxUsageQuotaStatusMailboxCounts'
description: Узнайте, сколько почтовых ящиков пользователей в каждой категории квоты.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 7588c445e844bcfc633687078e3b4f4b7eb29388
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873701"
---
# <a name="reportroot-getmailboxusagequotastatusmailboxcounts"></a><span data-ttu-id="10d28-103">reportRoot: getMailboxUsageQuotaStatusMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="10d28-103">reportRoot: getMailboxUsageQuotaStatusMailboxCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10d28-104">Узнайте, сколько почтовых ящиков пользователей в каждой категории квоты.</span><span class="sxs-lookup"><span data-stu-id="10d28-104">Get the count of user mailboxes in each quota category.</span></span>

> <span data-ttu-id="10d28-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="10d28-105">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="10d28-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="10d28-106">Permissions</span></span>

<span data-ttu-id="10d28-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10d28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="10d28-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10d28-109">Permission type</span></span>                        | <span data-ttu-id="10d28-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="10d28-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="10d28-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10d28-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="10d28-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="10d28-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="10d28-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10d28-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10d28-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10d28-114">Not supported.</span></span>                           |
| <span data-ttu-id="10d28-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="10d28-115">Application</span></span>                            | <span data-ttu-id="10d28-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="10d28-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="10d28-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10d28-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageQuotaStatusMailboxCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="10d28-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="10d28-118">Function parameters</span></span>

<span data-ttu-id="10d28-119">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="10d28-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="10d28-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="10d28-120">Parameter</span></span> | <span data-ttu-id="10d28-121">Тип</span><span class="sxs-lookup"><span data-stu-id="10d28-121">Type</span></span>   | <span data-ttu-id="10d28-122">Описание</span><span class="sxs-lookup"><span data-stu-id="10d28-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="10d28-123">period</span><span class="sxs-lookup"><span data-stu-id="10d28-123">period</span></span>    | <span data-ttu-id="10d28-124">string</span><span class="sxs-lookup"><span data-stu-id="10d28-124">string</span></span> | <span data-ttu-id="10d28-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="10d28-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="10d28-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="10d28-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="10d28-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="10d28-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="10d28-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10d28-128">Required.</span></span> |

<span data-ttu-id="10d28-129">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="10d28-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="10d28-130">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="10d28-130">The default output type is text/csv.</span></span> <span data-ttu-id="10d28-131">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="10d28-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="10d28-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10d28-132">Request headers</span></span>

| <span data-ttu-id="10d28-133">Имя</span><span class="sxs-lookup"><span data-stu-id="10d28-133">Name</span></span>          | <span data-ttu-id="10d28-134">Описание</span><span class="sxs-lookup"><span data-stu-id="10d28-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="10d28-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="10d28-135">Authorization</span></span> | <span data-ttu-id="10d28-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10d28-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="10d28-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="10d28-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="10d28-139">CSV</span><span class="sxs-lookup"><span data-stu-id="10d28-139">CSV</span></span>

<span data-ttu-id="10d28-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="10d28-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="10d28-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="10d28-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="10d28-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="10d28-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="10d28-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="10d28-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="10d28-144">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="10d28-144">Report Refresh Date</span></span>
- <span data-ttu-id="10d28-145">Under Limit (ограничение не превышено)</span><span class="sxs-lookup"><span data-stu-id="10d28-145">Under Limit</span></span>
- <span data-ttu-id="10d28-146">Warning Issued (выведено предупреждение)</span><span class="sxs-lookup"><span data-stu-id="10d28-146">Warning Issued</span></span>
- <span data-ttu-id="10d28-147">Send Prohibited (отправка запрещена)</span><span class="sxs-lookup"><span data-stu-id="10d28-147">Send Prohibited</span></span>
- <span data-ttu-id="10d28-148">Send/Receive Prohibited (отправка и получение запрещены)</span><span class="sxs-lookup"><span data-stu-id="10d28-148">Send/Receive Prohibited</span></span>
- <span data-ttu-id="10d28-149">Indeterminate (не определено)</span><span class="sxs-lookup"><span data-stu-id="10d28-149">Indeterminate</span></span>
- <span data-ttu-id="10d28-150">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="10d28-150">Report Date</span></span>
- <span data-ttu-id="10d28-151">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="10d28-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="10d28-152">JSON</span><span class="sxs-lookup"><span data-stu-id="10d28-152">JSON</span></span>

<span data-ttu-id="10d28-153">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[маилбоксусажекуотастатусмаилбокскаунтс](../resources/mailboxusagequotastatusmailboxcounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="10d28-153">If successful, this method returns a `200 OK` response code and a **[mailboxUsageQuotaStatusMailboxCounts](../resources/mailboxusagequotastatusmailboxcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10d28-154">Пример</span><span class="sxs-lookup"><span data-stu-id="10d28-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="10d28-155">CSV</span><span class="sxs-lookup"><span data-stu-id="10d28-155">CSV</span></span>

<span data-ttu-id="10d28-156">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="10d28-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="10d28-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="10d28-157">Request</span></span>

<span data-ttu-id="10d28-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10d28-158">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="10d28-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="10d28-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagequotastatusmailboxcounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageQuotaStatusMailboxCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="10d28-160">C#</span><span class="sxs-lookup"><span data-stu-id="10d28-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getmailboxusagequotastatusmailboxcounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="10d28-161">Javascript</span><span class="sxs-lookup"><span data-stu-id="10d28-161">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getmailboxusagequotastatusmailboxcounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="10d28-162">Цель — C</span><span class="sxs-lookup"><span data-stu-id="10d28-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getmailboxusagequotastatusmailboxcounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="10d28-163">Java</span><span class="sxs-lookup"><span data-stu-id="10d28-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getmailboxusagequotastatusmailboxcounts-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="10d28-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="10d28-164">Response</span></span>

<span data-ttu-id="10d28-165">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="10d28-165">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="10d28-166">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="10d28-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Under Limit,Warning Issued,Send Prohibited,Send/Receive Prohibited,Indeterminate,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="10d28-167">JSON</span><span class="sxs-lookup"><span data-stu-id="10d28-167">JSON</span></span>

<span data-ttu-id="10d28-168">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="10d28-168">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="10d28-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="10d28-169">Request</span></span>

<span data-ttu-id="10d28-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10d28-170">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="10d28-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="10d28-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagequotastatusmailboxcounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageQuotaStatusMailboxCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="10d28-172">C#</span><span class="sxs-lookup"><span data-stu-id="10d28-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getmailboxusagequotastatusmailboxcounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="10d28-173">Javascript</span><span class="sxs-lookup"><span data-stu-id="10d28-173">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getmailboxusagequotastatusmailboxcounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="10d28-174">Цель — C</span><span class="sxs-lookup"><span data-stu-id="10d28-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getmailboxusagequotastatusmailboxcounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="10d28-175">Java</span><span class="sxs-lookup"><span data-stu-id="10d28-175">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getmailboxusagequotastatusmailboxcounts-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="10d28-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="10d28-176">Response</span></span>

<span data-ttu-id="10d28-177">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="10d28-177">The following is an example of the response.</span></span>

> <span data-ttu-id="10d28-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="10d28-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxUsageQuotaStatusMailboxCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 311

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.mailboxUsageQuotaMailboxStatusCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "underLimit": 155, 
      "warningIssued": 0, 
      "sendProhibited": 0, 
      "sendReceiveProhibited": 0, 
      "indeterminate": 14, 
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
