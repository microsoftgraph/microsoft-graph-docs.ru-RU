---
title: 'reportRoot: getTeamsDeviceUsageDistributionUserCounts'
description: Получение количества уникальных пользователей Microsoft Teams с сортировкой по типам устройств за выбранный период.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: e59c7c82192e287d00ccb1ae4582416955588c47
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868949"
---
# <a name="reportroot-getteamsdeviceusagedistributionusercounts"></a><span data-ttu-id="45f24-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="45f24-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45f24-104">Получение количества уникальных пользователей Microsoft Teams с сортировкой по типам устройств за выбранный период.</span><span class="sxs-lookup"><span data-stu-id="45f24-104">Get the number of Microsoft Teams unique users by device type over the selected time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="45f24-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="45f24-105">Permissions</span></span>

<span data-ttu-id="45f24-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45f24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="45f24-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="45f24-108">Permission type</span></span>                        | <span data-ttu-id="45f24-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="45f24-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="45f24-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="45f24-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="45f24-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="45f24-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="45f24-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="45f24-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45f24-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45f24-113">Not supported.</span></span>                           |
| <span data-ttu-id="45f24-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="45f24-114">Application</span></span>                            | <span data-ttu-id="45f24-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="45f24-115">Reports.Read.All</span></span>                         |

<span data-ttu-id="45f24-116">**Примечание**. для делегированных разрешений, чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя, администратору клиента необходимо назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="45f24-116">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="45f24-117">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="45f24-117">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="45f24-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="45f24-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="45f24-119">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="45f24-119">Function parameters</span></span>

<span data-ttu-id="45f24-120">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="45f24-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="45f24-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="45f24-121">Parameter</span></span> | <span data-ttu-id="45f24-122">Тип</span><span class="sxs-lookup"><span data-stu-id="45f24-122">Type</span></span>   | <span data-ttu-id="45f24-123">Описание</span><span class="sxs-lookup"><span data-stu-id="45f24-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="45f24-124">period</span><span class="sxs-lookup"><span data-stu-id="45f24-124">period</span></span>    | <span data-ttu-id="45f24-125">string</span><span class="sxs-lookup"><span data-stu-id="45f24-125">string</span></span> | <span data-ttu-id="45f24-126">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="45f24-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="45f24-127">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="45f24-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="45f24-128">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="45f24-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="45f24-129">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="45f24-129">Required.</span></span> |

<span data-ttu-id="45f24-130">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="45f24-130">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="45f24-131">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="45f24-131">The default output type is text/csv.</span></span> <span data-ttu-id="45f24-132">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="45f24-132">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="45f24-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="45f24-133">Request headers</span></span>

| <span data-ttu-id="45f24-134">Имя</span><span class="sxs-lookup"><span data-stu-id="45f24-134">Name</span></span>          | <span data-ttu-id="45f24-135">Описание</span><span class="sxs-lookup"><span data-stu-id="45f24-135">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="45f24-136">Авторизация</span><span class="sxs-lookup"><span data-stu-id="45f24-136">Authorization</span></span> | <span data-ttu-id="45f24-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="45f24-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="45f24-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="45f24-139">Response</span></span>

### <a name="csv"></a><span data-ttu-id="45f24-140">CSV</span><span class="sxs-lookup"><span data-stu-id="45f24-140">CSV</span></span>

<span data-ttu-id="45f24-141">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="45f24-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="45f24-142">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="45f24-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="45f24-143">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="45f24-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="45f24-144">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="45f24-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="45f24-145">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="45f24-145">Report Refresh Date</span></span>
- <span data-ttu-id="45f24-146">"Web" (Интернет);</span><span class="sxs-lookup"><span data-stu-id="45f24-146">Web</span></span>
- <span data-ttu-id="45f24-147">"Windows Phone";</span><span class="sxs-lookup"><span data-stu-id="45f24-147">Windows Phone</span></span>
- <span data-ttu-id="45f24-148">"Android Phone" (Телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="45f24-148">Android Phone</span></span>
- <span data-ttu-id="45f24-149">"iOS";</span><span class="sxs-lookup"><span data-stu-id="45f24-149">iOS</span></span>
- <span data-ttu-id="45f24-150">"Mac";</span><span class="sxs-lookup"><span data-stu-id="45f24-150">Mac</span></span>
- <span data-ttu-id="45f24-151">"Windows";</span><span class="sxs-lookup"><span data-stu-id="45f24-151">Windows</span></span>
- <span data-ttu-id="45f24-152">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="45f24-152">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="45f24-153">JSON</span><span class="sxs-lookup"><span data-stu-id="45f24-153">JSON</span></span>

<span data-ttu-id="45f24-154">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[теамсдевицеусажедистрибутионусеркаунтс](../resources/teamsdeviceusagedistributionusercounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="45f24-154">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45f24-155">Пример</span><span class="sxs-lookup"><span data-stu-id="45f24-155">Example</span></span>

### <a name="csv"></a><span data-ttu-id="45f24-156">CSV</span><span class="sxs-lookup"><span data-stu-id="45f24-156">CSV</span></span>

<span data-ttu-id="45f24-157">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="45f24-157">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="45f24-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="45f24-158">Request</span></span>

<span data-ttu-id="45f24-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="45f24-159">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="45f24-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="45f24-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="45f24-161">C#</span><span class="sxs-lookup"><span data-stu-id="45f24-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsdeviceusagedistributionusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="45f24-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="45f24-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsdeviceusagedistributionusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="45f24-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="45f24-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsdeviceusagedistributionusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="45f24-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="45f24-164">Response</span></span>

<span data-ttu-id="45f24-165">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="45f24-165">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="45f24-166">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="45f24-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iOS,Mac,Windows,Report Period
```

### <a name="json"></a><span data-ttu-id="45f24-167">JSON</span><span class="sxs-lookup"><span data-stu-id="45f24-167">JSON</span></span>

<span data-ttu-id="45f24-168">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="45f24-168">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="45f24-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="45f24-169">Request</span></span>

<span data-ttu-id="45f24-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="45f24-170">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="45f24-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="45f24-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="45f24-172">C#</span><span class="sxs-lookup"><span data-stu-id="45f24-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsdeviceusagedistributionusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="45f24-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="45f24-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsdeviceusagedistributionusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="45f24-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="45f24-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsdeviceusagedistributionusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="45f24-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="45f24-175">Response</span></span>

<span data-ttu-id="45f24-176">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="45f24-176">The following is an example of the response.</span></span>

> <span data-ttu-id="45f24-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="45f24-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsDeviceUsageDistributionUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 243

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsDeviceUsageDistributionUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "web": 51, 
      "windowsPhone": 2, 
      "androidPhone": 34, 
      "ios": 76, 
      "mac": 40, 
      "windows": 491, 
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
