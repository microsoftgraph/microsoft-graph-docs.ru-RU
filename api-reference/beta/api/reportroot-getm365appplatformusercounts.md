---
title: 'Reportroot.: getM365AppPlatformUserCounts'
description: Получите отчет, который обеспечивает тенденцию активных пользователей по всем приложениям для каждой платформы — Windows, Mac, Интернета и мобильных устройств в вашей организации.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: da99bf47dcc7d56101a46dfdca67f971b55178aa
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/30/2020
ms.locfileid: "48313872"
---
# <a name="reportroot-getm365appplatformusercounts"></a><span data-ttu-id="c9575-103">Reportroot.: getM365AppPlatformUserCounts</span><span class="sxs-lookup"><span data-stu-id="c9575-103">reportRoot: getM365AppPlatformUserCounts</span></span>

<span data-ttu-id="c9575-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9575-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9575-105">Получите отчет, который обеспечивает тенденцию активных пользователей по всем приложениям для каждой платформы — Windows, Mac, Интернета и мобильных устройств в вашей организации.</span><span class="sxs-lookup"><span data-stu-id="c9575-105">Get a report that provides the trend of active users across all apps for each platform – Windows, Mac, web, and mobile - in your organization.</span></span>

> <span data-ttu-id="c9575-106">**Примечание:** Сведения о различных представлениях отчетов и их именах можно найти в [статье microsoft 365 Reports — использование приложений microsoft 365](/microsoft-365/admin/activity-reports/microsoft365-apps-usage).</span><span class="sxs-lookup"><span data-stu-id="c9575-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft 365 Apps usage](/microsoft-365/admin/activity-reports/microsoft365-apps-usage).</span></span>

## <a name="permissions"></a><span data-ttu-id="c9575-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c9575-107">Permissions</span></span>

<span data-ttu-id="c9575-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9575-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c9575-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c9575-110">Permission type</span></span>                        | <span data-ttu-id="c9575-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c9575-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="c9575-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c9575-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="c9575-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c9575-113">Reports.Read.All</span></span>                            |
| <span data-ttu-id="c9575-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c9575-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9575-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9575-115">Not supported.</span></span>                              |
| <span data-ttu-id="c9575-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c9575-116">Application</span></span>                            | <span data-ttu-id="c9575-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c9575-117">Reports.Read.All</span></span>                            |

> <span data-ttu-id="c9575-118">**Примечание:** Для делегированных разрешений, позволяющих приложениям читать отчеты об использовании служб от имени пользователя, администратору клиента необходимо назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c9575-118">**Note:** For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="c9575-119">Дополнительные сведения см. [в статье авторизация для API для чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="c9575-119">For details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="c9575-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c9575-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getM365AppPlatformUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="c9575-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="c9575-121">Function parameters</span></span>

<span data-ttu-id="c9575-122">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="c9575-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="c9575-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="c9575-123">Parameter</span></span> | <span data-ttu-id="c9575-124">Тип</span><span class="sxs-lookup"><span data-stu-id="c9575-124">Type</span></span>   | <span data-ttu-id="c9575-125">Описание</span><span class="sxs-lookup"><span data-stu-id="c9575-125">Description</span></span>                                                                                                                                                                                                                                                       |
| :-------- | :----- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="c9575-126">period</span><span class="sxs-lookup"><span data-stu-id="c9575-126">period</span></span>    | <span data-ttu-id="c9575-127">string</span><span class="sxs-lookup"><span data-stu-id="c9575-127">string</span></span> | <span data-ttu-id="c9575-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="c9575-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="c9575-129">Для {period_value} поддерживаются следующие значения: `D7` , `D30` , `D90` и `D180` .</span><span class="sxs-lookup"><span data-stu-id="c9575-129">The supported values for {period_value} are: `D7`, `D30`, `D90`, and `D180`.</span></span> <span data-ttu-id="c9575-130">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="c9575-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="c9575-131">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c9575-131">Required.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="c9575-132">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c9575-132">Optional query parameters</span></span>

<span data-ttu-id="c9575-133">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="c9575-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="c9575-134">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="c9575-134">The default output type is text/csv.</span></span> <span data-ttu-id="c9575-135">Тем не менее, если вы хотите указать тип выходных данных, можно использовать `$format` параметр запроса OData для установки выходных данных по умолчанию в Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="c9575-135">However, if you want to specify the output type, you can use the OData `$format` query parameter to set the default output to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c9575-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c9575-136">Request headers</span></span>

| <span data-ttu-id="c9575-137">Имя</span><span class="sxs-lookup"><span data-stu-id="c9575-137">Name</span></span>          | <span data-ttu-id="c9575-138">Описание</span><span class="sxs-lookup"><span data-stu-id="c9575-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="c9575-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c9575-139">Authorization</span></span> | <span data-ttu-id="c9575-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c9575-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c9575-142">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c9575-142">Request body</span></span>

<span data-ttu-id="c9575-143">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c9575-143">Do not supply a request body with this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9575-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9575-144">Response</span></span>

