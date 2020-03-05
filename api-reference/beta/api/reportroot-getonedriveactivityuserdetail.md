---
title: 'reportRoot: getOneDriveActivityUserDetail'
description: Получите сведения о действиях в OneDrive с разбивкой по пользователям.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: f8e9bea1d08ca2a14658b60127a50b631a9eb404
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454320"
---
# <a name="reportroot-getonedriveactivityuserdetail"></a><span data-ttu-id="51745-103">reportRoot: getOneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="51745-103">reportRoot: getOneDriveActivityUserDetail</span></span>

<span data-ttu-id="51745-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="51745-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51745-105">Получите сведения о действиях в OneDrive с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="51745-105">Get details about OneDrive activity by user.</span></span>

> <span data-ttu-id="51745-106">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия в OneDrive для бизнеса](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span><span class="sxs-lookup"><span data-stu-id="51745-106">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="permissions"></a><span data-ttu-id="51745-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="51745-107">Permissions</span></span>

<span data-ttu-id="51745-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51745-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="51745-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51745-110">Permission type</span></span>                        | <span data-ttu-id="51745-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="51745-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="51745-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51745-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="51745-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="51745-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="51745-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51745-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51745-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51745-115">Not supported.</span></span>                           |
| <span data-ttu-id="51745-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="51745-116">Application</span></span>                            | <span data-ttu-id="51745-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="51745-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="51745-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="51745-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="51745-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="51745-119">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="51745-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51745-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveActivityUserDetail(period='{period_value}')
GET /reports/getOneDriveActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="51745-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="51745-121">Function parameters</span></span>

<span data-ttu-id="51745-122">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="51745-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="51745-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="51745-123">Parameter</span></span> | <span data-ttu-id="51745-124">Тип</span><span class="sxs-lookup"><span data-stu-id="51745-124">Type</span></span>   | <span data-ttu-id="51745-125">Описание</span><span class="sxs-lookup"><span data-stu-id="51745-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="51745-126">period</span><span class="sxs-lookup"><span data-stu-id="51745-126">period</span></span>    | <span data-ttu-id="51745-127">string</span><span class="sxs-lookup"><span data-stu-id="51745-127">string</span></span> | <span data-ttu-id="51745-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="51745-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="51745-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="51745-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="51745-130">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="51745-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="51745-131">date</span><span class="sxs-lookup"><span data-stu-id="51745-131">date</span></span>      | <span data-ttu-id="51745-132">Date</span><span class="sxs-lookup"><span data-stu-id="51745-132">Date</span></span>   | <span data-ttu-id="51745-133">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="51745-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="51745-134">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="51745-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="51745-135">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="51745-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="51745-136">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="51745-136">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="51745-137">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="51745-137">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="51745-138">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="51745-138">The default output type is text/csv.</span></span> <span data-ttu-id="51745-139">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="51745-139">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="51745-140">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="51745-140">Request headers</span></span>

| <span data-ttu-id="51745-141">Имя</span><span class="sxs-lookup"><span data-stu-id="51745-141">Name</span></span>          | <span data-ttu-id="51745-142">Описание</span><span class="sxs-lookup"><span data-stu-id="51745-142">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="51745-143">Авторизация</span><span class="sxs-lookup"><span data-stu-id="51745-143">Authorization</span></span> | <span data-ttu-id="51745-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="51745-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="51745-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="51745-146">Response</span></span>

### <a name="csv"></a><span data-ttu-id="51745-147">CSV</span><span class="sxs-lookup"><span data-stu-id="51745-147">CSV</span></span>

<span data-ttu-id="51745-148">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="51745-148">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="51745-149">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="51745-149">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="51745-150">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="51745-150">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="51745-151">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="51745-151">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="51745-152">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="51745-152">Report Refresh Date</span></span>
- <span data-ttu-id="51745-153">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="51745-153">User Principal Name</span></span>
- <span data-ttu-id="51745-154">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="51745-154">Is Deleted</span></span>
- <span data-ttu-id="51745-155">"Deleted Date" (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="51745-155">Deleted Date</span></span>
- <span data-ttu-id="51745-156">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="51745-156">Last Activity Date</span></span>
- <span data-ttu-id="51745-157">"Viewed Or Edited File Count" (Количество просмотренных или измененных файлов);</span><span class="sxs-lookup"><span data-stu-id="51745-157">Viewed Or Edited File Count</span></span>
- <span data-ttu-id="51745-158">"Synced File Count" (Количество синхронизированных файлов);</span><span class="sxs-lookup"><span data-stu-id="51745-158">Synced File Count</span></span>
- <span data-ttu-id="51745-159">"Shared Internally File Count" (Количество файлов, к которым предоставлен доступ внутренним пользователям);</span><span class="sxs-lookup"><span data-stu-id="51745-159">Shared Internally File Count</span></span>
- <span data-ttu-id="51745-160">"Shared Externally File Count" (Количество файлов, к которым предоставлен доступ внешним пользователям);</span><span class="sxs-lookup"><span data-stu-id="51745-160">Shared Externally File Count</span></span>
- <span data-ttu-id="51745-161">Assigned Products (назначенные продукты)</span><span class="sxs-lookup"><span data-stu-id="51745-161">Assigned Products</span></span>
- <span data-ttu-id="51745-162">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="51745-162">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="51745-163">JSON</span><span class="sxs-lookup"><span data-stu-id="51745-163">JSON</span></span>

<span data-ttu-id="51745-164">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[онедривеактивитюсердетаил](../resources/onedriveactivityuserdetail.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="51745-164">If successful, this method returns a `200 OK` response code and a **[oneDriveActivityUserDetail](../resources/onedriveactivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="51745-165">Размер страницы по умолчанию для этого запроса составляет 200 элементов.</span><span class="sxs-lookup"><span data-stu-id="51745-165">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="51745-166">Пример</span><span class="sxs-lookup"><span data-stu-id="51745-166">Example</span></span>

### <a name="csv"></a><span data-ttu-id="51745-167">CSV</span><span class="sxs-lookup"><span data-stu-id="51745-167">CSV</span></span>

<span data-ttu-id="51745-168">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="51745-168">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="51745-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="51745-169">Request</span></span>

<span data-ttu-id="51745-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51745-170">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="51745-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="51745-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveactivityuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOneDriveActivityUserDetail(period='D7')?$format=text/csv
```
# <a name="c"></a>[<span data-ttu-id="51745-172">C#</span><span class="sxs-lookup"><span data-stu-id="51745-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveactivityuserdetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="51745-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="51745-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveactivityuserdetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="51745-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="51745-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveactivityuserdetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="51745-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="51745-175">Response</span></span>

<span data-ttu-id="51745-176">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="51745-176">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="51745-177">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="51745-177">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Viewed Or Edited File Count,Synced File Count,Shared Internally File Count,Shared Externally File Count,Assigned Products,Report Period
```

### <a name="json"></a><span data-ttu-id="51745-178">JSON</span><span class="sxs-lookup"><span data-stu-id="51745-178">JSON</span></span>

<span data-ttu-id="51745-179">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="51745-179">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="51745-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="51745-180">Request</span></span>

<span data-ttu-id="51745-181">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51745-181">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="51745-182">HTTP</span><span class="sxs-lookup"><span data-stu-id="51745-182">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveactivityuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOneDriveActivityUserDetail(period='D7')?$format=application/json
```
# <a name="c"></a>[<span data-ttu-id="51745-183">C#</span><span class="sxs-lookup"><span data-stu-id="51745-183">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveactivityuserdetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="51745-184">JavaScript</span><span class="sxs-lookup"><span data-stu-id="51745-184">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveactivityuserdetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="51745-185">Objective-C</span><span class="sxs-lookup"><span data-stu-id="51745-185">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveactivityuserdetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="51745-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="51745-186">Response</span></span>

<span data-ttu-id="51745-187">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="51745-187">The following is an example of the response.</span></span>

> <span data-ttu-id="51745-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="51745-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oneDriveActivityUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 450

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.oneDriveActivityUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "isDeleted": false, 
      "deletedDate": null, 
      "lastActivityDate": "2017-09-01", 
      "viewedOrEditedFileCount": 1, 
      "syncedFileCount": 0, 
      "sharedInternallyFileCount": 0, 
      "sharedExternallyFileCount": 0, 
      "assignedProducts": [
        "OFFICE 365 ENTERPRISE E5"
      ], 
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
