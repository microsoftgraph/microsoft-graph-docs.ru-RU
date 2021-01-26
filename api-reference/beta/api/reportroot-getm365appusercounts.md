---
title: 'reportRoot: getM365AppUserCounts'
description: Получите отчет, который обеспечивает тенденцию числа активных пользователей для каждого приложения — Outlook, Word, Excel, PowerPoint, OneNote и Teams — в вашей организации.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 3c415e973e2e0e84edb306d9e64a024f91b1a905
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981356"
---
# <a name="reportroot-getm365appusercounts"></a><span data-ttu-id="6536c-103">reportRoot: getM365AppUserCounts</span><span class="sxs-lookup"><span data-stu-id="6536c-103">reportRoot: getM365AppUserCounts</span></span>

<span data-ttu-id="6536c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6536c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6536c-105">Получите отчет, который обеспечивает тенденцию числа активных пользователей для каждого приложения — Outlook, Word, Excel, PowerPoint, OneNote и Teams — в вашей организации.</span><span class="sxs-lookup"><span data-stu-id="6536c-105">Get a report that provides the trend in the number of active users for each app – Outlook, Word, Excel, PowerPoint, OneNote, and Teams - in your organization.</span></span>

> <span data-ttu-id="6536c-106">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [отчетах Microsoft 365 об использовании приложений Microsoft 365.](/microsoft-365/admin/activity-reports/microsoft365-apps-usage)</span><span class="sxs-lookup"><span data-stu-id="6536c-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft 365 Apps usage](/microsoft-365/admin/activity-reports/microsoft365-apps-usage).</span></span>

## <a name="permissions"></a><span data-ttu-id="6536c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6536c-107">Permissions</span></span>

<span data-ttu-id="6536c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6536c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6536c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6536c-110">Permission type</span></span>                        | <span data-ttu-id="6536c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6536c-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="6536c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6536c-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="6536c-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6536c-113">Reports.Read.All</span></span>                            |
| <span data-ttu-id="6536c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6536c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6536c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6536c-115">Not supported.</span></span>                              |
| <span data-ttu-id="6536c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6536c-116">Application</span></span>                            | <span data-ttu-id="6536c-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6536c-117">Reports.Read.All</span></span>                            |

> <span data-ttu-id="6536c-118">**Примечание.** Чтобы делегировать разрешения, позволяющие приложениям читать отчеты об использовании служб от имени пользователя, администратор клиента должен на назначенную пользователю роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6536c-118">**Note:** For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="6536c-119">Подробные сведения [см. в авторизации для API для чтения отчетов об использовании Microsoft 365.](/graph/reportroot-authorization)</span><span class="sxs-lookup"><span data-stu-id="6536c-119">For details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="6536c-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6536c-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getM365AppUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="6536c-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="6536c-121">Function parameters</span></span>

<span data-ttu-id="6536c-122">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="6536c-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="6536c-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="6536c-123">Parameter</span></span> | <span data-ttu-id="6536c-124">Тип</span><span class="sxs-lookup"><span data-stu-id="6536c-124">Type</span></span>   | <span data-ttu-id="6536c-125">Описание</span><span class="sxs-lookup"><span data-stu-id="6536c-125">Description</span></span>                                                                                                                                                                                                                                                       |
| :-------- | :----- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="6536c-126">period</span><span class="sxs-lookup"><span data-stu-id="6536c-126">period</span></span>    | <span data-ttu-id="6536c-127">string</span><span class="sxs-lookup"><span data-stu-id="6536c-127">string</span></span> | <span data-ttu-id="6536c-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="6536c-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="6536c-129">Поддерживаемые значения для {period_value}: `D7` , `D30` , и `D90` `D180` .</span><span class="sxs-lookup"><span data-stu-id="6536c-129">The supported values for {period_value} are: `D7`, `D30`, `D90`, and `D180`.</span></span> <span data-ttu-id="6536c-130">Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="6536c-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="6536c-131">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6536c-131">Required.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="6536c-132">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6536c-132">Optional query parameters</span></span>

<span data-ttu-id="6536c-133">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="6536c-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="6536c-134">Тип выходных данных по умолчанию — text/csv.</span><span class="sxs-lookup"><span data-stu-id="6536c-134">The default output type is text/csv.</span></span> <span data-ttu-id="6536c-135">Однако если требуется указать тип выходных данных, можно использовать параметр запроса OData, чтобы задать для выходных данных по умолчанию значение `$format` text/csv или application/json.</span><span class="sxs-lookup"><span data-stu-id="6536c-135">However, if you want to specify the output type, you can use the OData `$format` query parameter to set the default output to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6536c-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6536c-136">Request headers</span></span>

| <span data-ttu-id="6536c-137">Имя</span><span class="sxs-lookup"><span data-stu-id="6536c-137">Name</span></span>          | <span data-ttu-id="6536c-138">Описание</span><span class="sxs-lookup"><span data-stu-id="6536c-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="6536c-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6536c-139">Authorization</span></span> | <span data-ttu-id="6536c-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6536c-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6536c-142">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6536c-142">Request body</span></span>

<span data-ttu-id="6536c-143">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6536c-143">Do not supply a request body with this method.</span></span>

## <a name="response"></a><span data-ttu-id="6536c-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="6536c-144">Response</span></span>

