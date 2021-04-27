---
title: 'reportRoot: getM365AppPlatformUserCounts'
description: Получите отчет, который предоставляет тенденцию активных пользователей во всех приложениях для каждой платформы — Windows, Mac, web и mobile — в вашей организации.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 2f6377776cedc7394c2e9573c24e5209d7dda755
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050950"
---
# <a name="reportroot-getm365appplatformusercounts"></a><span data-ttu-id="3f4d0-103">reportRoot: getM365AppPlatformUserCounts</span><span class="sxs-lookup"><span data-stu-id="3f4d0-103">reportRoot: getM365AppPlatformUserCounts</span></span>

<span data-ttu-id="3f4d0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f4d0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f4d0-105">Получите отчет, который предоставляет тенденцию активных пользователей во всех приложениях для каждой платформы — Windows, Mac, web и mobile — в вашей организации.</span><span class="sxs-lookup"><span data-stu-id="3f4d0-105">Get a report that provides the trend of active users across all apps for each platform – Windows, Mac, web, and mobile - in your organization.</span></span>

> <span data-ttu-id="3f4d0-106">**Примечание:** Сведения о различных представлениях отчетов и [именах см. в Microsoft 365 отчетов - Приложения Microsoft 365 использования.](/microsoft-365/admin/activity-reports/microsoft365-apps-usage)</span><span class="sxs-lookup"><span data-stu-id="3f4d0-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft 365 Apps usage](/microsoft-365/admin/activity-reports/microsoft365-apps-usage).</span></span>

## <a name="permissions"></a><span data-ttu-id="3f4d0-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3f4d0-107">Permissions</span></span>

<span data-ttu-id="3f4d0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f4d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3f4d0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3f4d0-110">Permission type</span></span>                        | <span data-ttu-id="3f4d0-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3f4d0-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="3f4d0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3f4d0-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="3f4d0-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3f4d0-113">Reports.Read.All</span></span>                            |
| <span data-ttu-id="3f4d0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3f4d0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3f4d0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f4d0-115">Not supported.</span></span>                              |
| <span data-ttu-id="3f4d0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3f4d0-116">Application</span></span>                            | <span data-ttu-id="3f4d0-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3f4d0-117">Reports.Read.All</span></span>                            |

> <span data-ttu-id="3f4d0-118">**Примечание:** Для делегирования разрешений, позволяющих приложениям читать отчеты об использовании служб от имени пользователя, администратор клиента должен присвоить пользователю соответствующую роль администратора Azure AD с ограниченной ответственностью.</span><span class="sxs-lookup"><span data-stu-id="3f4d0-118">**Note:** For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="3f4d0-119">Подробные сведения [см. в публикации Авторизация API для Microsoft 365 отчетов об использовании.](/graph/reportroot-authorization)</span><span class="sxs-lookup"><span data-stu-id="3f4d0-119">For details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="3f4d0-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3f4d0-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getM365AppPlatformUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="3f4d0-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="3f4d0-121">Function parameters</span></span>

<span data-ttu-id="3f4d0-122">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="3f4d0-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="3f4d0-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="3f4d0-123">Parameter</span></span> | <span data-ttu-id="3f4d0-124">Тип</span><span class="sxs-lookup"><span data-stu-id="3f4d0-124">Type</span></span>   | <span data-ttu-id="3f4d0-125">Описание</span><span class="sxs-lookup"><span data-stu-id="3f4d0-125">Description</span></span>                                                                                                                                                                                                                                                       |
| :-------- | :----- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="3f4d0-126">period</span><span class="sxs-lookup"><span data-stu-id="3f4d0-126">period</span></span>    | <span data-ttu-id="3f4d0-127">string</span><span class="sxs-lookup"><span data-stu-id="3f4d0-127">string</span></span> | <span data-ttu-id="3f4d0-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="3f4d0-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="3f4d0-129">Поддерживаемые значения {period_value} : `D7` , `D30` , и `D90` `D180` .</span><span class="sxs-lookup"><span data-stu-id="3f4d0-129">The supported values for {period_value} are: `D7`, `D30`, `D90`, and `D180`.</span></span> <span data-ttu-id="3f4d0-130">Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="3f4d0-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="3f4d0-131">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3f4d0-131">Required.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="3f4d0-132">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3f4d0-132">Optional query parameters</span></span>

