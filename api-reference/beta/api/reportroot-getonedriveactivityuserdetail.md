---
title: 'reportRoot: getOneDriveActivityUserDetail'
description: Получите сведения о действиях в OneDrive с разбивкой по пользователям.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 4575847ccd0a1a607f74b7b7dad1cc0b7334b14a
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869103"
---
# <a name="reportroot-getonedriveactivityuserdetail"></a><span data-ttu-id="94319-103">reportRoot: getOneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="94319-103">reportRoot: getOneDriveActivityUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94319-104">Получите сведения о действиях в OneDrive с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="94319-104">Get details about OneDrive activity by user.</span></span>

> <span data-ttu-id="94319-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия в OneDrive для бизнеса](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span><span class="sxs-lookup"><span data-stu-id="94319-105">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="permissions"></a><span data-ttu-id="94319-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="94319-106">Permissions</span></span>

<span data-ttu-id="94319-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94319-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="94319-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="94319-109">Permission type</span></span>                        | <span data-ttu-id="94319-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="94319-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="94319-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="94319-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="94319-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="94319-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="94319-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="94319-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94319-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94319-114">Not supported.</span></span>                           |
| <span data-ttu-id="94319-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="94319-115">Application</span></span>                            | <span data-ttu-id="94319-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="94319-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="94319-117">**Примечание**. для делегированных разрешений, чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя, администратору клиента необходимо назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="94319-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="94319-118">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="94319-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="94319-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="94319-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveActivityUserDetail(period='{period_value}')
GET /reports/getOneDriveActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="94319-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="94319-120">Function parameters</span></span>

<span data-ttu-id="94319-121">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="94319-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="94319-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="94319-122">Parameter</span></span> | <span data-ttu-id="94319-123">Тип</span><span class="sxs-lookup"><span data-stu-id="94319-123">Type</span></span>   | <span data-ttu-id="94319-124">Описание</span><span class="sxs-lookup"><span data-stu-id="94319-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="94319-125">period</span><span class="sxs-lookup"><span data-stu-id="94319-125">period</span></span>    | <span data-ttu-id="94319-126">string</span><span class="sxs-lookup"><span data-stu-id="94319-126">string</span></span> | <span data-ttu-id="94319-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="94319-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="94319-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="94319-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="94319-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="94319-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="94319-130">date</span><span class="sxs-lookup"><span data-stu-id="94319-130">date</span></span>      | <span data-ttu-id="94319-131">Date</span><span class="sxs-lookup"><span data-stu-id="94319-131">Date</span></span>   | <span data-ttu-id="94319-132">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="94319-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="94319-133">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="94319-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="94319-134">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="94319-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="94319-135">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="94319-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="94319-136">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="94319-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="94319-137">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="94319-137">The default output type is text/csv.</span></span> <span data-ttu-id="94319-138">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="94319-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="94319-139">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="94319-139">Request headers</span></span>

| <span data-ttu-id="94319-140">Имя</span><span class="sxs-lookup"><span data-stu-id="94319-140">Name</span></span>          | <span data-ttu-id="94319-141">Описание</span><span class="sxs-lookup"><span data-stu-id="94319-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="94319-142">Авторизация</span><span class="sxs-lookup"><span data-stu-id="94319-142">Authorization</span></span> | <span data-ttu-id="94319-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="94319-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="94319-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="94319-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="94319-146">CSV</span><span class="sxs-lookup"><span data-stu-id="94319-146">CSV</span></span>

<span data-ttu-id="94319-147">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="94319-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="94319-148">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="94319-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="94319-149">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="94319-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="94319-150">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="94319-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="94319-151">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="94319-151">Report Refresh Date</span></span>
- <span data-ttu-id="94319-152">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="94319-152">User Principal Name</span></span>
- <span data-ttu-id="94319-153">Is Deleted (Удален);</span><span class="sxs-lookup"><span data-stu-id="94319-153">Is Deleted</span></span>
- <span data-ttu-id="94319-154">"Deleted Date" (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="94319-154">Deleted Date</span></span>
- <span data-ttu-id="94319-155">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="94319-155">Last Activity Date</span></span>
- <span data-ttu-id="94319-156">"Viewed Or Edited File Count" (Количество просмотренных или измененных файлов);</span><span class="sxs-lookup"><span data-stu-id="94319-156">Viewed Or Edited File Count</span></span>
- <span data-ttu-id="94319-157">"Synced File Count" (Количество синхронизированных файлов);</span><span class="sxs-lookup"><span data-stu-id="94319-157">Synced File Count</span></span>
- <span data-ttu-id="94319-158">"Shared Internally File Count" (Количество файлов, к которым предоставлен доступ внутренним пользователям);</span><span class="sxs-lookup"><span data-stu-id="94319-158">Shared Internally File Count</span></span>
- <span data-ttu-id="94319-159">"Shared Externally File Count" (Количество файлов, к которым предоставлен доступ внешним пользователям);</span><span class="sxs-lookup"><span data-stu-id="94319-159">Shared Externally File Count</span></span>
- <span data-ttu-id="94319-160">Assigned Products (назначенные продукты)</span><span class="sxs-lookup"><span data-stu-id="94319-160">Assigned Products</span></span>
- <span data-ttu-id="94319-161">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="94319-161">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="94319-162">JSON</span><span class="sxs-lookup"><span data-stu-id="94319-162">JSON</span></span>

<span data-ttu-id="94319-163">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[онедривеактивитюсердетаил](../resources/onedriveactivityuserdetail.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="94319-163">If successful, this method returns a `200 OK` response code and a **[oneDriveActivityUserDetail](../resources/onedriveactivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="94319-164">Размер страницы по умолчанию для этого запроса составляет 200 элементов.</span><span class="sxs-lookup"><span data-stu-id="94319-164">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="94319-165">Пример</span><span class="sxs-lookup"><span data-stu-id="94319-165">Example</span></span>

### <a name="csv"></a><span data-ttu-id="94319-166">CSV</span><span class="sxs-lookup"><span data-stu-id="94319-166">CSV</span></span>

<span data-ttu-id="94319-167">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="94319-167">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="94319-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="94319-168">Request</span></span>

<span data-ttu-id="94319-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="94319-169">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="94319-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="94319-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveactivityuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOneDriveActivityUserDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="94319-171">C#</span><span class="sxs-lookup"><span data-stu-id="94319-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveactivityuserdetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="94319-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94319-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveactivityuserdetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="94319-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="94319-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveactivityuserdetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="94319-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="94319-174">Response</span></span>

<span data-ttu-id="94319-175">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="94319-175">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="94319-176">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="94319-176">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="94319-177">JSON</span><span class="sxs-lookup"><span data-stu-id="94319-177">JSON</span></span>

<span data-ttu-id="94319-178">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="94319-178">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="94319-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="94319-179">Request</span></span>

<span data-ttu-id="94319-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="94319-180">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="94319-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="94319-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveactivityuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOneDriveActivityUserDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="94319-182">C#</span><span class="sxs-lookup"><span data-stu-id="94319-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveactivityuserdetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="94319-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94319-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveactivityuserdetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="94319-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="94319-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveactivityuserdetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="94319-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="94319-185">Response</span></span>

<span data-ttu-id="94319-186">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="94319-186">The following is an example of the response.</span></span>

> <span data-ttu-id="94319-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="94319-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
