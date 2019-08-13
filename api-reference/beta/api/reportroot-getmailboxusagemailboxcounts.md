---
title: 'reportRoot: getMailboxUsageMailboxCounts'
description: Узнайте, сколько всего почтовых ящиков в организации и сколько из них были активный в отчетный период. Почтовый ящик считается активным, если пользователь отправил или прочитал по крайней мере одно письмо.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 7d1f2a81c4d007afa937d329c03a234799ab7739
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36308699"
---
# <a name="reportroot-getmailboxusagemailboxcounts"></a><span data-ttu-id="f68a5-104">reportRoot: getMailboxUsageMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="f68a5-104">reportRoot: getMailboxUsageMailboxCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f68a5-105">Узнайте, сколько всего почтовых ящиков в организации и сколько из них были активный в отчетный период.</span><span class="sxs-lookup"><span data-stu-id="f68a5-105">Get the total number of user mailboxes in your organization and how many are active each day of the reporting period.</span></span> <span data-ttu-id="f68a5-106">Почтовый ящик считается активным, если пользователь отправил или прочитал по крайней мере одно письмо.</span><span class="sxs-lookup"><span data-stu-id="f68a5-106">A mailbox is considered active if the user sent or read any email.</span></span>

> <span data-ttu-id="f68a5-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="f68a5-107">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="f68a5-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f68a5-108">Permissions</span></span>

<span data-ttu-id="f68a5-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f68a5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f68a5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f68a5-111">Permission type</span></span>                        | <span data-ttu-id="f68a5-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f68a5-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="f68a5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f68a5-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="f68a5-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f68a5-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="f68a5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f68a5-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f68a5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f68a5-116">Not supported.</span></span>                           |
| <span data-ttu-id="f68a5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f68a5-117">Application</span></span>                            | <span data-ttu-id="f68a5-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f68a5-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="f68a5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f68a5-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageMailboxCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="f68a5-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="f68a5-120">Function parameters</span></span>

<span data-ttu-id="f68a5-121">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="f68a5-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="f68a5-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="f68a5-122">Parameter</span></span> | <span data-ttu-id="f68a5-123">Тип</span><span class="sxs-lookup"><span data-stu-id="f68a5-123">Type</span></span>   | <span data-ttu-id="f68a5-124">Описание</span><span class="sxs-lookup"><span data-stu-id="f68a5-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="f68a5-125">period</span><span class="sxs-lookup"><span data-stu-id="f68a5-125">period</span></span>    | <span data-ttu-id="f68a5-126">string</span><span class="sxs-lookup"><span data-stu-id="f68a5-126">string</span></span> | <span data-ttu-id="f68a5-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="f68a5-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="f68a5-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="f68a5-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="f68a5-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="f68a5-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="f68a5-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f68a5-130">Required.</span></span> |

<span data-ttu-id="f68a5-131">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="f68a5-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="f68a5-132">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="f68a5-132">The default output type is text/csv.</span></span> <span data-ttu-id="f68a5-133">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="f68a5-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f68a5-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f68a5-134">Request headers</span></span>

| <span data-ttu-id="f68a5-135">Имя</span><span class="sxs-lookup"><span data-stu-id="f68a5-135">Name</span></span>          | <span data-ttu-id="f68a5-136">Описание</span><span class="sxs-lookup"><span data-stu-id="f68a5-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="f68a5-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f68a5-137">Authorization</span></span> | <span data-ttu-id="f68a5-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f68a5-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="f68a5-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="f68a5-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="f68a5-141">CSV</span><span class="sxs-lookup"><span data-stu-id="f68a5-141">CSV</span></span>

<span data-ttu-id="f68a5-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="f68a5-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="f68a5-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="f68a5-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="f68a5-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="f68a5-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="f68a5-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="f68a5-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="f68a5-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="f68a5-146">Report Refresh Date</span></span>
- <span data-ttu-id="f68a5-147">Total (всего)</span><span class="sxs-lookup"><span data-stu-id="f68a5-147">Total</span></span>
- <span data-ttu-id="f68a5-148">Active (активные)</span><span class="sxs-lookup"><span data-stu-id="f68a5-148">Active</span></span>
- <span data-ttu-id="f68a5-149">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="f68a5-149">Report Date</span></span>
- <span data-ttu-id="f68a5-150">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="f68a5-150">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="f68a5-151">JSON</span><span class="sxs-lookup"><span data-stu-id="f68a5-151">JSON</span></span>

<span data-ttu-id="f68a5-152">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[маилбоксусажемаилбокскаунтс](../resources/mailboxusagemailboxcounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f68a5-152">If successful, this method returns a `200 OK` response code and a **[mailboxUsageMailboxCounts](../resources/mailboxusagemailboxcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f68a5-153">Пример</span><span class="sxs-lookup"><span data-stu-id="f68a5-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="f68a5-154">CSV</span><span class="sxs-lookup"><span data-stu-id="f68a5-154">CSV</span></span>

<span data-ttu-id="f68a5-155">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="f68a5-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="f68a5-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="f68a5-156">Request</span></span>

<span data-ttu-id="f68a5-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f68a5-157">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f68a5-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="f68a5-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagemailboxcounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageMailboxCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f68a5-159">C#</span><span class="sxs-lookup"><span data-stu-id="f68a5-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getmailboxusagemailboxcounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f68a5-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f68a5-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getmailboxusagemailboxcounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f68a5-161">Цель — C</span><span class="sxs-lookup"><span data-stu-id="f68a5-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getmailboxusagemailboxcounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f68a5-162">Java</span><span class="sxs-lookup"><span data-stu-id="f68a5-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getmailboxusagemailboxcounts-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f68a5-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="f68a5-163">Response</span></span>

<span data-ttu-id="f68a5-164">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f68a5-164">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="f68a5-165">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="f68a5-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Total,Active,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="f68a5-166">JSON</span><span class="sxs-lookup"><span data-stu-id="f68a5-166">JSON</span></span>

<span data-ttu-id="f68a5-167">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="f68a5-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="f68a5-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="f68a5-168">Request</span></span>

<span data-ttu-id="f68a5-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f68a5-169">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f68a5-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="f68a5-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagemailboxcounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageMailboxCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f68a5-171">C#</span><span class="sxs-lookup"><span data-stu-id="f68a5-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getmailboxusagemailboxcounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f68a5-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f68a5-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getmailboxusagemailboxcounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f68a5-173">Цель — C</span><span class="sxs-lookup"><span data-stu-id="f68a5-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getmailboxusagemailboxcounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f68a5-174">Java</span><span class="sxs-lookup"><span data-stu-id="f68a5-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getmailboxusagemailboxcounts-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f68a5-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="f68a5-175">Response</span></span>

<span data-ttu-id="f68a5-176">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f68a5-176">The following is an example of the response.</span></span>

> <span data-ttu-id="f68a5-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f68a5-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxUsageMailboxCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 232

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.mailboxUsageMailboxCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "total": 202, 
      "active": 198, 
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