<span data-ttu-id="c9575-145">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [Report](../resources/intune-shared-report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c9575-145">If successful, this method returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) object in the response body.</span></span> <span data-ttu-id="c9575-146">Данные отчета хранятся в свойстве **Content** объекта **Report** .</span><span class="sxs-lookup"><span data-stu-id="c9575-146">Report data is contained in the **content** property of the **report** object.</span></span>

### <a name="csv"></a><span data-ttu-id="c9575-147">CSV</span><span class="sxs-lookup"><span data-stu-id="c9575-147">CSV</span></span>

<span data-ttu-id="c9575-148">При успешном выполнении запрос свойства **Content** возвращает `302 Found` ответ, который перенаправляет на URL-адрес скачивания, прошедший проверку подлинности для отчета.</span><span class="sxs-lookup"><span data-stu-id="c9575-148">If successful, requesting the **content** property returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="c9575-149">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="c9575-149">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="c9575-150">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="c9575-150">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="c9575-151">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="c9575-151">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="c9575-152">Report Refresh Date (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="c9575-152">Report Refresh Date</span></span>
- <span data-ttu-id="c9575-153">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="c9575-153">Report Period</span></span>
- <span data-ttu-id="c9575-154">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="c9575-154">Report Date</span></span>
- <span data-ttu-id="c9575-155">Outlook</span><span class="sxs-lookup"><span data-stu-id="c9575-155">Outlook</span></span>
- <span data-ttu-id="c9575-156">Word</span><span class="sxs-lookup"><span data-stu-id="c9575-156">Word</span></span>
- <span data-ttu-id="c9575-157">Excel</span><span class="sxs-lookup"><span data-stu-id="c9575-157">Excel</span></span>
- <span data-ttu-id="c9575-158">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="c9575-158">PowerPoint</span></span>
- <span data-ttu-id="c9575-159">OneNote</span><span class="sxs-lookup"><span data-stu-id="c9575-159">OneNote</span></span>
- <span data-ttu-id="c9575-160">Teams</span><span class="sxs-lookup"><span data-stu-id="c9575-160">Teams</span></span>

### <a name="json"></a><span data-ttu-id="c9575-161">JSON</span><span class="sxs-lookup"><span data-stu-id="c9575-161">JSON</span></span>

<span data-ttu-id="c9575-162">В случае успешного выполнения запрос свойства **Content** возвращает `200 OK` код отклика и объект JSON в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c9575-162">If successful, requesting the **content** property returns a `200 OK` response code and a JSON object in response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c9575-163">Примеры</span><span class="sxs-lookup"><span data-stu-id="c9575-163">Examples</span></span>

### <a name="example-1-csv-output"></a><span data-ttu-id="c9575-164">Пример 1: вывод в формате CSV</span><span class="sxs-lookup"><span data-stu-id="c9575-164">Example 1: CSV output</span></span>

<span data-ttu-id="c9575-165">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="c9575-165">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="c9575-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9575-166">Request</span></span>

<span data-ttu-id="c9575-167">Ниже приведен пример запроса на получение свойства **содержимого** .</span><span class="sxs-lookup"><span data-stu-id="c9575-167">The following is an example of the request to get the **content** property.</span></span>



# <a name="http"></a>[<span data-ttu-id="c9575-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="c9575-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getM365AppPlatformUserCounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getM365AppPlatformUserCounts(period='D7')/content?$format=text/csv
```
# <a name="c"></a>[<span data-ttu-id="c9575-169">C#</span><span class="sxs-lookup"><span data-stu-id="c9575-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getm365appplatformusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c9575-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c9575-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getm365appplatformusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c9575-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c9575-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getm365appplatformusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="c9575-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9575-172">Response</span></span>

<span data-ttu-id="c9575-173">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c9575-173">The following is an example of the response.</span></span>

<!-- { "blockType": "response" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="c9575-174">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="c9575-174">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Period,Report Date,Windows,Mac,Mobile,Web
```

### <a name="example-2-json-output"></a><span data-ttu-id="c9575-175">Пример 2: выходные данные JSON</span><span class="sxs-lookup"><span data-stu-id="c9575-175">Example 2: JSON output</span></span>

<span data-ttu-id="c9575-176">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="c9575-176">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="c9575-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9575-177">Request</span></span>

<span data-ttu-id="c9575-178">Ниже приведен пример запроса на получение свойства **содержимого** .</span><span class="sxs-lookup"><span data-stu-id="c9575-178">The following is an example of the request to get the **content** property.</span></span>



# <a name="http"></a>[<span data-ttu-id="c9575-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="c9575-179">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getM365AppPlatformUserCounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getM365AppPlatformUserCounts(period='D7')/content?$format=application/json
```
# <a name="c"></a>[<span data-ttu-id="c9575-180">C#</span><span class="sxs-lookup"><span data-stu-id="c9575-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getm365appplatformusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c9575-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c9575-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getm365appplatformusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c9575-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c9575-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getm365appplatformusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="c9575-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9575-183">Response</span></span>

<span data-ttu-id="c9575-184">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c9575-184">The following is an example of the response.</span></span>

> <span data-ttu-id="c9575-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c9575-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 156

{
  "value": [
    {
      "reportRefreshDate": "2020-06-30",
      "reportPeriod": 7,
      "userCounts": [
        {
          "reportDate": "2020-06-30",
          "windows": 1445,
          "mac": 146,
          "mobile": 1131,
          "web": 1080
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