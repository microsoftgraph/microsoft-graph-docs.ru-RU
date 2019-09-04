---
title: 'reportRoot: getEmailAppUsageUserDetail'
description: Узнайте, какие действия пользователи выполняли в различных почтовых приложениях.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 16785097219a53c78502d72b2f2d06c0c741411e
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36723128"
---
# <a name="reportroot-getemailappusageuserdetail"></a><span data-ttu-id="085c8-103">reportRoot: getEmailAppUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="085c8-103">reportRoot: getEmailAppUsageUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="085c8-104">Узнайте, какие действия пользователи выполняли в различных почтовых приложениях.</span><span class="sxs-lookup"><span data-stu-id="085c8-104">Get details about which activities users performed on the various email apps.</span></span>

> <span data-ttu-id="085c8-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: использование почтовых приложений](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span><span class="sxs-lookup"><span data-stu-id="085c8-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="085c8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="085c8-106">Permissions</span></span>

<span data-ttu-id="085c8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="085c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="085c8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="085c8-109">Permission type</span></span>                        | <span data-ttu-id="085c8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="085c8-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="085c8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="085c8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="085c8-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="085c8-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="085c8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="085c8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="085c8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="085c8-114">Not supported.</span></span>                           |
| <span data-ttu-id="085c8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="085c8-115">Application</span></span>                            | <span data-ttu-id="085c8-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="085c8-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="085c8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="085c8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageUserDetail(period='{period_value}')
GET /reports/getEmailAppUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="085c8-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="085c8-118">Function parameters</span></span>

<span data-ttu-id="085c8-119">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="085c8-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="085c8-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="085c8-120">Parameter</span></span> | <span data-ttu-id="085c8-121">Тип</span><span class="sxs-lookup"><span data-stu-id="085c8-121">Type</span></span>   | <span data-ttu-id="085c8-122">Описание</span><span class="sxs-lookup"><span data-stu-id="085c8-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="085c8-123">period</span><span class="sxs-lookup"><span data-stu-id="085c8-123">period</span></span>    | <span data-ttu-id="085c8-124">string</span><span class="sxs-lookup"><span data-stu-id="085c8-124">string</span></span> | <span data-ttu-id="085c8-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="085c8-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="085c8-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="085c8-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="085c8-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="085c8-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="085c8-128">date</span><span class="sxs-lookup"><span data-stu-id="085c8-128">date</span></span>      | <span data-ttu-id="085c8-129">Date</span><span class="sxs-lookup"><span data-stu-id="085c8-129">Date</span></span>   | <span data-ttu-id="085c8-130">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="085c8-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="085c8-131">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="085c8-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="085c8-132">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="085c8-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="085c8-133">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="085c8-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="085c8-134">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="085c8-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="085c8-135">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="085c8-135">The default output type is text/csv.</span></span> <span data-ttu-id="085c8-136">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="085c8-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="085c8-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="085c8-137">Request headers</span></span>

| <span data-ttu-id="085c8-138">Имя</span><span class="sxs-lookup"><span data-stu-id="085c8-138">Name</span></span>          | <span data-ttu-id="085c8-139">Описание</span><span class="sxs-lookup"><span data-stu-id="085c8-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="085c8-140">Авторизация</span><span class="sxs-lookup"><span data-stu-id="085c8-140">Authorization</span></span> | <span data-ttu-id="085c8-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="085c8-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="085c8-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="085c8-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="085c8-144">CSV</span><span class="sxs-lookup"><span data-stu-id="085c8-144">CSV</span></span>

