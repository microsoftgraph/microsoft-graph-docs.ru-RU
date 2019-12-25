---
title: 'reportRoot: getTeamsDeviceUsageUserDetail'
description: Получение сведений об использовании устройств Microsoft Teams по каждому пользователю.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: c3758796e5fd5fa2997019e137211b787d5f005b
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868935"
---
# <a name="reportroot-getteamsdeviceusageuserdetail"></a><span data-ttu-id="49e5c-103">reportRoot: getTeamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="49e5c-103">reportRoot: getTeamsDeviceUsageUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49e5c-104">Получение сведений об использовании устройств Microsoft Teams по каждому пользователю.</span><span class="sxs-lookup"><span data-stu-id="49e5c-104">Get details about Microsoft Teams device usage by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="49e5c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="49e5c-105">Permissions</span></span>

<span data-ttu-id="49e5c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49e5c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="49e5c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49e5c-108">Permission type</span></span>                        | <span data-ttu-id="49e5c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="49e5c-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="49e5c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49e5c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="49e5c-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="49e5c-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="49e5c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49e5c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49e5c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49e5c-113">Not supported.</span></span>                           |
| <span data-ttu-id="49e5c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="49e5c-114">Application</span></span>                            | <span data-ttu-id="49e5c-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="49e5c-115">Reports.Read.All</span></span>                         |

