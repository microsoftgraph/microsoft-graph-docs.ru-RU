---
title: 'reportRoot: getOffice365GroupsActivityCounts'
description: Узнайте, сколько различных действий было в группах.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 21f311cb86237ecfd35997ff3950ee9bc86f22d6
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867542"
---
# <a name="reportroot-getoffice365groupsactivitycounts"></a><span data-ttu-id="984bc-103">reportRoot: getOffice365GroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="984bc-103">reportRoot: getOffice365GroupsActivityCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="984bc-104">Узнайте, сколько различных действий было в группах.</span><span class="sxs-lookup"><span data-stu-id="984bc-104">Get the number of group activities across group workloads.</span></span>

> <span data-ttu-id="984bc-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="984bc-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="984bc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="984bc-106">Permissions</span></span>

<span data-ttu-id="984bc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="984bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="984bc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="984bc-109">Permission type</span></span>                        | <span data-ttu-id="984bc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="984bc-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="984bc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="984bc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="984bc-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="984bc-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="984bc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="984bc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="984bc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="984bc-114">Not supported.</span></span>                           |
| <span data-ttu-id="984bc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="984bc-115">Application</span></span>                            | <span data-ttu-id="984bc-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="984bc-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="984bc-117">**Примечание**. для делегированных разрешений, чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя, администратору клиента необходимо назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="984bc-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="984bc-118">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="984bc-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="984bc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="984bc-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="984bc-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="984bc-120">Function parameters</span></span>

<span data-ttu-id="984bc-121">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="984bc-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="984bc-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="984bc-122">Parameter</span></span> | <span data-ttu-id="984bc-123">Тип</span><span class="sxs-lookup"><span data-stu-id="984bc-123">Type</span></span>   | <span data-ttu-id="984bc-124">Описание</span><span class="sxs-lookup"><span data-stu-id="984bc-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="984bc-125">period</span><span class="sxs-lookup"><span data-stu-id="984bc-125">period</span></span>    | <span data-ttu-id="984bc-126">string</span><span class="sxs-lookup"><span data-stu-id="984bc-126">string</span></span> | <span data-ttu-id="984bc-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="984bc-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="984bc-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="984bc-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="984bc-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="984bc-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="984bc-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="984bc-130">Required.</span></span> |

<span data-ttu-id="984bc-131">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="984bc-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="984bc-132">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="984bc-132">The default output type is text/csv.</span></span> <span data-ttu-id="984bc-133">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="984bc-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="984bc-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="984bc-134">Request headers</span></span>

| <span data-ttu-id="984bc-135">Имя</span><span class="sxs-lookup"><span data-stu-id="984bc-135">Name</span></span>          | <span data-ttu-id="984bc-136">Описание</span><span class="sxs-lookup"><span data-stu-id="984bc-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="984bc-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="984bc-137">Authorization</span></span> | <span data-ttu-id="984bc-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="984bc-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="984bc-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="984bc-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="984bc-141">CSV</span><span class="sxs-lookup"><span data-stu-id="984bc-141">CSV</span></span>