<span data-ttu-id="085c8-145">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="085c8-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="085c8-146">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="085c8-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="085c8-147">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="085c8-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="085c8-148">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="085c8-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="085c8-149">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="085c8-149">Report Refresh Date</span></span>
- <span data-ttu-id="085c8-150">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="085c8-150">User Principal Name</span></span>
- <span data-ttu-id="085c8-151">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="085c8-151">Display Name</span></span>
- <span data-ttu-id="085c8-152">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="085c8-152">Is Deleted</span></span>
- <span data-ttu-id="085c8-153">"Deleted Date" (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="085c8-153">Deleted Date</span></span>
- <span data-ttu-id="085c8-154">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="085c8-154">Last Activity Date</span></span>
- <span data-ttu-id="085c8-155">"Mail For Mac" (Почта для Mac);</span><span class="sxs-lookup"><span data-stu-id="085c8-155">Mail For Mac</span></span>
- <span data-ttu-id="085c8-156">"Outlook For Mac" (Outlook для Mac);</span><span class="sxs-lookup"><span data-stu-id="085c8-156">Outlook For Mac</span></span>
- <span data-ttu-id="085c8-157">"Outlook For Windows" (Outlook для Windows);</span><span class="sxs-lookup"><span data-stu-id="085c8-157">Outlook For Windows</span></span>
- <span data-ttu-id="085c8-158">"Outlook For Mobile" (Outlook для мобильных устройств);</span><span class="sxs-lookup"><span data-stu-id="085c8-158">Outlook For Mobile</span></span>
- <span data-ttu-id="085c8-159">"Other For Mobile" (Другое для мобильных устройств);</span><span class="sxs-lookup"><span data-stu-id="085c8-159">Other For Mobile</span></span>
- <span data-ttu-id="085c8-160">"Outlook For Web" (Outlook для браузера);</span><span class="sxs-lookup"><span data-stu-id="085c8-160">Outlook For Web</span></span>
- <span data-ttu-id="085c8-161">"POP3 App" (Приложение с поддержкой POP3);</span><span class="sxs-lookup"><span data-stu-id="085c8-161">POP3 App</span></span>
- <span data-ttu-id="085c8-162">"IMAP4 App" (Приложение с поддержкой IMAP4);</span><span class="sxs-lookup"><span data-stu-id="085c8-162">IMAP4 App</span></span>
- <span data-ttu-id="085c8-163">"SMTP App" (Приложение с поддержкой SMTP);</span><span class="sxs-lookup"><span data-stu-id="085c8-163">SMTP App</span></span>
- <span data-ttu-id="085c8-164">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="085c8-164">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="085c8-165">JSON</span><span class="sxs-lookup"><span data-stu-id="085c8-165">JSON</span></span>

<span data-ttu-id="085c8-166">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[емаилаппусажеусердетаил](../resources/emailappusageuserdetail.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="085c8-166">If successful, this method returns a `200 OK` response code and an **[emailAppUsageUserDetail](../resources/emailappusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="085c8-167">Размер страницы по умолчанию для этого запроса составляет 200 элементов.</span><span class="sxs-lookup"><span data-stu-id="085c8-167">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="085c8-168">Пример</span><span class="sxs-lookup"><span data-stu-id="085c8-168">Example</span></span>

### <a name="csv"></a><span data-ttu-id="085c8-169">CSV</span><span class="sxs-lookup"><span data-stu-id="085c8-169">CSV</span></span>

<span data-ttu-id="085c8-170">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="085c8-170">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="085c8-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="085c8-171">Request</span></span>

<span data-ttu-id="085c8-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="085c8-172">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="085c8-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="085c8-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageUserDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="085c8-174">C#</span><span class="sxs-lookup"><span data-stu-id="085c8-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailappusageuserdetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="085c8-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="085c8-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailappusageuserdetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="085c8-176">Цель — C</span><span class="sxs-lookup"><span data-stu-id="085c8-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailappusageuserdetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="085c8-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="085c8-177">Response</span></span>

<span data-ttu-id="085c8-178">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="085c8-178">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="085c8-179">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="085c8-179">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Last Activity Date,Mail For Mac,Outlook For Mac,Outlook For Windows,Outlook For Mobile,Other For Mobile,Outlook For Web,POP3 App,IMAP4 App,SMTP App,Report Period
```

### <a name="json"></a><span data-ttu-id="085c8-180">JSON</span><span class="sxs-lookup"><span data-stu-id="085c8-180">JSON</span></span>

<span data-ttu-id="085c8-181">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="085c8-181">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="085c8-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="085c8-182">Request</span></span>

<span data-ttu-id="085c8-183">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="085c8-183">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="085c8-184">HTTP</span><span class="sxs-lookup"><span data-stu-id="085c8-184">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageUserDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="085c8-185">C#</span><span class="sxs-lookup"><span data-stu-id="085c8-185">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailappusageuserdetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="085c8-186">JavaScript</span><span class="sxs-lookup"><span data-stu-id="085c8-186">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailappusageuserdetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="085c8-187">Цель — C</span><span class="sxs-lookup"><span data-stu-id="085c8-187">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailappusageuserdetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="085c8-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="085c8-188">Response</span></span>

<span data-ttu-id="085c8-189">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="085c8-189">The following is an example of the response.</span></span>

> <span data-ttu-id="085c8-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="085c8-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAppUsageUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 515

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailAppUsageUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "displayName": "displayName-value", 
      "isDeleted": false, 
      "deletedDate": null, 
      "lastActivityDate": "2017-09-01", 
      "mailForMac": [ ], 
      "outlookForMac": [ ], 
      "outlookForWindows": [ ], 
      "outlookForMobile": [
        "Undetermined"
      ], 
      "otherForMobile": [ ], 
      "outlookForWeb": [
        "Undetermined"
      ], 
      "pop3App": [ ], 
      "imap4App": [ ], 
      "smtpApp": [ ], 
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
