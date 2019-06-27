---
title: 'reportRoot: getMailboxUsageStorage'
description: Узнайте, сколько места занято в хранилище организации.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 85243c1a924351b010a5e13c6e1235d0440a139e
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35267398"
---
# <a name="reportroot-getmailboxusagestorage"></a><span data-ttu-id="0d9a0-103">reportRoot: getMailboxUsageStorage</span><span class="sxs-lookup"><span data-stu-id="0d9a0-103">reportRoot: getMailboxUsageStorage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d9a0-104">Узнайте, сколько места занято в хранилище организации.</span><span class="sxs-lookup"><span data-stu-id="0d9a0-104">Get the amount of storage used in your organization.</span></span>

> <span data-ttu-id="0d9a0-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="0d9a0-105">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="0d9a0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0d9a0-106">Permissions</span></span>

<span data-ttu-id="0d9a0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d9a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0d9a0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0d9a0-109">Permission type</span></span>                        | <span data-ttu-id="0d9a0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0d9a0-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="0d9a0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0d9a0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0d9a0-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0d9a0-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="0d9a0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0d9a0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d9a0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d9a0-114">Not supported.</span></span>                           |
| <span data-ttu-id="0d9a0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0d9a0-115">Application</span></span>                            | <span data-ttu-id="0d9a0-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0d9a0-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="0d9a0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0d9a0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageStorage(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="0d9a0-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="0d9a0-118">Function parameters</span></span>

<span data-ttu-id="0d9a0-119">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="0d9a0-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="0d9a0-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="0d9a0-120">Parameter</span></span> | <span data-ttu-id="0d9a0-121">Тип</span><span class="sxs-lookup"><span data-stu-id="0d9a0-121">Type</span></span>   | <span data-ttu-id="0d9a0-122">Описание</span><span class="sxs-lookup"><span data-stu-id="0d9a0-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="0d9a0-123">period</span><span class="sxs-lookup"><span data-stu-id="0d9a0-123">period</span></span>    | <span data-ttu-id="0d9a0-124">string</span><span class="sxs-lookup"><span data-stu-id="0d9a0-124">string</span></span> | <span data-ttu-id="0d9a0-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="0d9a0-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="0d9a0-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="0d9a0-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="0d9a0-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="0d9a0-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="0d9a0-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0d9a0-128">Required.</span></span> |

<span data-ttu-id="0d9a0-129">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="0d9a0-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="0d9a0-130">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="0d9a0-130">The default output type is text/csv.</span></span> <span data-ttu-id="0d9a0-131">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="0d9a0-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0d9a0-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0d9a0-132">Request headers</span></span>

| <span data-ttu-id="0d9a0-133">Имя</span><span class="sxs-lookup"><span data-stu-id="0d9a0-133">Name</span></span>          | <span data-ttu-id="0d9a0-134">Описание</span><span class="sxs-lookup"><span data-stu-id="0d9a0-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="0d9a0-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0d9a0-135">Authorization</span></span> | <span data-ttu-id="0d9a0-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0d9a0-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="0d9a0-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d9a0-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="0d9a0-139">CSV</span><span class="sxs-lookup"><span data-stu-id="0d9a0-139">CSV</span></span>

<span data-ttu-id="0d9a0-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="0d9a0-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="0d9a0-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="0d9a0-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="0d9a0-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="0d9a0-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="0d9a0-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="0d9a0-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="0d9a0-144">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="0d9a0-144">Report Refresh Date</span></span>
- <span data-ttu-id="0d9a0-145">"Storage Used (Byte)" (Используемый объем хранилища в байтах);</span><span class="sxs-lookup"><span data-stu-id="0d9a0-145">Storage Used (Byte)</span></span>
- <span data-ttu-id="0d9a0-146">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="0d9a0-146">Report Date</span></span>
- <span data-ttu-id="0d9a0-147">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="0d9a0-147">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="0d9a0-148">JSON</span><span class="sxs-lookup"><span data-stu-id="0d9a0-148">JSON</span></span>

<span data-ttu-id="0d9a0-149">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[маилбоксусажестораже](../resources/mailboxusagestorage.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0d9a0-149">If successful, this method returns a `200 OK` response code and a **[mailboxUsageStorage](../resources/mailboxusagestorage.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d9a0-150">Пример</span><span class="sxs-lookup"><span data-stu-id="0d9a0-150">Example</span></span>

### <a name="csv"></a><span data-ttu-id="0d9a0-151">CSV</span><span class="sxs-lookup"><span data-stu-id="0d9a0-151">CSV</span></span>

<span data-ttu-id="0d9a0-152">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="0d9a0-152">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="0d9a0-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d9a0-153">Request</span></span>

<span data-ttu-id="0d9a0-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0d9a0-154">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagestorage_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageStorage(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="0d9a0-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d9a0-155">Response</span></span>

<span data-ttu-id="0d9a0-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0d9a0-156">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="0d9a0-157">Образец кода SDK</span><span class="sxs-lookup"><span data-stu-id="0d9a0-157">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0d9a0-158">C#</span><span class="sxs-lookup"><span data-stu-id="0d9a0-158">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getmailboxusagestorage_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0d9a0-159">Javascript</span><span class="sxs-lookup"><span data-stu-id="0d9a0-159">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getmailboxusagestorage_csv-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="0d9a0-160">Цель — C</span><span class="sxs-lookup"><span data-stu-id="0d9a0-160">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getmailboxusagestorage_csv-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="0d9a0-161">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="0d9a0-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Storage Used (Byte),Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="0d9a0-162">JSON</span><span class="sxs-lookup"><span data-stu-id="0d9a0-162">JSON</span></span>

<span data-ttu-id="0d9a0-163">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="0d9a0-163">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="0d9a0-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d9a0-164">Request</span></span>

<span data-ttu-id="0d9a0-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0d9a0-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagestorage_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageStorage(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="0d9a0-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d9a0-166">Response</span></span>

<span data-ttu-id="0d9a0-167">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0d9a0-167">The following is an example of the response.</span></span>

> <span data-ttu-id="0d9a0-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0d9a0-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxUsageStorage"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 235

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.mailboxUsageStorage)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "storageUsedInBytes": 5159432679270, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="0d9a0-170">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="0d9a0-170">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0d9a0-171">C#</span><span class="sxs-lookup"><span data-stu-id="0d9a0-171">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getmailboxusagestorage_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0d9a0-172">Javascript</span><span class="sxs-lookup"><span data-stu-id="0d9a0-172">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getmailboxusagestorage_json-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="0d9a0-173">Цель — C</span><span class="sxs-lookup"><span data-stu-id="0d9a0-173">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getmailboxusagestorage_json-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getmailboxusagestorage.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getmailboxusagestorage.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getmailboxusagestorage.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getmailboxusagestorage.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getmailboxusagestorage.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
