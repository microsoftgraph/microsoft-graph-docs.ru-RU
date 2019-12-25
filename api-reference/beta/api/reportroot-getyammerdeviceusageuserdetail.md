---
title: 'reportRoot: getYammerDeviceUsageUserDetail function'
description: Получение сведений об использовании устройства с Yammer с разбивкой по пользователям.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: e80aa5253d5548b6181395664a150420811b196d
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867045"
---
# <a name="reportroot-getyammerdeviceusageuserdetail-function"></a><span data-ttu-id="06462-103">reportRoot: getYammerDeviceUsageUserDetail function</span><span class="sxs-lookup"><span data-stu-id="06462-103">reportRoot: getYammerDeviceUsageUserDetail function</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06462-104">Получение сведений об использовании устройства с Yammer с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="06462-104">Get details about Yammer device usage by user.</span></span>

> <span data-ttu-id="06462-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: использование устройств с Yammer](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="06462-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="06462-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="06462-106">Permissions</span></span>

<span data-ttu-id="06462-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06462-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="06462-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="06462-109">Permission type</span></span>                        | <span data-ttu-id="06462-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="06462-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="06462-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="06462-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="06462-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="06462-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="06462-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="06462-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06462-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06462-114">Not supported.</span></span>                           |
| <span data-ttu-id="06462-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="06462-115">Application</span></span>                            | <span data-ttu-id="06462-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="06462-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="06462-117">**Примечание**. для делегированных разрешений, чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя, администратору клиента необходимо назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="06462-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="06462-118">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="06462-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="06462-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="06462-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserDetail(period='{period_value}')
GET /reports/getYammerDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="06462-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="06462-120">Function parameters</span></span>

<span data-ttu-id="06462-121">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="06462-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="06462-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="06462-122">Parameter</span></span> | <span data-ttu-id="06462-123">Тип</span><span class="sxs-lookup"><span data-stu-id="06462-123">Type</span></span>   | <span data-ttu-id="06462-124">Описание</span><span class="sxs-lookup"><span data-stu-id="06462-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="06462-125">period</span><span class="sxs-lookup"><span data-stu-id="06462-125">period</span></span>    | <span data-ttu-id="06462-126">string</span><span class="sxs-lookup"><span data-stu-id="06462-126">string</span></span> | <span data-ttu-id="06462-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="06462-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="06462-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="06462-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="06462-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="06462-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="06462-130">date</span><span class="sxs-lookup"><span data-stu-id="06462-130">date</span></span>      | <span data-ttu-id="06462-131">Date</span><span class="sxs-lookup"><span data-stu-id="06462-131">Date</span></span>   | <span data-ttu-id="06462-132">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="06462-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="06462-133">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="06462-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="06462-134">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="06462-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="06462-135">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="06462-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="06462-136">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="06462-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="06462-137">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="06462-137">The default output type is text/csv.</span></span> <span data-ttu-id="06462-138">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="06462-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="06462-139">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="06462-139">Request headers</span></span>

| <span data-ttu-id="06462-140">Имя</span><span class="sxs-lookup"><span data-stu-id="06462-140">Name</span></span>          | <span data-ttu-id="06462-141">Описание</span><span class="sxs-lookup"><span data-stu-id="06462-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="06462-142">Авторизация</span><span class="sxs-lookup"><span data-stu-id="06462-142">Authorization</span></span> | <span data-ttu-id="06462-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="06462-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="06462-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="06462-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="06462-146">CSV</span><span class="sxs-lookup"><span data-stu-id="06462-146">CSV</span></span>

