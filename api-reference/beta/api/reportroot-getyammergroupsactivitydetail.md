---
title: 'reportRoot: getYammerGroupsActivityDetail'
description: Получите сведения об активности в группах Yammer.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 0f24445dc38edbdab501ca0212fd1ee1c4575e0f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453956"
---
# <a name="reportroot-getyammergroupsactivitydetail"></a><span data-ttu-id="47fb1-103">reportRoot: getYammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="47fb1-103">reportRoot: getYammerGroupsActivityDetail</span></span>

<span data-ttu-id="47fb1-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="47fb1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47fb1-105">Получите сведения об активности в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="47fb1-105">Get details about Yammer groups activity by group.</span></span>

> <span data-ttu-id="47fb1-106">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span><span class="sxs-lookup"><span data-stu-id="47fb1-106">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="47fb1-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="47fb1-107">Permissions</span></span>

<span data-ttu-id="47fb1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47fb1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="47fb1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47fb1-110">Permission type</span></span>                        | <span data-ttu-id="47fb1-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="47fb1-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="47fb1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47fb1-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="47fb1-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="47fb1-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="47fb1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47fb1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47fb1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47fb1-115">Not supported.</span></span>                           |
| <span data-ttu-id="47fb1-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="47fb1-116">Application</span></span>                            | <span data-ttu-id="47fb1-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="47fb1-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="47fb1-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="47fb1-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="47fb1-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="47fb1-119">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="47fb1-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47fb1-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityDetail(period='{period_value}')
GET /reports/getYammerGroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="47fb1-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="47fb1-121">Function parameters</span></span>

<span data-ttu-id="47fb1-122">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="47fb1-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="47fb1-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="47fb1-123">Parameter</span></span> | <span data-ttu-id="47fb1-124">Тип</span><span class="sxs-lookup"><span data-stu-id="47fb1-124">Type</span></span>   | <span data-ttu-id="47fb1-125">Описание</span><span class="sxs-lookup"><span data-stu-id="47fb1-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="47fb1-126">period</span><span class="sxs-lookup"><span data-stu-id="47fb1-126">period</span></span>    | <span data-ttu-id="47fb1-127">string</span><span class="sxs-lookup"><span data-stu-id="47fb1-127">string</span></span> | <span data-ttu-id="47fb1-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="47fb1-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="47fb1-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="47fb1-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="47fb1-130">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="47fb1-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="47fb1-131">date</span><span class="sxs-lookup"><span data-stu-id="47fb1-131">date</span></span>      | <span data-ttu-id="47fb1-132">Date</span><span class="sxs-lookup"><span data-stu-id="47fb1-132">Date</span></span>   | <span data-ttu-id="47fb1-133">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="47fb1-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="47fb1-134">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="47fb1-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="47fb1-135">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="47fb1-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="47fb1-136">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="47fb1-136">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="47fb1-137">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="47fb1-137">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="47fb1-138">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="47fb1-138">The default output type is text/csv.</span></span> <span data-ttu-id="47fb1-139">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="47fb1-139">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="47fb1-140">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="47fb1-140">Request headers</span></span>

| <span data-ttu-id="47fb1-141">Имя</span><span class="sxs-lookup"><span data-stu-id="47fb1-141">Name</span></span>          | <span data-ttu-id="47fb1-142">Описание</span><span class="sxs-lookup"><span data-stu-id="47fb1-142">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="47fb1-143">Авторизация</span><span class="sxs-lookup"><span data-stu-id="47fb1-143">Authorization</span></span> | <span data-ttu-id="47fb1-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="47fb1-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="47fb1-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="47fb1-146">Response</span></span>

### <a name="csv"></a><span data-ttu-id="47fb1-147">CSV</span><span class="sxs-lookup"><span data-stu-id="47fb1-147">CSV</span></span>