<span data-ttu-id="3f4d0-133">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="3f4d0-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="3f4d0-134">Тип вывода по умолчанию — текст/csv.</span><span class="sxs-lookup"><span data-stu-id="3f4d0-134">The default output type is text/csv.</span></span> <span data-ttu-id="3f4d0-135">Однако если требуется указать тип вывода, можно использовать параметр запроса OData, чтобы задать выход по умолчанию `$format` тексту/csv или приложению/json.</span><span class="sxs-lookup"><span data-stu-id="3f4d0-135">However, if you want to specify the output type, you can use the OData `$format` query parameter to set the default output to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3f4d0-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3f4d0-136">Request headers</span></span>

| <span data-ttu-id="3f4d0-137">Имя</span><span class="sxs-lookup"><span data-stu-id="3f4d0-137">Name</span></span>          | <span data-ttu-id="3f4d0-138">Описание</span><span class="sxs-lookup"><span data-stu-id="3f4d0-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="3f4d0-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3f4d0-139">Authorization</span></span> | <span data-ttu-id="3f4d0-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3f4d0-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3f4d0-142">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3f4d0-142">Request body</span></span>

<span data-ttu-id="3f4d0-143">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3f4d0-143">Do not supply a request body with this method.</span></span>

## <a name="response"></a><span data-ttu-id="3f4d0-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f4d0-144">Response</span></span>

