---
title: 'reportRoot: getMailboxUsageStorage'
description: Узнайте, сколько места занято в хранилище организации.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 8978424f583990ff0d4bb497c836d85e7a983e65
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36411776"
---
# <a name="reportroot-getmailboxusagestorage"></a><span data-ttu-id="0dda2-103">reportRoot: getMailboxUsageStorage</span><span class="sxs-lookup"><span data-stu-id="0dda2-103">reportRoot: getMailboxUsageStorage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0dda2-104">Узнайте, сколько места занято в хранилище организации.</span><span class="sxs-lookup"><span data-stu-id="0dda2-104">Get the amount of storage used in your organization.</span></span>

> <span data-ttu-id="0dda2-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="0dda2-105">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="0dda2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0dda2-106">Permissions</span></span>

<span data-ttu-id="0dda2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0dda2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0dda2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0dda2-109">Permission type</span></span>                        | <span data-ttu-id="0dda2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0dda2-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="0dda2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0dda2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0dda2-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0dda2-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="0dda2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0dda2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0dda2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0dda2-114">Not supported.</span></span>                           |
| <span data-ttu-id="0dda2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0dda2-115">Application</span></span>                            | <span data-ttu-id="0dda2-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0dda2-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="0dda2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0dda2-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageStorage(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="0dda2-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="0dda2-118">Function parameters</span></span>

<span data-ttu-id="0dda2-119">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="0dda2-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="0dda2-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="0dda2-120">Parameter</span></span> | <span data-ttu-id="0dda2-121">Тип</span><span class="sxs-lookup"><span data-stu-id="0dda2-121">Type</span></span>   | <span data-ttu-id="0dda2-122">Описание</span><span class="sxs-lookup"><span data-stu-id="0dda2-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="0dda2-123">period</span><span class="sxs-lookup"><span data-stu-id="0dda2-123">period</span></span>    | <span data-ttu-id="0dda2-124">string</span><span class="sxs-lookup"><span data-stu-id="0dda2-124">string</span></span> | <span data-ttu-id="0dda2-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="0dda2-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="0dda2-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="0dda2-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="0dda2-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="0dda2-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="0dda2-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0dda2-128">Required.</span></span> |

<span data-ttu-id="0dda2-129">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="0dda2-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="0dda2-130">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="0dda2-130">The default output type is text/csv.</span></span> <span data-ttu-id="0dda2-131">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="0dda2-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0dda2-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0dda2-132">Request headers</span></span>

| <span data-ttu-id="0dda2-133">Имя</span><span class="sxs-lookup"><span data-stu-id="0dda2-133">Name</span></span>          | <span data-ttu-id="0dda2-134">Описание</span><span class="sxs-lookup"><span data-stu-id="0dda2-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="0dda2-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0dda2-135">Authorization</span></span> | <span data-ttu-id="0dda2-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0dda2-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="0dda2-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="0dda2-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="0dda2-139">CSV</span><span class="sxs-lookup"><span data-stu-id="0dda2-139">CSV</span></span>

<span data-ttu-id="0dda2-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="0dda2-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="0dda2-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="0dda2-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="0dda2-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="0dda2-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="0dda2-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="0dda2-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="0dda2-144">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="0dda2-144">Report Refresh Date</span></span>
- <span data-ttu-id="0dda2-145">"Storage Used (Byte)" (Используемый объем хранилища в байтах);</span><span class="sxs-lookup"><span data-stu-id="0dda2-145">Storage Used (Byte)</span></span>
- <span data-ttu-id="0dda2-146">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="0dda2-146">Report Date</span></span>
- <span data-ttu-id="0dda2-147">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="0dda2-147">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="0dda2-148">JSON</span><span class="sxs-lookup"><span data-stu-id="0dda2-148">JSON</span></span>

<span data-ttu-id="0dda2-149">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[маилбоксусажестораже](../resources/mailboxusagestorage.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0dda2-149">If successful, this method returns a `200 OK` response code and a **[mailboxUsageStorage](../resources/mailboxusagestorage.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0dda2-150">Пример</span><span class="sxs-lookup"><span data-stu-id="0dda2-150">Example</span></span>

### <a name="csv"></a><span data-ttu-id="0dda2-151">CSV</span><span class="sxs-lookup"><span data-stu-id="0dda2-151">CSV</span></span>

<span data-ttu-id="0dda2-152">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="0dda2-152">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="0dda2-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="0dda2-153">Request</span></span>

<span data-ttu-id="0dda2-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0dda2-154">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0dda2-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="0dda2-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagestorage_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageStorage(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0dda2-156">C#</span><span class="sxs-lookup"><span data-stu-id="0dda2-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getmailboxusagestorage-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0dda2-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0dda2-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getmailboxusagestorage-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0dda2-158">Цель — C</span><span class="sxs-lookup"><span data-stu-id="0dda2-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getmailboxusagestorage-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0dda2-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="0dda2-159">Response</span></span>

<span data-ttu-id="0dda2-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0dda2-160">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="0dda2-161">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="0dda2-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="0dda2-162">JSON</span><span class="sxs-lookup"><span data-stu-id="0dda2-162">JSON</span></span>

<span data-ttu-id="0dda2-163">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="0dda2-163">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="0dda2-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="0dda2-164">Request</span></span>

<span data-ttu-id="0dda2-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0dda2-165">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0dda2-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="0dda2-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagestorage_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageStorage(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0dda2-167">C#</span><span class="sxs-lookup"><span data-stu-id="0dda2-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getmailboxusagestorage-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0dda2-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0dda2-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getmailboxusagestorage-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0dda2-169">Цель — C</span><span class="sxs-lookup"><span data-stu-id="0dda2-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getmailboxusagestorage-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0dda2-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="0dda2-170">Response</span></span>

<span data-ttu-id="0dda2-171">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0dda2-171">The following is an example of the response.</span></span>

> <span data-ttu-id="0dda2-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0dda2-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
