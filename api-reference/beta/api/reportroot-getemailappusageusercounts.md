---
title: 'reportRoot: getEmailAppUsageUserCounts'
description: Получение числа уникальных пользователей, которые подключались к Exchange Online с помощью приложения электронной почты.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: e7ae6269e69527c5c3230356c31880969028de6a
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36411853"
---
# <a name="reportroot-getemailappusageusercounts"></a><span data-ttu-id="7f9b5-103">reportRoot: getEmailAppUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="7f9b5-103">reportRoot: getEmailAppUsageUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f9b5-104">Получение числа уникальных пользователей, которые подключались к Exchange Online с помощью приложения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="7f9b5-104">Get the count of unique users that connected to Exchange Online using any email app.</span></span>

> <span data-ttu-id="7f9b5-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Центре администрирования Office 365 — использование почтовых приложений](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span><span class="sxs-lookup"><span data-stu-id="7f9b5-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="7f9b5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7f9b5-106">Permissions</span></span>

<span data-ttu-id="7f9b5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f9b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7f9b5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7f9b5-109">Permission type</span></span>                        | <span data-ttu-id="7f9b5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7f9b5-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="7f9b5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7f9b5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7f9b5-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f9b5-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="7f9b5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7f9b5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f9b5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f9b5-114">Not supported.</span></span>                           |
| <span data-ttu-id="7f9b5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7f9b5-115">Application</span></span>                            | <span data-ttu-id="7f9b5-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f9b5-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="7f9b5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7f9b5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="7f9b5-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="7f9b5-118">Function parameters</span></span>

<span data-ttu-id="7f9b5-119">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="7f9b5-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="7f9b5-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="7f9b5-120">Parameter</span></span> | <span data-ttu-id="7f9b5-121">Тип</span><span class="sxs-lookup"><span data-stu-id="7f9b5-121">Type</span></span>   | <span data-ttu-id="7f9b5-122">Описание</span><span class="sxs-lookup"><span data-stu-id="7f9b5-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="7f9b5-123">period</span><span class="sxs-lookup"><span data-stu-id="7f9b5-123">period</span></span>    | <span data-ttu-id="7f9b5-124">string</span><span class="sxs-lookup"><span data-stu-id="7f9b5-124">string</span></span> | <span data-ttu-id="7f9b5-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="7f9b5-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="7f9b5-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="7f9b5-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="7f9b5-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="7f9b5-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="7f9b5-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7f9b5-128">Required.</span></span> |

<span data-ttu-id="7f9b5-129">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="7f9b5-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="7f9b5-130">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="7f9b5-130">The default output type is text/csv.</span></span> <span data-ttu-id="7f9b5-131">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="7f9b5-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7f9b5-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7f9b5-132">Request headers</span></span>

| <span data-ttu-id="7f9b5-133">Имя</span><span class="sxs-lookup"><span data-stu-id="7f9b5-133">Name</span></span>          | <span data-ttu-id="7f9b5-134">Описание</span><span class="sxs-lookup"><span data-stu-id="7f9b5-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="7f9b5-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7f9b5-135">Authorization</span></span> | <span data-ttu-id="7f9b5-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7f9b5-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="7f9b5-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f9b5-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="7f9b5-139">CSV</span><span class="sxs-lookup"><span data-stu-id="7f9b5-139">CSV</span></span>

