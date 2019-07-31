---
title: 'reportRoot: getTeamsUserActivityUserDetail'
description: Получение сведений о действиях отдельных пользователей Microsoft Teams.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 15456b0f341ef16742764c0191a66fdf9c3c9bf1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35983133"
---
# <a name="reportroot-getteamsuseractivityuserdetail"></a><span data-ttu-id="97e3d-103">reportRoot: getTeamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="97e3d-103">reportRoot: getTeamsUserActivityUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97e3d-104">Получение сведений о действиях отдельных пользователей Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="97e3d-104">Get details about Microsoft Teams user activity by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="97e3d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="97e3d-105">Permissions</span></span>

<span data-ttu-id="97e3d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97e3d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="97e3d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="97e3d-108">Permission type</span></span>                        | <span data-ttu-id="97e3d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="97e3d-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="97e3d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="97e3d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="97e3d-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="97e3d-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="97e3d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="97e3d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97e3d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97e3d-113">Not supported.</span></span>                           |
| <span data-ttu-id="97e3d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="97e3d-114">Application</span></span>                            | <span data-ttu-id="97e3d-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="97e3d-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="97e3d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="97e3d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserDetail(period='D7')
GET /reports/getTeamsUserActivityUserDetail(date=2017-09-01)
```

## <a name="function-parameters"></a><span data-ttu-id="97e3d-117">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="97e3d-117">Function parameters</span></span>

<span data-ttu-id="97e3d-118">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="97e3d-118">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="97e3d-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="97e3d-119">Parameter</span></span> | <span data-ttu-id="97e3d-120">Тип</span><span class="sxs-lookup"><span data-stu-id="97e3d-120">Type</span></span>   | <span data-ttu-id="97e3d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="97e3d-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="97e3d-122">period</span><span class="sxs-lookup"><span data-stu-id="97e3d-122">period</span></span>    | <span data-ttu-id="97e3d-123">string</span><span class="sxs-lookup"><span data-stu-id="97e3d-123">string</span></span> | <span data-ttu-id="97e3d-124">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="97e3d-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="97e3d-125">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="97e3d-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="97e3d-126">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="97e3d-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="97e3d-127">date</span><span class="sxs-lookup"><span data-stu-id="97e3d-127">date</span></span>      | <span data-ttu-id="97e3d-128">Date</span><span class="sxs-lookup"><span data-stu-id="97e3d-128">Date</span></span>   | <span data-ttu-id="97e3d-129">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="97e3d-129">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="97e3d-130">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="97e3d-130">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="97e3d-131">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="97e3d-131">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="97e3d-132">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="97e3d-132">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="97e3d-133">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="97e3d-133">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="97e3d-134">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="97e3d-134">The default output type is text/csv.</span></span> <span data-ttu-id="97e3d-135">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="97e3d-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="97e3d-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="97e3d-136">Request headers</span></span>

| <span data-ttu-id="97e3d-137">Имя</span><span class="sxs-lookup"><span data-stu-id="97e3d-137">Name</span></span>          | <span data-ttu-id="97e3d-138">Описание</span><span class="sxs-lookup"><span data-stu-id="97e3d-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="97e3d-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="97e3d-139">Authorization</span></span> | <span data-ttu-id="97e3d-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="97e3d-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="97e3d-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="97e3d-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="97e3d-143">CSV</span><span class="sxs-lookup"><span data-stu-id="97e3d-143">CSV</span></span>

<span data-ttu-id="97e3d-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="97e3d-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="97e3d-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="97e3d-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="97e3d-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="97e3d-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="97e3d-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="97e3d-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="97e3d-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="97e3d-148">Report Refresh Date</span></span>
- <span data-ttu-id="97e3d-149">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="97e3d-149">User Principal Name</span></span>
- <span data-ttu-id="97e3d-150">Last Activity Date (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="97e3d-150">Last Activity Date</span></span>
- <span data-ttu-id="97e3d-151">Is Deleted (Удален);</span><span class="sxs-lookup"><span data-stu-id="97e3d-151">Is Deleted</span></span>
- <span data-ttu-id="97e3d-152">Deleted Date (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="97e3d-152">Deleted Date</span></span>
- <span data-ttu-id="97e3d-153">Assigned Products (Назначенные продукты);</span><span class="sxs-lookup"><span data-stu-id="97e3d-153">Assigned Products</span></span>
- <span data-ttu-id="97e3d-154">Team Chat Messages Count (Количество сообщений в чатах групп);</span><span class="sxs-lookup"><span data-stu-id="97e3d-154">Team Chat Message Count</span></span>
- <span data-ttu-id="97e3d-155">Private Chat Message Count (Количество сообщений в приватных чатах);</span><span class="sxs-lookup"><span data-stu-id="97e3d-155">Private Chat Message Count</span></span>
- <span data-ttu-id="97e3d-156">Call Count (Количество звонков);</span><span class="sxs-lookup"><span data-stu-id="97e3d-156">Call Count</span></span>
- <span data-ttu-id="97e3d-157">Meeting Count (Количество собраний);</span><span class="sxs-lookup"><span data-stu-id="97e3d-157">Meeting Count</span></span>
- <span data-ttu-id="97e3d-158">Has Other Action (Есть другое действие);</span><span class="sxs-lookup"><span data-stu-id="97e3d-158">Has Other Action</span></span>
- <span data-ttu-id="97e3d-159">Report Period (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="97e3d-159">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="97e3d-160">JSON</span><span class="sxs-lookup"><span data-stu-id="97e3d-160">JSON</span></span>

<span data-ttu-id="97e3d-161">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[теамсусерактивитюсердетаил](../resources/teamsuseractivityuserdetail.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="97e3d-161">If successful, this method returns a `200 OK` response code and a **[teamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="97e3d-162">Размер страницы по умолчанию для этого запроса составляет 2000 элементов.</span><span class="sxs-lookup"><span data-stu-id="97e3d-162">The default page size for this request is 2000 items.</span></span>

## <a name="example"></a><span data-ttu-id="97e3d-163">Пример</span><span class="sxs-lookup"><span data-stu-id="97e3d-163">Example</span></span>

### <a name="csv"></a><span data-ttu-id="97e3d-164">CSV</span><span class="sxs-lookup"><span data-stu-id="97e3d-164">CSV</span></span>

<span data-ttu-id="97e3d-165">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="97e3d-165">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="97e3d-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="97e3d-166">Request</span></span>

<span data-ttu-id="97e3d-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="97e3d-167">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="97e3d-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="97e3d-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="97e3d-169">C#</span><span class="sxs-lookup"><span data-stu-id="97e3d-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsuseractivityuserdetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="97e3d-170">Javascript</span><span class="sxs-lookup"><span data-stu-id="97e3d-170">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsuseractivityuserdetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="97e3d-171">Цель — C</span><span class="sxs-lookup"><span data-stu-id="97e3d-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsuseractivityuserdetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="97e3d-172">Java</span><span class="sxs-lookup"><span data-stu-id="97e3d-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getteamsuseractivityuserdetail-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="97e3d-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="97e3d-173">Response</span></span>

<span data-ttu-id="97e3d-174">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="97e3d-174">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="97e3d-175">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="97e3d-175">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Is Deleted,Deleted Date,Assigned Products,Team Chat Message Count,Private Chat Message Count,Call Count,Meeting Count,Has Other Action,Report Period
```