<span data-ttu-id="6536c-145">В случае успеха этот метод возвращает код отклика и `200 OK` объект [отчета](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6536c-145">If successful, this method returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) object in the response body.</span></span> <span data-ttu-id="6536c-146">Данные отчета содержатся в свойстве **контента** объекта **отчета.**</span><span class="sxs-lookup"><span data-stu-id="6536c-146">Report data is contained in the **content** property of the **report** object.</span></span>

### <a name="csv"></a><span data-ttu-id="6536c-147">CSV</span><span class="sxs-lookup"><span data-stu-id="6536c-147">CSV</span></span>

<span data-ttu-id="6536c-148">В случае успешного запроса свойства **контента** возвращается ответ, который перенаправляет на URL-адрес предварительной загрузки для `302 Found` отчета.</span><span class="sxs-lookup"><span data-stu-id="6536c-148">If successful, requesting the **content** property returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="6536c-149">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="6536c-149">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="6536c-150">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="6536c-150">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="6536c-151">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="6536c-151">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="6536c-152">Report Refresh Date (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="6536c-152">Report Refresh Date</span></span>
- <span data-ttu-id="6536c-153">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="6536c-153">Report Period</span></span>
- <span data-ttu-id="6536c-154">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="6536c-154">Report Date</span></span>
- <span data-ttu-id="6536c-155">Outlook</span><span class="sxs-lookup"><span data-stu-id="6536c-155">Outlook</span></span>
- <span data-ttu-id="6536c-156">Word</span><span class="sxs-lookup"><span data-stu-id="6536c-156">Word</span></span>
- <span data-ttu-id="6536c-157">Excel</span><span class="sxs-lookup"><span data-stu-id="6536c-157">Excel</span></span>
- <span data-ttu-id="6536c-158">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="6536c-158">PowerPoint</span></span>
- <span data-ttu-id="6536c-159">OneNote</span><span class="sxs-lookup"><span data-stu-id="6536c-159">OneNote</span></span>
- <span data-ttu-id="6536c-160">Teams</span><span class="sxs-lookup"><span data-stu-id="6536c-160">Teams</span></span>

### <a name="json"></a><span data-ttu-id="6536c-161">JSON</span><span class="sxs-lookup"><span data-stu-id="6536c-161">JSON</span></span>

<span data-ttu-id="6536c-162">В случае успешного запроса свойства **контента** возвращается `200 OK` код отклика и объект JSON в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6536c-162">If successful, requesting the **content** property returns a `200 OK` response code and a JSON object in response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6536c-163">Примеры</span><span class="sxs-lookup"><span data-stu-id="6536c-163">Examples</span></span>

### <a name="example-1-csv-output"></a><span data-ttu-id="6536c-164">Пример 1. Выходные данные CSV</span><span class="sxs-lookup"><span data-stu-id="6536c-164">Example 1: CSV output</span></span>

<span data-ttu-id="6536c-165">Ниже приводится пример вывода CSV-данных.</span><span class="sxs-lookup"><span data-stu-id="6536c-165">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="6536c-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="6536c-166">Request</span></span>

<span data-ttu-id="6536c-167">Ниже приводится пример запроса на получения **свойства контента.**</span><span class="sxs-lookup"><span data-stu-id="6536c-167">The following is an example of the request to get the **content** property.</span></span>



# <a name="http"></a>[<span data-ttu-id="6536c-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="6536c-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getM365AppUserCounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getM365AppUserCounts(period='D7')/content?$format=text/csv
```
# <a name="c"></a>[<span data-ttu-id="6536c-169">C#</span><span class="sxs-lookup"><span data-stu-id="6536c-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getm365appusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6536c-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6536c-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getm365appusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6536c-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6536c-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getm365appusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6536c-172">Java</span><span class="sxs-lookup"><span data-stu-id="6536c-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getm365appusercounts-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="6536c-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="6536c-173">Response</span></span>

<span data-ttu-id="6536c-174">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6536c-174">The following is an example of the response.</span></span>

<!-- { "blockType": "response" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="6536c-175">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="6536c-175">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Period,Report Date,Outlook,Word,Excel,PowerPoint,OneNote,Teams
```

### <a name="example-2-json-output"></a><span data-ttu-id="6536c-176">Пример 2. Выходные данные JSON</span><span class="sxs-lookup"><span data-stu-id="6536c-176">Example 2: JSON output</span></span>

<span data-ttu-id="6536c-177">Ниже приводится пример, который возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="6536c-177">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="6536c-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="6536c-178">Request</span></span>

<span data-ttu-id="6536c-179">Ниже приводится пример запроса на получения **свойства контента.**</span><span class="sxs-lookup"><span data-stu-id="6536c-179">The following is an example of the request to get the **content** property.</span></span>



# <a name="http"></a>[<span data-ttu-id="6536c-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="6536c-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getM365AppUserCounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getM365AppUserCounts(period='D7')/content?$format=application/json
```
# <a name="c"></a>[<span data-ttu-id="6536c-181">C#</span><span class="sxs-lookup"><span data-stu-id="6536c-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getm365appusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6536c-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6536c-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getm365appusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6536c-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6536c-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getm365appusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6536c-184">Java</span><span class="sxs-lookup"><span data-stu-id="6536c-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getm365appusercounts-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="6536c-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="6536c-185">Response</span></span>

<span data-ttu-id="6536c-186">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6536c-186">The following is an example of the response.</span></span>

> <span data-ttu-id="6536c-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6536c-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 188

{
  "value": [
    {
      "reportRefreshDate": "2020-06-30",
      "reportPeriod": 7,
      "userCounts": [
        {
          "reportDate": "2020-06-30",
          "outlook": 1513,
          "word": 911,
          "excel": 790,
          "powerPoint": 683,
          "oneNote": 969,
          "teams": 1532
        }
      ]
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