<span data-ttu-id="47fb1-148">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="47fb1-148">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="47fb1-149">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="47fb1-149">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="47fb1-150">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="47fb1-150">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="47fb1-151">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="47fb1-151">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="47fb1-152">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="47fb1-152">Report Refresh Date</span></span>
- <span data-ttu-id="47fb1-153">Group Display Name (отображаемое имя группы)</span><span class="sxs-lookup"><span data-stu-id="47fb1-153">Group Display Name</span></span>
- <span data-ttu-id="47fb1-154">Is Deleted (удален)</span><span class="sxs-lookup"><span data-stu-id="47fb1-154">Is Deleted</span></span>
- <span data-ttu-id="47fb1-155">Owner Principal Name (имя участника-владельца)</span><span class="sxs-lookup"><span data-stu-id="47fb1-155">Owner Principal Name</span></span>
- <span data-ttu-id="47fb1-156">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="47fb1-156">Last Activity Date</span></span>
- <span data-ttu-id="47fb1-157">Group Type (тип группы)</span><span class="sxs-lookup"><span data-stu-id="47fb1-157">Group Type</span></span>
- <span data-ttu-id="47fb1-158">Office 365 Connected (подключены к Office 365)</span><span class="sxs-lookup"><span data-stu-id="47fb1-158">Office 365 Connected</span></span>
- <span data-ttu-id="47fb1-159">Member Count (количество участников)</span><span class="sxs-lookup"><span data-stu-id="47fb1-159">Member Count</span></span>
- <span data-ttu-id="47fb1-160">Posted Count (количество опубликованных сообщений)</span><span class="sxs-lookup"><span data-stu-id="47fb1-160">Posted Count</span></span>
- <span data-ttu-id="47fb1-161">Read Count (количество прочитанных сообщений)</span><span class="sxs-lookup"><span data-stu-id="47fb1-161">Read Count</span></span>
- <span data-ttu-id="47fb1-162">Liked Count (количество понравившихся сообщений)</span><span class="sxs-lookup"><span data-stu-id="47fb1-162">Liked Count</span></span>
- <span data-ttu-id="47fb1-163">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="47fb1-163">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="47fb1-164">JSON</span><span class="sxs-lookup"><span data-stu-id="47fb1-164">JSON</span></span>

<span data-ttu-id="47fb1-165">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[яммерграупсактивитидетаил](../resources/yammergroupsactivitydetail.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="47fb1-165">If successful, this method returns a `200 OK` response code and a **[yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md)** object in the response body.</span></span>

<span data-ttu-id="47fb1-166">Размер страницы по умолчанию для этого запроса составляет 200 элементов.</span><span class="sxs-lookup"><span data-stu-id="47fb1-166">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="47fb1-167">Пример</span><span class="sxs-lookup"><span data-stu-id="47fb1-167">Example</span></span>

### <a name="csv"></a><span data-ttu-id="47fb1-168">CSV</span><span class="sxs-lookup"><span data-stu-id="47fb1-168">CSV</span></span>

<span data-ttu-id="47fb1-169">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="47fb1-169">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="47fb1-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="47fb1-170">Request</span></span>

<span data-ttu-id="47fb1-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47fb1-171">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="47fb1-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="47fb1-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitydetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityDetail(period='D7')?$format=text/csv
```
# <a name="c"></a>[<span data-ttu-id="47fb1-173">C#</span><span class="sxs-lookup"><span data-stu-id="47fb1-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammergroupsactivitydetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="47fb1-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="47fb1-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammergroupsactivitydetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="47fb1-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="47fb1-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammergroupsactivitydetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="47fb1-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="47fb1-176">Response</span></span>

<span data-ttu-id="47fb1-177">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="47fb1-177">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="47fb1-178">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="47fb1-178">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Group Display Name,Is Deleted,Owner Principal Name,Last Activity Date,Group Type,Office 365 Connected,Member Count,Posted Count,Read Count,Liked Count,Report Period
```

### <a name="json"></a><span data-ttu-id="47fb1-179">JSON</span><span class="sxs-lookup"><span data-stu-id="47fb1-179">JSON</span></span>

<span data-ttu-id="47fb1-180">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="47fb1-180">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="47fb1-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="47fb1-181">Request</span></span>

<span data-ttu-id="47fb1-182">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47fb1-182">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="47fb1-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="47fb1-183">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitydetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityDetail(period='D7')?$format=application/json
```
# <a name="c"></a>[<span data-ttu-id="47fb1-184">C#</span><span class="sxs-lookup"><span data-stu-id="47fb1-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammergroupsactivitydetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="47fb1-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="47fb1-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammergroupsactivitydetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="47fb1-186">Objective-C</span><span class="sxs-lookup"><span data-stu-id="47fb1-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammergroupsactivitydetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="47fb1-187">Отклик</span><span class="sxs-lookup"><span data-stu-id="47fb1-187">Response</span></span>

<span data-ttu-id="47fb1-188">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="47fb1-188">The following is an example of the response.</span></span>

> <span data-ttu-id="47fb1-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="47fb1-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerGroupsActivityDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 441

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerGroupsActivityDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "groupDisplayName": "groupDisplayName-value", 
      "isDeleted": false, 
      "ownerPrincipalName": "ownerPrincipalName-value", 
      "lastActivityDate": "2017-08-30", 
      "groupType": "private", 
      "office365Connected": true, 
      "memberCount": 176, 
      "postedCount": 15, 
      "readCount": 24, 
      "likedCount": 3, 
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