<span data-ttu-id="49e5c-116">**Примечание**. для делегированных разрешений, чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя, администратору клиента необходимо назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="49e5c-116">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="49e5c-117">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="49e5c-117">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="49e5c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49e5c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageUserDetail(period='D7')
GET /reports/getTeamsDeviceUsageUserDetail(date=2017-09-01)
```

## <a name="function-parameters"></a><span data-ttu-id="49e5c-119">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="49e5c-119">Function parameters</span></span>

<span data-ttu-id="49e5c-120">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="49e5c-120">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="49e5c-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="49e5c-121">Parameter</span></span> | <span data-ttu-id="49e5c-122">Тип</span><span class="sxs-lookup"><span data-stu-id="49e5c-122">Type</span></span>   | <span data-ttu-id="49e5c-123">Описание</span><span class="sxs-lookup"><span data-stu-id="49e5c-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="49e5c-124">period</span><span class="sxs-lookup"><span data-stu-id="49e5c-124">period</span></span>    | <span data-ttu-id="49e5c-125">string</span><span class="sxs-lookup"><span data-stu-id="49e5c-125">string</span></span> | <span data-ttu-id="49e5c-126">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="49e5c-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="49e5c-127">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="49e5c-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="49e5c-128">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="49e5c-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="49e5c-129">date</span><span class="sxs-lookup"><span data-stu-id="49e5c-129">date</span></span>      | <span data-ttu-id="49e5c-130">Date</span><span class="sxs-lookup"><span data-stu-id="49e5c-130">Date</span></span>   | <span data-ttu-id="49e5c-131">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="49e5c-131">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="49e5c-132">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="49e5c-132">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="49e5c-133">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="49e5c-133">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="49e5c-134">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="49e5c-134">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="49e5c-135">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="49e5c-135">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="49e5c-136">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="49e5c-136">The default output type is text/csv.</span></span> <span data-ttu-id="49e5c-137">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="49e5c-137">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="49e5c-138">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="49e5c-138">Request headers</span></span>

| <span data-ttu-id="49e5c-139">Имя</span><span class="sxs-lookup"><span data-stu-id="49e5c-139">Name</span></span>          | <span data-ttu-id="49e5c-140">Описание</span><span class="sxs-lookup"><span data-stu-id="49e5c-140">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="49e5c-141">Авторизация</span><span class="sxs-lookup"><span data-stu-id="49e5c-141">Authorization</span></span> | <span data-ttu-id="49e5c-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="49e5c-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="49e5c-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="49e5c-144">Response</span></span>

### <a name="csv"></a><span data-ttu-id="49e5c-145">CSV</span><span class="sxs-lookup"><span data-stu-id="49e5c-145">CSV</span></span>

<span data-ttu-id="49e5c-146">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="49e5c-146">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="49e5c-147">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="49e5c-147">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="49e5c-148">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="49e5c-148">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="49e5c-149">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="49e5c-149">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="49e5c-150">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="49e5c-150">Report Refresh Date</span></span>
- <span data-ttu-id="49e5c-151">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="49e5c-151">User Principal Name</span></span>
- <span data-ttu-id="49e5c-152">Last Activity Date (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="49e5c-152">Last Activity Date</span></span>
- <span data-ttu-id="49e5c-153">Is Deleted (Удален);</span><span class="sxs-lookup"><span data-stu-id="49e5c-153">Is Deleted</span></span>
- <span data-ttu-id="49e5c-154">Deleted Date (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="49e5c-154">Deleted Date</span></span>
- <span data-ttu-id="49e5c-155">Used Web (использовал браузер);</span><span class="sxs-lookup"><span data-stu-id="49e5c-155">Used Web</span></span>
- <span data-ttu-id="49e5c-156">Used Windows Phone (использовал телефон с Windows);</span><span class="sxs-lookup"><span data-stu-id="49e5c-156">Used Windows Phone</span></span>
- <span data-ttu-id="49e5c-157">Used iOS (использовал iOS);</span><span class="sxs-lookup"><span data-stu-id="49e5c-157">Used iOS</span></span>
- <span data-ttu-id="49e5c-158">Used Mac (использовал Mac);</span><span class="sxs-lookup"><span data-stu-id="49e5c-158">Used Mac</span></span>
- <span data-ttu-id="49e5c-159">Used Android Phone (использовал телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="49e5c-159">Used Android Phone</span></span>
- <span data-ttu-id="49e5c-160">Used Windows (использовал Windows);</span><span class="sxs-lookup"><span data-stu-id="49e5c-160">Used Windows</span></span>
- <span data-ttu-id="49e5c-161">Report Period (отчетный период).</span><span class="sxs-lookup"><span data-stu-id="49e5c-161">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="49e5c-162">JSON</span><span class="sxs-lookup"><span data-stu-id="49e5c-162">JSON</span></span>

<span data-ttu-id="49e5c-163">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[теамсдевицеусажеусердетаил](../resources/teamsdeviceusageuserdetail.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="49e5c-163">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="49e5c-164">Размер страницы по умолчанию для этого запроса составляет 2000 элементов.</span><span class="sxs-lookup"><span data-stu-id="49e5c-164">The default page size for this request is 2000 items.</span></span>

## <a name="example"></a><span data-ttu-id="49e5c-165">Пример</span><span class="sxs-lookup"><span data-stu-id="49e5c-165">Example</span></span>

### <a name="csv"></a><span data-ttu-id="49e5c-166">CSV</span><span class="sxs-lookup"><span data-stu-id="49e5c-166">CSV</span></span>

<span data-ttu-id="49e5c-167">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="49e5c-167">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="49e5c-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="49e5c-168">Request</span></span>

<span data-ttu-id="49e5c-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="49e5c-169">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="49e5c-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="49e5c-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="49e5c-171">C#</span><span class="sxs-lookup"><span data-stu-id="49e5c-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsdeviceusageuserdetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="49e5c-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49e5c-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsdeviceusageuserdetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="49e5c-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="49e5c-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsdeviceusageuserdetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="49e5c-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="49e5c-174">Response</span></span>

<span data-ttu-id="49e5c-175">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="49e5c-175">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="49e5c-176">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="49e5c-176">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Is Deleted,Deleted Date,Used Web,Used Windows Phone,Used iOS,Used Mac,Used Android Phone,Used Windows,Report Period
```

### <a name="json"></a><span data-ttu-id="49e5c-177">JSON</span><span class="sxs-lookup"><span data-stu-id="49e5c-177">JSON</span></span>

<span data-ttu-id="49e5c-178">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="49e5c-178">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="49e5c-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="49e5c-179">Request</span></span>

<span data-ttu-id="49e5c-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="49e5c-180">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="49e5c-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="49e5c-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="49e5c-182">C#</span><span class="sxs-lookup"><span data-stu-id="49e5c-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsdeviceusageuserdetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="49e5c-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49e5c-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsdeviceusageuserdetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="49e5c-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="49e5c-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsdeviceusageuserdetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="49e5c-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="49e5c-185">Response</span></span>

<span data-ttu-id="49e5c-186">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="49e5c-186">The following is an example of the response.</span></span>

> <span data-ttu-id="49e5c-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="49e5c-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 374

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsDeviceUsageUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "lastActivityDate": "2017-09-01", 
      "isDeleted": false, 
      "deletedDate": null, 
      "usedWeb": false, 
      "usedWindowsPhone": false, 
      "usediOS": true, 
      "usedMac": false, 
      "usedAndroidPhone": false, 
      "usedWindows": true, 
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
