---
title: 'reportRoot: getMailboxUsageDetail'
description: Получите сведения об использовании почтовых ящиков.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: fde6fd233ef61cfce718898418c9a2b756c253df
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873812"
---
# <a name="reportroot-getmailboxusagedetail"></a><span data-ttu-id="a075a-103">reportRoot: getMailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="a075a-103">reportRoot: getMailboxUsageDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a075a-104">Получите сведения об использовании почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="a075a-104">Get details about mailbox usage.</span></span>

> <span data-ttu-id="a075a-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="a075a-105">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="a075a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a075a-106">Permissions</span></span>

<span data-ttu-id="a075a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a075a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a075a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a075a-109">Permission type</span></span>                        | <span data-ttu-id="a075a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a075a-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="a075a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a075a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a075a-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a075a-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="a075a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a075a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a075a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a075a-114">Not supported.</span></span>                           |
| <span data-ttu-id="a075a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a075a-115">Application</span></span>                            | <span data-ttu-id="a075a-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a075a-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="a075a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a075a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageDetail(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="a075a-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="a075a-118">Function parameters</span></span>

<span data-ttu-id="a075a-119">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="a075a-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="a075a-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="a075a-120">Parameter</span></span> | <span data-ttu-id="a075a-121">Тип</span><span class="sxs-lookup"><span data-stu-id="a075a-121">Type</span></span>   | <span data-ttu-id="a075a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a075a-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="a075a-123">period</span><span class="sxs-lookup"><span data-stu-id="a075a-123">period</span></span>    | <span data-ttu-id="a075a-124">string</span><span class="sxs-lookup"><span data-stu-id="a075a-124">string</span></span> | <span data-ttu-id="a075a-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="a075a-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="a075a-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="a075a-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="a075a-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="a075a-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="a075a-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a075a-128">Required.</span></span> |

<span data-ttu-id="a075a-129">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a075a-129">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="a075a-130">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="a075a-130">The default output type is text/csv.</span></span> <span data-ttu-id="a075a-131">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="a075a-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a075a-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a075a-132">Request headers</span></span>

| <span data-ttu-id="a075a-133">Имя</span><span class="sxs-lookup"><span data-stu-id="a075a-133">Name</span></span>          | <span data-ttu-id="a075a-134">Описание</span><span class="sxs-lookup"><span data-stu-id="a075a-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="a075a-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a075a-135">Authorization</span></span> | <span data-ttu-id="a075a-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a075a-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="a075a-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="a075a-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="a075a-139">CSV</span><span class="sxs-lookup"><span data-stu-id="a075a-139">CSV</span></span>

<span data-ttu-id="a075a-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="a075a-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="a075a-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="a075a-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="a075a-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="a075a-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="a075a-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="a075a-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="a075a-144">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="a075a-144">Report Refresh Date</span></span>
- <span data-ttu-id="a075a-145">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="a075a-145">User Principal Name</span></span>
- <span data-ttu-id="a075a-146">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="a075a-146">Display Name</span></span>
- <span data-ttu-id="a075a-147">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="a075a-147">Is Deleted</span></span>
- <span data-ttu-id="a075a-148">Deleted Date (дата удаления)</span><span class="sxs-lookup"><span data-stu-id="a075a-148">Deleted Date</span></span>
- <span data-ttu-id="a075a-149">Created Date (дата создания)</span><span class="sxs-lookup"><span data-stu-id="a075a-149">Created Date</span></span>
- <span data-ttu-id="a075a-150">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="a075a-150">Last Activity Date</span></span>
- <span data-ttu-id="a075a-151">Item Count (количество элементов)</span><span class="sxs-lookup"><span data-stu-id="a075a-151">Item Count</span></span>
- <span data-ttu-id="a075a-152">Storage Used (Byte) [использовано (байт)]</span><span class="sxs-lookup"><span data-stu-id="a075a-152">Storage Used (Byte)</span></span>
- <span data-ttu-id="a075a-153">Issue Warning Quota (Byte) [объем, при котором выводится предупреждение (байт)]</span><span class="sxs-lookup"><span data-stu-id="a075a-153">Issue Warning Quota (Byte)</span></span>
- <span data-ttu-id="a075a-154">Prohibit Send Quota (Byte) [объем, при котором блокируется отправка (байт)]</span><span class="sxs-lookup"><span data-stu-id="a075a-154">Prohibit Send Quota (Byte)</span></span>
- <span data-ttu-id="a075a-155">Prohibit Send/Receive Quota (Byte) [объем, при котором блокируются отправка и получение (байт)]</span><span class="sxs-lookup"><span data-stu-id="a075a-155">Prohibit Send/Receive Quota (Byte)</span></span>
- <span data-ttu-id="a075a-156">Число удаленных элементов</span><span class="sxs-lookup"><span data-stu-id="a075a-156">Deleted Item Count</span></span>
- <span data-ttu-id="a075a-157">Размер удаленного элемента (Byte)</span><span class="sxs-lookup"><span data-stu-id="a075a-157">Deleted Item Size (Byte)</span></span>
- <span data-ttu-id="a075a-158">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="a075a-158">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="a075a-159">JSON</span><span class="sxs-lookup"><span data-stu-id="a075a-159">JSON</span></span>

<span data-ttu-id="a075a-160">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[маилбоксусажедетаил](../resources/mailboxusagedetail.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a075a-160">If successful, this method returns a `200 OK` response code and a **[mailboxUsageDetail](../resources/mailboxusagedetail.md)** object in the response body.</span></span>

<span data-ttu-id="a075a-161">Размер страницы по умолчанию для этого запроса составляет 200 элементов.</span><span class="sxs-lookup"><span data-stu-id="a075a-161">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="a075a-162">Пример</span><span class="sxs-lookup"><span data-stu-id="a075a-162">Example</span></span>

### <a name="csv"></a><span data-ttu-id="a075a-163">CSV</span><span class="sxs-lookup"><span data-stu-id="a075a-163">CSV</span></span>

<span data-ttu-id="a075a-164">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="a075a-164">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="a075a-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="a075a-165">Request</span></span>

<span data-ttu-id="a075a-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a075a-166">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a075a-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="a075a-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagedetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a075a-168">C#</span><span class="sxs-lookup"><span data-stu-id="a075a-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getmailboxusagedetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a075a-169">Javascript</span><span class="sxs-lookup"><span data-stu-id="a075a-169">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getmailboxusagedetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a075a-170">Цель — C</span><span class="sxs-lookup"><span data-stu-id="a075a-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getmailboxusagedetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a075a-171">Java</span><span class="sxs-lookup"><span data-stu-id="a075a-171">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getmailboxusagedetail-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a075a-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="a075a-172">Response</span></span>

<span data-ttu-id="a075a-173">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a075a-173">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="a075a-174">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="a075a-174">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Created Date,Last Activity Date,Item Count,Storage Used (Byte),Issue Warning Quota (Byte),Prohibit Send Quota (Byte),Prohibit Send/Receive Quota (Byte),Deleted Item Count,Deleted Item Size (Byte),Report Period
```

### <a name="json"></a><span data-ttu-id="a075a-175">JSON</span><span class="sxs-lookup"><span data-stu-id="a075a-175">JSON</span></span>

<span data-ttu-id="a075a-176">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="a075a-176">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="a075a-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="a075a-177">Request</span></span>

<span data-ttu-id="a075a-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a075a-178">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a075a-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="a075a-179">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagedetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getMailboxUsageDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a075a-180">C#</span><span class="sxs-lookup"><span data-stu-id="a075a-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getmailboxusagedetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a075a-181">Javascript</span><span class="sxs-lookup"><span data-stu-id="a075a-181">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getmailboxusagedetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a075a-182">Цель — C</span><span class="sxs-lookup"><span data-stu-id="a075a-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getmailboxusagedetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a075a-183">Java</span><span class="sxs-lookup"><span data-stu-id="a075a-183">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getmailboxusagedetail-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a075a-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="a075a-184">Response</span></span>

<span data-ttu-id="a075a-185">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a075a-185">The following is an example of the response.</span></span>

> <span data-ttu-id="a075a-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a075a-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxUsageDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 526

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.mailboxUsageDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "displayName": "displayName-value", 
      "isDeleted": false, 
      "deletedDate": null, 
      "createdDate": "2016-03-30", 
      "lastActivityDate": "2017-09-01", 
      "itemCount": 138481, 
      "storageUsedInBytes": 10414748704, 
      "deletedItemCount": 138481,
      "deletedItemSizeInBytes": 10414748704, 
      "issueWarningQuotaInBytes": 10522698752, 
      "prohibitSendQuotaInBytes": 10630040576, 
      "prohibitSendReceiveQuotaInBytes": 10737418240, 
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
