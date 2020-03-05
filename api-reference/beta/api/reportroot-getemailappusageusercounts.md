---
title: 'reportRoot: getEmailAppUsageUserCounts'
description: Получение числа уникальных пользователей, которые подключались к Exchange Online с помощью приложения электронной почты.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: ba2fae8877744d927b33155ff7076604d8169e32
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454467"
---
# <a name="reportroot-getemailappusageusercounts"></a><span data-ttu-id="3b0d3-103">reportRoot: getEmailAppUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="3b0d3-103">reportRoot: getEmailAppUsageUserCounts</span></span>

<span data-ttu-id="3b0d3-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3b0d3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b0d3-105">Получение числа уникальных пользователей, которые подключались к Exchange Online с помощью приложения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="3b0d3-105">Get the count of unique users that connected to Exchange Online using any email app.</span></span>

> <span data-ttu-id="3b0d3-106">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Центре администрирования Office 365 — использование почтовых приложений](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span><span class="sxs-lookup"><span data-stu-id="3b0d3-106">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="3b0d3-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3b0d3-107">Permissions</span></span>

<span data-ttu-id="3b0d3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b0d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3b0d3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3b0d3-110">Permission type</span></span>                        | <span data-ttu-id="3b0d3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3b0d3-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="3b0d3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3b0d3-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="3b0d3-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3b0d3-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="3b0d3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3b0d3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b0d3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b0d3-115">Not supported.</span></span>                           |
| <span data-ttu-id="3b0d3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3b0d3-116">Application</span></span>                            | <span data-ttu-id="3b0d3-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3b0d3-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="3b0d3-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3b0d3-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="3b0d3-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="3b0d3-119">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="3b0d3-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3b0d3-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="3b0d3-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="3b0d3-121">Function parameters</span></span>

<span data-ttu-id="3b0d3-122">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="3b0d3-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="3b0d3-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="3b0d3-123">Parameter</span></span> | <span data-ttu-id="3b0d3-124">Тип</span><span class="sxs-lookup"><span data-stu-id="3b0d3-124">Type</span></span>   | <span data-ttu-id="3b0d3-125">Описание</span><span class="sxs-lookup"><span data-stu-id="3b0d3-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="3b0d3-126">period</span><span class="sxs-lookup"><span data-stu-id="3b0d3-126">period</span></span>    | <span data-ttu-id="3b0d3-127">string</span><span class="sxs-lookup"><span data-stu-id="3b0d3-127">string</span></span> | <span data-ttu-id="3b0d3-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="3b0d3-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="3b0d3-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="3b0d3-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="3b0d3-130">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="3b0d3-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="3b0d3-131">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3b0d3-131">Required.</span></span> |

<span data-ttu-id="3b0d3-132">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="3b0d3-132">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="3b0d3-133">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="3b0d3-133">The default output type is text/csv.</span></span> <span data-ttu-id="3b0d3-134">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="3b0d3-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3b0d3-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3b0d3-135">Request headers</span></span>

| <span data-ttu-id="3b0d3-136">Имя</span><span class="sxs-lookup"><span data-stu-id="3b0d3-136">Name</span></span>          | <span data-ttu-id="3b0d3-137">Описание</span><span class="sxs-lookup"><span data-stu-id="3b0d3-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="3b0d3-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3b0d3-138">Authorization</span></span> | <span data-ttu-id="3b0d3-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3b0d3-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="3b0d3-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b0d3-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="3b0d3-142">CSV</span><span class="sxs-lookup"><span data-stu-id="3b0d3-142">CSV</span></span>

<span data-ttu-id="3b0d3-143">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="3b0d3-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="3b0d3-144">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="3b0d3-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="3b0d3-145">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="3b0d3-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="3b0d3-146">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="3b0d3-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="3b0d3-147">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="3b0d3-147">Report Refresh Date</span></span>
- <span data-ttu-id="3b0d3-148">Mail For Mac (Mail для Mac)</span><span class="sxs-lookup"><span data-stu-id="3b0d3-148">Mail For Mac</span></span>
- <span data-ttu-id="3b0d3-149">"Outlook For Mac" (Outlook для Mac);</span><span class="sxs-lookup"><span data-stu-id="3b0d3-149">Outlook For Mac</span></span>
- <span data-ttu-id="3b0d3-150">"Outlook For Windows" (Outlook для Windows);</span><span class="sxs-lookup"><span data-stu-id="3b0d3-150">Outlook For Windows</span></span>
- <span data-ttu-id="3b0d3-151">"Outlook For Mobile" (Outlook для мобильных устройств);</span><span class="sxs-lookup"><span data-stu-id="3b0d3-151">Outlook For Mobile</span></span>
- <span data-ttu-id="3b0d3-152">"Other For Mobile" (Другое для мобильных устройств);</span><span class="sxs-lookup"><span data-stu-id="3b0d3-152">Other For Mobile</span></span>
- <span data-ttu-id="3b0d3-153">"Outlook For Web" (Outlook для браузера);</span><span class="sxs-lookup"><span data-stu-id="3b0d3-153">Outlook For Web</span></span>
- <span data-ttu-id="3b0d3-154">"POP3 App" (Приложение с поддержкой POP3);</span><span class="sxs-lookup"><span data-stu-id="3b0d3-154">POP3 App</span></span>
- <span data-ttu-id="3b0d3-155">"IMAP4 App" (Приложение с поддержкой IMAP4);</span><span class="sxs-lookup"><span data-stu-id="3b0d3-155">IMAP4 App</span></span>
- <span data-ttu-id="3b0d3-156">SMTP App (Приложение с поддержкой SMTP)</span><span class="sxs-lookup"><span data-stu-id="3b0d3-156">SMTP App</span></span>
- <span data-ttu-id="3b0d3-157">Report Date (Дата отчета)</span><span class="sxs-lookup"><span data-stu-id="3b0d3-157">Report Date</span></span>
- <span data-ttu-id="3b0d3-158">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="3b0d3-158">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="3b0d3-159">JSON</span><span class="sxs-lookup"><span data-stu-id="3b0d3-159">JSON</span></span>

<span data-ttu-id="3b0d3-160">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[емаилаппусажеусеркаунтс](../resources/emailappusageusercounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3b0d3-160">If successful, this method returns a `200 OK` response code and an **[emailAppUsageUserCounts](../resources/emailappusageusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b0d3-161">Пример</span><span class="sxs-lookup"><span data-stu-id="3b0d3-161">Example</span></span>

### <a name="csv"></a><span data-ttu-id="3b0d3-162">CSV</span><span class="sxs-lookup"><span data-stu-id="3b0d3-162">CSV</span></span>

<span data-ttu-id="3b0d3-163">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="3b0d3-163">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="3b0d3-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="3b0d3-164">Request</span></span>

<span data-ttu-id="3b0d3-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3b0d3-165">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3b0d3-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="3b0d3-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageUserCounts(period='D7')?$format=text/csv
```
# <a name="c"></a>[<span data-ttu-id="3b0d3-167">C#</span><span class="sxs-lookup"><span data-stu-id="3b0d3-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailappusageusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3b0d3-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3b0d3-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailappusageusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3b0d3-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3b0d3-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailappusageusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3b0d3-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b0d3-170">Response</span></span>

<span data-ttu-id="3b0d3-171">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3b0d3-171">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="3b0d3-172">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="3b0d3-172">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="3b0d3-173">JSON</span><span class="sxs-lookup"><span data-stu-id="3b0d3-173">JSON</span></span>

<span data-ttu-id="3b0d3-174">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="3b0d3-174">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="3b0d3-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="3b0d3-175">Request</span></span>

<span data-ttu-id="3b0d3-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3b0d3-176">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3b0d3-177">HTTP</span><span class="sxs-lookup"><span data-stu-id="3b0d3-177">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageUserCounts(period='D7')?$format=application/json
```
# <a name="c"></a>[<span data-ttu-id="3b0d3-178">C#</span><span class="sxs-lookup"><span data-stu-id="3b0d3-178">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailappusageusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3b0d3-179">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3b0d3-179">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailappusageusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3b0d3-180">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3b0d3-180">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailappusageusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3b0d3-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b0d3-181">Response</span></span>

<span data-ttu-id="3b0d3-182">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3b0d3-182">The following is an example of the response.</span></span>

> <span data-ttu-id="3b0d3-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3b0d3-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