### <a name="json"></a><span data-ttu-id="97e3d-176">JSON</span><span class="sxs-lookup"><span data-stu-id="97e3d-176">JSON</span></span>

<span data-ttu-id="97e3d-177">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="97e3d-177">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="97e3d-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="97e3d-178">Request</span></span>

<span data-ttu-id="97e3d-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="97e3d-179">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="97e3d-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="97e3d-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="97e3d-181">C#</span><span class="sxs-lookup"><span data-stu-id="97e3d-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsuseractivityuserdetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="97e3d-182">Javascript</span><span class="sxs-lookup"><span data-stu-id="97e3d-182">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsuseractivityuserdetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="97e3d-183">Цель — C</span><span class="sxs-lookup"><span data-stu-id="97e3d-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsuseractivityuserdetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="97e3d-184">Java</span><span class="sxs-lookup"><span data-stu-id="97e3d-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getteamsuseractivityuserdetail-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="97e3d-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="97e3d-185">Response</span></span>

<span data-ttu-id="97e3d-186">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="97e3d-186">The following is an example of the response.</span></span>

> <span data-ttu-id="97e3d-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="97e3d-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsUserActivityUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 452

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsUserActivityUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "lastActivityDate": "2017-09-01", 
      "isDeleted": false, 
      "deletedDate": null, 
      "assignedProducts": [
        "OFFICE 365 ENTERPRISE E5"
      ], 
      "teamChatMessageCount": 0, 
      "privateChatMessageCount": 49, 
      "callCount": 2, 
      "meetingCount": 0, 
      "hasOtherAction": true, 
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