<span data-ttu-id="7f9b5-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="7f9b5-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="7f9b5-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="7f9b5-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="7f9b5-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="7f9b5-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="7f9b5-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="7f9b5-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="7f9b5-144">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="7f9b5-144">Report Refresh Date</span></span>
- <span data-ttu-id="7f9b5-145">Mail For Mac (Mail для Mac)</span><span class="sxs-lookup"><span data-stu-id="7f9b5-145">Mail For Mac</span></span>
- <span data-ttu-id="7f9b5-146">"Outlook For Mac" (Outlook для Mac);</span><span class="sxs-lookup"><span data-stu-id="7f9b5-146">Outlook For Mac</span></span>
- <span data-ttu-id="7f9b5-147">"Outlook For Windows" (Outlook для Windows);</span><span class="sxs-lookup"><span data-stu-id="7f9b5-147">Outlook For Windows</span></span>
- <span data-ttu-id="7f9b5-148">"Outlook For Mobile" (Outlook для мобильных устройств);</span><span class="sxs-lookup"><span data-stu-id="7f9b5-148">Outlook For Mobile</span></span>
- <span data-ttu-id="7f9b5-149">"Other For Mobile" (Другое для мобильных устройств);</span><span class="sxs-lookup"><span data-stu-id="7f9b5-149">Other For Mobile</span></span>
- <span data-ttu-id="7f9b5-150">"Outlook For Web" (Outlook для браузера);</span><span class="sxs-lookup"><span data-stu-id="7f9b5-150">Outlook For Web</span></span>
- <span data-ttu-id="7f9b5-151">"POP3 App" (Приложение с поддержкой POP3);</span><span class="sxs-lookup"><span data-stu-id="7f9b5-151">POP3 App</span></span>
- <span data-ttu-id="7f9b5-152">"IMAP4 App" (Приложение с поддержкой IMAP4);</span><span class="sxs-lookup"><span data-stu-id="7f9b5-152">IMAP4 App</span></span>
- <span data-ttu-id="7f9b5-153">SMTP App (Приложение с поддержкой SMTP)</span><span class="sxs-lookup"><span data-stu-id="7f9b5-153">SMTP App</span></span>
- <span data-ttu-id="7f9b5-154">Report Date (Дата отчета)</span><span class="sxs-lookup"><span data-stu-id="7f9b5-154">Report Date</span></span>
- <span data-ttu-id="7f9b5-155">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="7f9b5-155">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="7f9b5-156">JSON</span><span class="sxs-lookup"><span data-stu-id="7f9b5-156">JSON</span></span>

<span data-ttu-id="7f9b5-157">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[емаилаппусажеусеркаунтс](../resources/emailappusageusercounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7f9b5-157">If successful, this method returns a `200 OK` response code and an **[emailAppUsageUserCounts](../resources/emailappusageusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f9b5-158">Пример</span><span class="sxs-lookup"><span data-stu-id="7f9b5-158">Example</span></span>

### <a name="csv"></a><span data-ttu-id="7f9b5-159">CSV</span><span class="sxs-lookup"><span data-stu-id="7f9b5-159">CSV</span></span>

<span data-ttu-id="7f9b5-160">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="7f9b5-160">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="7f9b5-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="7f9b5-161">Request</span></span>

<span data-ttu-id="7f9b5-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7f9b5-162">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7f9b5-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="7f9b5-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7f9b5-164">C#</span><span class="sxs-lookup"><span data-stu-id="7f9b5-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailappusageusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7f9b5-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7f9b5-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailappusageusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7f9b5-166">Цель — C</span><span class="sxs-lookup"><span data-stu-id="7f9b5-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailappusageusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7f9b5-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f9b5-167">Response</span></span>

<span data-ttu-id="7f9b5-168">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7f9b5-168">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="7f9b5-169">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="7f9b5-169">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Mail For Mac,Outlook For Mac,Outlook For Windows,Outlook For Mobile,Other For Mobile,Outlook For Web,POP3 App,IMAP4 App,SMTP App,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="7f9b5-170">JSON</span><span class="sxs-lookup"><span data-stu-id="7f9b5-170">JSON</span></span>

<span data-ttu-id="7f9b5-171">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="7f9b5-171">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="7f9b5-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="7f9b5-172">Request</span></span>

<span data-ttu-id="7f9b5-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7f9b5-173">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7f9b5-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="7f9b5-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7f9b5-175">C#</span><span class="sxs-lookup"><span data-stu-id="7f9b5-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailappusageusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7f9b5-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7f9b5-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailappusageusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7f9b5-177">Цель — C</span><span class="sxs-lookup"><span data-stu-id="7f9b5-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailappusageusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7f9b5-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f9b5-178">Response</span></span>

<span data-ttu-id="7f9b5-179">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7f9b5-179">The following is an example of the response.</span></span>

> <span data-ttu-id="7f9b5-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7f9b5-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAppUsageUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 355

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailAppUsageUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "mailForMac": 0, 
      "outlookForMac": 0, 
      "outlookForWindows": 0, 
      "outlookForMobile": 0, 
      "otherForMobile": 0, 
      "outlookForWeb": 0, 
      "pop3App": 0, 
      "imap4App": 0, 
      "smtpApp": 0, 
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