<span data-ttu-id="984bc-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="984bc-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="984bc-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="984bc-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="984bc-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="984bc-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="984bc-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="984bc-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="984bc-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="984bc-146">Report Refresh Date</span></span>
- <span data-ttu-id="984bc-147">Exchange Emails Received (получено писем Exchange)</span><span class="sxs-lookup"><span data-stu-id="984bc-147">Exchange Emails Received</span></span>
- <span data-ttu-id="984bc-148">Yammer Messages Posted (опубликовано сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="984bc-148">Yammer Messages Posted</span></span>
- <span data-ttu-id="984bc-149">Yammer Messages Read (прочитано сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="984bc-149">Yammer Messages Read</span></span>
- <span data-ttu-id="984bc-150">Yammer Messages Liked (понравилось сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="984bc-150">Yammer Messages Liked</span></span>
- <span data-ttu-id="984bc-151">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="984bc-151">Report Date</span></span>
- <span data-ttu-id="984bc-152">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="984bc-152">Report Period</span></span>

<span data-ttu-id="984bc-153">Следующие столбцы не поддерживаются в Китае Microsoft Graph, предоставляемом компанией 21Vianet:</span><span class="sxs-lookup"><span data-stu-id="984bc-153">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="984bc-154">Yammer Messages Posted (опубликовано сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="984bc-154">Yammer Messages Posted</span></span>
- <span data-ttu-id="984bc-155">Yammer Messages Read (прочитано сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="984bc-155">Yammer Messages Read</span></span>
- <span data-ttu-id="984bc-156">Yammer Messages Liked (понравилось сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="984bc-156">Yammer Messages Liked</span></span>

### <a name="json"></a><span data-ttu-id="984bc-157">JSON</span><span class="sxs-lookup"><span data-stu-id="984bc-157">JSON</span></span>

<span data-ttu-id="984bc-158">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="984bc-158">If successful, this method returns a `200 OK` response code and an **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** object in the response body.</span></span>

<span data-ttu-id="984bc-159">Следующие свойства в объекте **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** не поддерживаются в Китае Microsoft Graph, предоставляемом компанией 21vianet:</span><span class="sxs-lookup"><span data-stu-id="984bc-159">The following properties in **[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="984bc-160">яммермессажеспостед</span><span class="sxs-lookup"><span data-stu-id="984bc-160">yammerMessagesPosted</span></span>
- <span data-ttu-id="984bc-161">яммермессажесреад</span><span class="sxs-lookup"><span data-stu-id="984bc-161">yammerMessagesRead</span></span>
- <span data-ttu-id="984bc-162">яммермессажесликед</span><span class="sxs-lookup"><span data-stu-id="984bc-162">yammerMessagesLiked</span></span>

## <a name="example"></a><span data-ttu-id="984bc-163">Пример</span><span class="sxs-lookup"><span data-stu-id="984bc-163">Example</span></span>

### <a name="csv"></a><span data-ttu-id="984bc-164">CSV</span><span class="sxs-lookup"><span data-stu-id="984bc-164">CSV</span></span>

<span data-ttu-id="984bc-165">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="984bc-165">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="984bc-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="984bc-166">Request</span></span>

<span data-ttu-id="984bc-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="984bc-167">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="984bc-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="984bc-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitycounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="984bc-169">C#</span><span class="sxs-lookup"><span data-stu-id="984bc-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365groupsactivitycounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="984bc-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="984bc-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365groupsactivitycounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="984bc-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="984bc-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365groupsactivitycounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="984bc-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="984bc-172">Response</span></span>

<span data-ttu-id="984bc-173">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="984bc-173">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="984bc-174">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="984bc-174">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Exchange Emails Received,Yammer Messages Posted,Yammer Messages Read,Yammer Messages Liked,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="984bc-175">JSON</span><span class="sxs-lookup"><span data-stu-id="984bc-175">JSON</span></span>

<span data-ttu-id="984bc-176">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="984bc-176">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="984bc-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="984bc-177">Request</span></span>

<span data-ttu-id="984bc-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="984bc-178">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="984bc-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="984bc-179">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitycounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="984bc-180">C#</span><span class="sxs-lookup"><span data-stu-id="984bc-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365groupsactivitycounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="984bc-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="984bc-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365groupsactivitycounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="984bc-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="984bc-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365groupsactivitycounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="984bc-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="984bc-183">Response</span></span>

<span data-ttu-id="984bc-184">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="984bc-184">The following is an example of the response.</span></span>

> <span data-ttu-id="984bc-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="984bc-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365GroupsActivityCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 310

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365GroupsActivityCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "exchangeEmailsReceived": 0, 
      "yammerMessagesPosted": 0, 
      "yammerMessagesRead": 0, 
      "yammerMessagesLiked": 0, 
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
