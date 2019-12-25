---
title: 'reportRoot: getTeamsDeviceUsageUserCounts'
description: Получение сведений о количестве уникальных пользователей Microsoft Teams в день с сортировкой по типам устройств.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 19663a689efa2359df7f6aa5b3a461c23262021b
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868919"
---
# <a name="reportroot-getteamsdeviceusageusercounts"></a><span data-ttu-id="b1b6d-103">reportRoot: getTeamsDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="b1b6d-103">reportRoot: getTeamsDeviceUsageUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1b6d-104">Получение сведений о количестве уникальных пользователей Microsoft Teams в день с сортировкой по типам устройств.</span><span class="sxs-lookup"><span data-stu-id="b1b6d-104">Get the number of Microsoft Teams daily unique users by device type.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1b6d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b1b6d-105">Permissions</span></span>

<span data-ttu-id="b1b6d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1b6d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b1b6d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b1b6d-108">Permission type</span></span>                        | <span data-ttu-id="b1b6d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b1b6d-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b1b6d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b1b6d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b1b6d-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b1b6d-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b1b6d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b1b6d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1b6d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1b6d-113">Not supported.</span></span>                           |
| <span data-ttu-id="b1b6d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b1b6d-114">Application</span></span>                            | <span data-ttu-id="b1b6d-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b1b6d-115">Reports.Read.All</span></span>                         |

<span data-ttu-id="b1b6d-116">**Примечание**. для делегированных разрешений, чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя, администратору клиента необходимо назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b1b6d-116">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="b1b6d-117">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="b1b6d-117">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="b1b6d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b1b6d-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="b1b6d-119">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="b1b6d-119">Function parameters</span></span>

<span data-ttu-id="b1b6d-120">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="b1b6d-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="b1b6d-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="b1b6d-121">Parameter</span></span> | <span data-ttu-id="b1b6d-122">Тип</span><span class="sxs-lookup"><span data-stu-id="b1b6d-122">Type</span></span>   | <span data-ttu-id="b1b6d-123">Описание</span><span class="sxs-lookup"><span data-stu-id="b1b6d-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b1b6d-124">period</span><span class="sxs-lookup"><span data-stu-id="b1b6d-124">period</span></span>    | <span data-ttu-id="b1b6d-125">string</span><span class="sxs-lookup"><span data-stu-id="b1b6d-125">string</span></span> | <span data-ttu-id="b1b6d-126">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="b1b6d-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b1b6d-127">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="b1b6d-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b1b6d-128">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="b1b6d-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="b1b6d-129">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1b6d-129">Required.</span></span> |

<span data-ttu-id="b1b6d-130">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="b1b6d-130">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="b1b6d-131">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="b1b6d-131">The default output type is text/csv.</span></span> <span data-ttu-id="b1b6d-132">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="b1b6d-132">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b1b6d-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b1b6d-133">Request headers</span></span>

| <span data-ttu-id="b1b6d-134">Имя</span><span class="sxs-lookup"><span data-stu-id="b1b6d-134">Name</span></span>          | <span data-ttu-id="b1b6d-135">Описание</span><span class="sxs-lookup"><span data-stu-id="b1b6d-135">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="b1b6d-136">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b1b6d-136">Authorization</span></span> | <span data-ttu-id="b1b6d-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1b6d-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="b1b6d-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1b6d-139">Response</span></span>

### <a name="csv"></a><span data-ttu-id="b1b6d-140">CSV</span><span class="sxs-lookup"><span data-stu-id="b1b6d-140">CSV</span></span>

<span data-ttu-id="b1b6d-141">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="b1b6d-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b1b6d-142">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="b1b6d-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b1b6d-143">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="b1b6d-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b1b6d-144">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="b1b6d-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b1b6d-145">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="b1b6d-145">Report Refresh Date</span></span>
- <span data-ttu-id="b1b6d-146">"Web" (Интернет);</span><span class="sxs-lookup"><span data-stu-id="b1b6d-146">Web</span></span>
- <span data-ttu-id="b1b6d-147">"Windows Phone";</span><span class="sxs-lookup"><span data-stu-id="b1b6d-147">Windows Phone</span></span>
- <span data-ttu-id="b1b6d-148">"Android Phone" (Телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="b1b6d-148">Android Phone</span></span>
- <span data-ttu-id="b1b6d-149">"iOS";</span><span class="sxs-lookup"><span data-stu-id="b1b6d-149">iOS</span></span>
- <span data-ttu-id="b1b6d-150">"Mac";</span><span class="sxs-lookup"><span data-stu-id="b1b6d-150">Mac</span></span>
- <span data-ttu-id="b1b6d-151">"Windows";</span><span class="sxs-lookup"><span data-stu-id="b1b6d-151">Windows</span></span>
- <span data-ttu-id="b1b6d-152">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="b1b6d-152">Report Date</span></span>
- <span data-ttu-id="b1b6d-153">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="b1b6d-153">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="b1b6d-154">JSON</span><span class="sxs-lookup"><span data-stu-id="b1b6d-154">JSON</span></span>

<span data-ttu-id="b1b6d-155">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[теамсдевицеусажеусеркаунтс](../resources/teamsdeviceusageusercounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b1b6d-155">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageUserCounts](../resources/teamsdeviceusageusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1b6d-156">Пример</span><span class="sxs-lookup"><span data-stu-id="b1b6d-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="b1b6d-157">CSV</span><span class="sxs-lookup"><span data-stu-id="b1b6d-157">CSV</span></span>

<span data-ttu-id="b1b6d-158">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="b1b6d-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="b1b6d-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1b6d-159">Request</span></span>

<span data-ttu-id="b1b6d-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b1b6d-160">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b1b6d-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="b1b6d-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b1b6d-162">C#</span><span class="sxs-lookup"><span data-stu-id="b1b6d-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsdeviceusageusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b1b6d-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b1b6d-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsdeviceusageusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b1b6d-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b1b6d-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsdeviceusageusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b1b6d-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1b6d-165">Response</span></span>

<span data-ttu-id="b1b6d-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b1b6d-166">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="b1b6d-167">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="b1b6d-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iOS,Mac,Windows,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="b1b6d-168">JSON</span><span class="sxs-lookup"><span data-stu-id="b1b6d-168">JSON</span></span>

<span data-ttu-id="b1b6d-169">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="b1b6d-169">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="b1b6d-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1b6d-170">Request</span></span>

<span data-ttu-id="b1b6d-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b1b6d-171">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b1b6d-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="b1b6d-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b1b6d-173">C#</span><span class="sxs-lookup"><span data-stu-id="b1b6d-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsdeviceusageusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b1b6d-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b1b6d-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsdeviceusageusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b1b6d-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b1b6d-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsdeviceusageusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b1b6d-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1b6d-176">Response</span></span>

<span data-ttu-id="b1b6d-177">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b1b6d-177">The following is an example of the response.</span></span>

> <span data-ttu-id="b1b6d-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b1b6d-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 269

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsDeviceUsageUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "web": 13, 
      "windowsPhone": 0, 
      "androidPhone": 22, 
      "ios": 75, 
      "mac": 16, 
      "windows": 257, 
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
