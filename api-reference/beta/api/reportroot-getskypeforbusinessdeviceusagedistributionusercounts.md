---
title: 'reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts'
description: Узнайте, сколько сотрудников организации используют уникальные устройства. В отчете будет показано количество пользователей устройств с Windows, телефонов с Windows, телефонов с Android, iPhone и iPad.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: b92525ca73ea17e35c0de430ca2e141834c6764e
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867370"
---
# <a name="reportroot-getskypeforbusinessdeviceusagedistributionusercounts"></a><span data-ttu-id="d38f4-104">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="d38f4-104">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d38f4-105">Узнайте, сколько сотрудников организации используют уникальные устройства.</span><span class="sxs-lookup"><span data-stu-id="d38f4-105">Get the number of users using unique devices in your organization.</span></span> <span data-ttu-id="d38f4-106">В отчете будет показано количество пользователей Windows, телефонов с Windows, телефонов с Android, iPhone и iPad.</span><span class="sxs-lookup"><span data-stu-id="d38f4-106">The report will show you the number of users per device including Windows, Windows phone, Android phone, iPhone, and iPad.</span></span>

> <span data-ttu-id="d38f4-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span><span class="sxs-lookup"><span data-stu-id="d38f4-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="d38f4-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d38f4-108">Permissions</span></span>

<span data-ttu-id="d38f4-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d38f4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d38f4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d38f4-111">Permission type</span></span>                        | <span data-ttu-id="d38f4-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d38f4-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="d38f4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d38f4-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="d38f4-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d38f4-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="d38f4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d38f4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d38f4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d38f4-116">Not supported.</span></span>                           |
| <span data-ttu-id="d38f4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d38f4-117">Application</span></span>                            | <span data-ttu-id="d38f4-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d38f4-118">Reports.Read.All</span></span>                         |

<span data-ttu-id="d38f4-119">**Примечание**. для делегированных разрешений, чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя, администратору клиента необходимо назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d38f4-119">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="d38f4-120">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="d38f4-120">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="d38f4-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d38f4-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="d38f4-122">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="d38f4-122">Function parameters</span></span>

<span data-ttu-id="d38f4-123">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="d38f4-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="d38f4-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="d38f4-124">Parameter</span></span> | <span data-ttu-id="d38f4-125">Тип</span><span class="sxs-lookup"><span data-stu-id="d38f4-125">Type</span></span>   | <span data-ttu-id="d38f4-126">Описание</span><span class="sxs-lookup"><span data-stu-id="d38f4-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="d38f4-127">period</span><span class="sxs-lookup"><span data-stu-id="d38f4-127">period</span></span>    | <span data-ttu-id="d38f4-128">string</span><span class="sxs-lookup"><span data-stu-id="d38f4-128">string</span></span> | <span data-ttu-id="d38f4-129">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="d38f4-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="d38f4-130">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="d38f4-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="d38f4-131">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="d38f4-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="d38f4-132">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d38f4-132">Required.</span></span> |

<span data-ttu-id="d38f4-133">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="d38f4-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="d38f4-134">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="d38f4-134">The default output type is text/csv.</span></span> <span data-ttu-id="d38f4-135">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="d38f4-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d38f4-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d38f4-136">Request headers</span></span>

| <span data-ttu-id="d38f4-137">Имя</span><span class="sxs-lookup"><span data-stu-id="d38f4-137">Name</span></span>          | <span data-ttu-id="d38f4-138">Описание</span><span class="sxs-lookup"><span data-stu-id="d38f4-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="d38f4-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d38f4-139">Authorization</span></span> | <span data-ttu-id="d38f4-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d38f4-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="d38f4-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="d38f4-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="d38f4-143">CSV</span><span class="sxs-lookup"><span data-stu-id="d38f4-143">CSV</span></span>

<span data-ttu-id="d38f4-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="d38f4-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d38f4-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="d38f4-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d38f4-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="d38f4-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="d38f4-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="d38f4-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="d38f4-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="d38f4-148">Report Refresh Date</span></span>
- <span data-ttu-id="d38f4-149">"Windows";</span><span class="sxs-lookup"><span data-stu-id="d38f4-149">Windows</span></span>
- <span data-ttu-id="d38f4-150">"Windows Phone";</span><span class="sxs-lookup"><span data-stu-id="d38f4-150">Windows Phone</span></span>
- <span data-ttu-id="d38f4-151">"Android Phone" (Телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="d38f4-151">Android Phone</span></span>
- <span data-ttu-id="d38f4-152">iPhone</span><span class="sxs-lookup"><span data-stu-id="d38f4-152">iPhone</span></span>
- <span data-ttu-id="d38f4-153">iPad</span><span class="sxs-lookup"><span data-stu-id="d38f4-153">iPad</span></span>
- <span data-ttu-id="d38f4-154">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="d38f4-154">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="d38f4-155">JSON</span><span class="sxs-lookup"><span data-stu-id="d38f4-155">JSON</span></span>

<span data-ttu-id="d38f4-156">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[скипефорбусинессдевицеусажедистрибутионусеркаунтс](../resources/skypeforbusinessdeviceusagedistributionusercounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d38f4-156">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessDeviceUsageDistributionUserCounts](../resources/skypeforbusinessdeviceusagedistributionusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d38f4-157">Пример</span><span class="sxs-lookup"><span data-stu-id="d38f4-157">Example</span></span>

### <a name="csv"></a><span data-ttu-id="d38f4-158">CSV</span><span class="sxs-lookup"><span data-stu-id="d38f4-158">CSV</span></span>

<span data-ttu-id="d38f4-159">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="d38f4-159">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="d38f4-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="d38f4-160">Request</span></span>

<span data-ttu-id="d38f4-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d38f4-161">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d38f4-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="d38f4-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusagedistributionusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d38f4-163">C#</span><span class="sxs-lookup"><span data-stu-id="d38f4-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessdeviceusagedistributionusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d38f4-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d38f4-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessdeviceusagedistributionusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d38f4-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d38f4-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessdeviceusagedistributionusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d38f4-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="d38f4-166">Response</span></span>

<span data-ttu-id="d38f4-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d38f4-167">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="d38f4-168">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="d38f4-168">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Windows,Windows Phone,Android Phone,iPhone,iPad,Report Period
```

### <a name="json"></a><span data-ttu-id="d38f4-169">JSON</span><span class="sxs-lookup"><span data-stu-id="d38f4-169">JSON</span></span>

<span data-ttu-id="d38f4-170">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="d38f4-170">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="d38f4-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="d38f4-171">Request</span></span>

<span data-ttu-id="d38f4-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d38f4-172">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d38f4-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="d38f4-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusagedistributionusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d38f4-174">C#</span><span class="sxs-lookup"><span data-stu-id="d38f4-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessdeviceusagedistributionusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d38f4-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d38f4-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessdeviceusagedistributionusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d38f4-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d38f4-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessdeviceusagedistributionusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d38f4-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="d38f4-177">Response</span></span>

<span data-ttu-id="d38f4-178">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d38f4-178">The following is an example of the response.</span></span>

> <span data-ttu-id="d38f4-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d38f4-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageDistributionUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 275

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessDeviceUsageDistributionUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "windows": 122, 
      "windowsPhone": 8, 
      "androidPhone": 19, 
      "iPhone": 28, 
      "iPad": 1, 
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