<span data-ttu-id="3f4d0-145">В случае успешной работы этот метод возвращает код `200 OK` отклика и объект [отчета](../resources/intune-shared-report.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3f4d0-145">If successful, this method returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) object in the response body.</span></span> <span data-ttu-id="3f4d0-146">Данные отчета содержатся в **свойстве** контента объекта **отчета.**</span><span class="sxs-lookup"><span data-stu-id="3f4d0-146">Report data is contained in the **content** property of the **report** object.</span></span>

### <a name="csv"></a><span data-ttu-id="3f4d0-147">CSV</span><span class="sxs-lookup"><span data-stu-id="3f4d0-147">CSV</span></span>

<span data-ttu-id="3f4d0-148">В случае успешного  запроса свойства контента возвращается ответ, который перенаправляется на предварительно заранее задаваемые URL-адрес `302 Found` загрузки отчета.</span><span class="sxs-lookup"><span data-stu-id="3f4d0-148">If successful, requesting the **content** property returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="3f4d0-149">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="3f4d0-149">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="3f4d0-150">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="3f4d0-150">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="3f4d0-151">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="3f4d0-151">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="3f4d0-152">Report Refresh Date (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="3f4d0-152">Report Refresh Date</span></span>
- <span data-ttu-id="3f4d0-153">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="3f4d0-153">Report Period</span></span>
- <span data-ttu-id="3f4d0-154">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="3f4d0-154">Report Date</span></span>
- <span data-ttu-id="3f4d0-155">Outlook</span><span class="sxs-lookup"><span data-stu-id="3f4d0-155">Outlook</span></span>
- <span data-ttu-id="3f4d0-156">Word</span><span class="sxs-lookup"><span data-stu-id="3f4d0-156">Word</span></span>
- <span data-ttu-id="3f4d0-157">Excel</span><span class="sxs-lookup"><span data-stu-id="3f4d0-157">Excel</span></span>
- <span data-ttu-id="3f4d0-158">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="3f4d0-158">PowerPoint</span></span>
- <span data-ttu-id="3f4d0-159">OneNote</span><span class="sxs-lookup"><span data-stu-id="3f4d0-159">OneNote</span></span>
- <span data-ttu-id="3f4d0-160">Teams</span><span class="sxs-lookup"><span data-stu-id="3f4d0-160">Teams</span></span>

### <a name="json"></a><span data-ttu-id="3f4d0-161">JSON</span><span class="sxs-lookup"><span data-stu-id="3f4d0-161">JSON</span></span>

<span data-ttu-id="3f4d0-162">В случае успешной работы запрос свойства **контента** возвращает код отклика `200 OK` и объект JSON в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3f4d0-162">If successful, requesting the **content** property returns a `200 OK` response code and a JSON object in response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3f4d0-163">Примеры</span><span class="sxs-lookup"><span data-stu-id="3f4d0-163">Examples</span></span>

### <a name="example-1-csv-output"></a><span data-ttu-id="3f4d0-164">Пример 1. Выход CSV</span><span class="sxs-lookup"><span data-stu-id="3f4d0-164">Example 1: CSV output</span></span>

<span data-ttu-id="3f4d0-165">Ниже приводится пример, который выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="3f4d0-165">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="3f4d0-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="3f4d0-166">Request</span></span>

<span data-ttu-id="3f4d0-167">Ниже приводится пример запроса на получения **свойства** контента.</span><span class="sxs-lookup"><span data-stu-id="3f4d0-167">The following is an example of the request to get the **content** property.</span></span>



# <a name="http"></a>[<span data-ttu-id="3f4d0-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="3f4d0-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getM365AppPlatformUserCounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getM365AppPlatformUserCounts(period='D7')/content?$format=text/csv
```
# <a name="c"></a>[<span data-ttu-id="3f4d0-169">C#</span><span class="sxs-lookup"><span data-stu-id="3f4d0-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getm365appplatformusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3f4d0-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3f4d0-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getm365appplatformusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3f4d0-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3f4d0-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getm365appplatformusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3f4d0-172">Java</span><span class="sxs-lookup"><span data-stu-id="3f4d0-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getm365appplatformusercounts-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="3f4d0-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f4d0-173">Response</span></span>

<span data-ttu-id="3f4d0-174">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3f4d0-174">The following is an example of the response.</span></span>

<!-- { "blockType": "response" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="3f4d0-175">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="3f4d0-175">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="example-2-json-output"></a><span data-ttu-id="3f4d0-176">Пример 2. Вывод JSON</span><span class="sxs-lookup"><span data-stu-id="3f4d0-176">Example 2: JSON output</span></span>

<span data-ttu-id="3f4d0-177">Ниже приводится пример, который возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="3f4d0-177">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="3f4d0-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="3f4d0-178">Request</span></span>

<span data-ttu-id="3f4d0-179">Ниже приводится пример запроса на получения **свойства** контента.</span><span class="sxs-lookup"><span data-stu-id="3f4d0-179">The following is an example of the request to get the **content** property.</span></span>



# <a name="http"></a>[<span data-ttu-id="3f4d0-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="3f4d0-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getM365AppPlatformUserCounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getM365AppPlatformUserCounts(period='D7')/content?$format=application/json
```
# <a name="c"></a>[<span data-ttu-id="3f4d0-181">C#</span><span class="sxs-lookup"><span data-stu-id="3f4d0-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getm365appplatformusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3f4d0-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3f4d0-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getm365appplatformusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3f4d0-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3f4d0-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getm365appplatformusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3f4d0-184">Java</span><span class="sxs-lookup"><span data-stu-id="3f4d0-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getm365appplatformusercounts-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="3f4d0-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f4d0-185">Response</span></span>

<span data-ttu-id="3f4d0-186">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3f4d0-186">The following is an example of the response.</span></span>

> <span data-ttu-id="3f4d0-187">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3f4d0-187">**Note:** The response object shown here might be shortened for readability.</span></span>

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