<span data-ttu-id="06462-147">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="06462-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="06462-148">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="06462-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="06462-149">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="06462-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="06462-150">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="06462-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="06462-151">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="06462-151">Report Refresh Date</span></span>
- <span data-ttu-id="06462-152">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="06462-152">User Principal Name</span></span>
- <span data-ttu-id="06462-153">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="06462-153">Display Name</span></span>
- <span data-ttu-id="06462-154">"User State" (Состояние пользователя);</span><span class="sxs-lookup"><span data-stu-id="06462-154">User State</span></span>
- <span data-ttu-id="06462-155">"State Change Date" (Дата изменения состояния);</span><span class="sxs-lookup"><span data-stu-id="06462-155">State Change Date</span></span>
- <span data-ttu-id="06462-156">"Last Activity Date" (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="06462-156">Last Activity Date</span></span>
- <span data-ttu-id="06462-157">"Used Web" (Используемое веб-приложение);</span><span class="sxs-lookup"><span data-stu-id="06462-157">Used Web</span></span>
- <span data-ttu-id="06462-158">"Used Windows Phone" (Используемое устройство Windows Phone);</span><span class="sxs-lookup"><span data-stu-id="06462-158">Used Windows Phone</span></span>
- <span data-ttu-id="06462-159">"Used Android Phone" (Используемый телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="06462-159">Used Android Phone</span></span>
- <span data-ttu-id="06462-160">"Used iPhone" (Используемый телефон iPhone);</span><span class="sxs-lookup"><span data-stu-id="06462-160">Used iPhone</span></span>
- <span data-ttu-id="06462-161">"Used iPad" (Используемое устройство iPad);</span><span class="sxs-lookup"><span data-stu-id="06462-161">Used iPad</span></span>
- <span data-ttu-id="06462-162">"Used Others" (Другое используемое);</span><span class="sxs-lookup"><span data-stu-id="06462-162">Used Others</span></span>
- <span data-ttu-id="06462-163">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="06462-163">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="06462-164">JSON</span><span class="sxs-lookup"><span data-stu-id="06462-164">JSON</span></span>

<span data-ttu-id="06462-165">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[яммердевицеусажеусердетаил](../resources/yammerdeviceusageuserdetail.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="06462-165">If successful, this method returns a `200 OK` response code and a **[yammerDeviceUsageUserDetail](../resources/yammerdeviceusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="06462-166">Размер страницы по умолчанию для этого запроса составляет 200 элементов.</span><span class="sxs-lookup"><span data-stu-id="06462-166">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="06462-167">Пример</span><span class="sxs-lookup"><span data-stu-id="06462-167">Example</span></span>

### <a name="csv"></a><span data-ttu-id="06462-168">CSV</span><span class="sxs-lookup"><span data-stu-id="06462-168">CSV</span></span>

<span data-ttu-id="06462-169">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="06462-169">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="06462-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="06462-170">Request</span></span>

<span data-ttu-id="06462-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="06462-171">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="06462-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="06462-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusageuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageUserDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="06462-173">C#</span><span class="sxs-lookup"><span data-stu-id="06462-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammerdeviceusageuserdetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="06462-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="06462-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammerdeviceusageuserdetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="06462-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="06462-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammerdeviceusageuserdetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="06462-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="06462-176">Response</span></span>

<span data-ttu-id="06462-177">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="06462-177">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="06462-178">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="06462-178">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,User State,State Change Date,Last Activity Date,Used Web,Used Windows Phone,Used Android Phone,Used iPhone,Used iPad,Used Others,Report Period
```

### <a name="json"></a><span data-ttu-id="06462-179">JSON</span><span class="sxs-lookup"><span data-stu-id="06462-179">JSON</span></span>

<span data-ttu-id="06462-180">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="06462-180">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="06462-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="06462-181">Request</span></span>

<span data-ttu-id="06462-182">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="06462-182">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="06462-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="06462-183">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusageuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageUserDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="06462-184">C#</span><span class="sxs-lookup"><span data-stu-id="06462-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammerdeviceusageuserdetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="06462-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="06462-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammerdeviceusageuserdetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="06462-186">Objective-C</span><span class="sxs-lookup"><span data-stu-id="06462-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammerdeviceusageuserdetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="06462-187">Отклик</span><span class="sxs-lookup"><span data-stu-id="06462-187">Response</span></span>

<span data-ttu-id="06462-188">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="06462-188">The following is an example of the response.</span></span>

> <span data-ttu-id="06462-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="06462-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerDeviceUsageUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 442

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerDeviceUsageUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-06", 
      "userPrincipalName": "userPrincipalName-value", 
      "displayName": "displayName-value", 
      "userState": "active", 
      "stateChangeDate": "2012-06-26", 
      "lastActivityDate": "2017-09-06", 
      "usedWeb": true, 
      "usedWindowsPhone": false, 
      "usedAndroidPhone": false, 
      "usediPhone": false, 
      "usediPad": false, 
      "usedOthers": false, 
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
