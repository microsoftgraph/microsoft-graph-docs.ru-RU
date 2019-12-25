---
title: 'reportRoot: getOffice365ActiveUserCounts'
description: Получение количества активных пользователей за каждый день отчетного периода по продукту.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: d92293e3daba5ba86d18ecdea347d70782e13170
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867559"
---
# <a name="reportroot-getoffice365activeusercounts"></a><span data-ttu-id="ac6aa-103">reportRoot: getOffice365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="ac6aa-103">reportRoot: getOffice365ActiveUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac6aa-104">Получение количества активных пользователей за каждый день отчетного периода по продукту.</span><span class="sxs-lookup"><span data-stu-id="ac6aa-104">Get the count of daily active users in the reporting period by product.</span></span>

> <span data-ttu-id="ac6aa-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: активные пользователи](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="ac6aa-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="ac6aa-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ac6aa-106">Permissions</span></span>

<span data-ttu-id="ac6aa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac6aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ac6aa-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ac6aa-109">Permission type</span></span>                        | <span data-ttu-id="ac6aa-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ac6aa-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ac6aa-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ac6aa-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ac6aa-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ac6aa-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ac6aa-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ac6aa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac6aa-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac6aa-114">Not supported.</span></span>                           |
| <span data-ttu-id="ac6aa-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ac6aa-115">Application</span></span>                            | <span data-ttu-id="ac6aa-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ac6aa-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="ac6aa-117">**Примечание**. для делегированных разрешений, чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя, администратору клиента необходимо назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ac6aa-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="ac6aa-118">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="ac6aa-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="ac6aa-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ac6aa-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="ac6aa-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="ac6aa-120">Function parameters</span></span>

<span data-ttu-id="ac6aa-121">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="ac6aa-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="ac6aa-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="ac6aa-122">Parameter</span></span> | <span data-ttu-id="ac6aa-123">Тип</span><span class="sxs-lookup"><span data-stu-id="ac6aa-123">Type</span></span>   | <span data-ttu-id="ac6aa-124">Описание</span><span class="sxs-lookup"><span data-stu-id="ac6aa-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="ac6aa-125">period</span><span class="sxs-lookup"><span data-stu-id="ac6aa-125">period</span></span>    | <span data-ttu-id="ac6aa-126">string</span><span class="sxs-lookup"><span data-stu-id="ac6aa-126">string</span></span> | <span data-ttu-id="ac6aa-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="ac6aa-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="ac6aa-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="ac6aa-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="ac6aa-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="ac6aa-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="ac6aa-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ac6aa-130">Required.</span></span> |

<span data-ttu-id="ac6aa-131">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="ac6aa-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="ac6aa-132">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="ac6aa-132">The default output type is text/csv.</span></span> <span data-ttu-id="ac6aa-133">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="ac6aa-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ac6aa-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ac6aa-134">Request headers</span></span>

| <span data-ttu-id="ac6aa-135">Имя</span><span class="sxs-lookup"><span data-stu-id="ac6aa-135">Name</span></span>          | <span data-ttu-id="ac6aa-136">Описание</span><span class="sxs-lookup"><span data-stu-id="ac6aa-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="ac6aa-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ac6aa-137">Authorization</span></span> | <span data-ttu-id="ac6aa-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ac6aa-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="ac6aa-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac6aa-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="ac6aa-141">CSV</span><span class="sxs-lookup"><span data-stu-id="ac6aa-141">CSV</span></span>

<span data-ttu-id="ac6aa-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="ac6aa-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ac6aa-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="ac6aa-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ac6aa-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="ac6aa-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ac6aa-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="ac6aa-145">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="ac6aa-146">Report Refresh Date (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="ac6aa-146">Report Refresh Date</span></span>
- <span data-ttu-id="ac6aa-147">Office 365</span><span class="sxs-lookup"><span data-stu-id="ac6aa-147">Office 365</span></span>
- <span data-ttu-id="ac6aa-148">Exchange</span><span class="sxs-lookup"><span data-stu-id="ac6aa-148">Exchange</span></span>
- <span data-ttu-id="ac6aa-149">OneDrive;</span><span class="sxs-lookup"><span data-stu-id="ac6aa-149">OneDrive</span></span>
- <span data-ttu-id="ac6aa-150">SharePoint;</span><span class="sxs-lookup"><span data-stu-id="ac6aa-150">SharePoint</span></span>
- <span data-ttu-id="ac6aa-151">Skype для бизнеса</span><span class="sxs-lookup"><span data-stu-id="ac6aa-151">Skype For Business</span></span> 
- <span data-ttu-id="ac6aa-152">Yammer</span><span class="sxs-lookup"><span data-stu-id="ac6aa-152">Yammer</span></span>
- <span data-ttu-id="ac6aa-153">Teams</span><span class="sxs-lookup"><span data-stu-id="ac6aa-153">Teams</span></span>
- <span data-ttu-id="ac6aa-154">Report Date (Дата отчета)</span><span class="sxs-lookup"><span data-stu-id="ac6aa-154">Report Date</span></span>
- <span data-ttu-id="ac6aa-155">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="ac6aa-155">Report Period</span></span>

<span data-ttu-id="ac6aa-156">Следующие столбцы не поддерживаются в Китае Microsoft Graph, предоставляемом компанией 21Vianet:</span><span class="sxs-lookup"><span data-stu-id="ac6aa-156">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="ac6aa-157">Yammer</span><span class="sxs-lookup"><span data-stu-id="ac6aa-157">Yammer</span></span>
- <span data-ttu-id="ac6aa-158">Teams</span><span class="sxs-lookup"><span data-stu-id="ac6aa-158">Teams</span></span>

### <a name="json"></a><span data-ttu-id="ac6aa-159">JSON</span><span class="sxs-lookup"><span data-stu-id="ac6aa-159">JSON</span></span>

<span data-ttu-id="ac6aa-160">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ac6aa-160">If successful, this method returns a `200 OK` response code and an **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** object in the response body.</span></span>

<span data-ttu-id="ac6aa-161">Следующие свойства в объекте **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** не поддерживаются в Китае Microsoft Graph, предоставляемом компанией 21vianet:</span><span class="sxs-lookup"><span data-stu-id="ac6aa-161">The following properties in **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="ac6aa-162">Yammer</span><span class="sxs-lookup"><span data-stu-id="ac6aa-162">yammer</span></span>
- <span data-ttu-id="ac6aa-163">Teams</span><span class="sxs-lookup"><span data-stu-id="ac6aa-163">teams</span></span>

## <a name="example"></a><span data-ttu-id="ac6aa-164">Пример</span><span class="sxs-lookup"><span data-stu-id="ac6aa-164">Example</span></span>

### <a name="csv"></a><span data-ttu-id="ac6aa-165">CSV</span><span class="sxs-lookup"><span data-stu-id="ac6aa-165">CSV</span></span>

<span data-ttu-id="ac6aa-166">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="ac6aa-166">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="ac6aa-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="ac6aa-167">Request</span></span>

<span data-ttu-id="ac6aa-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ac6aa-168">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ac6aa-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="ac6aa-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ac6aa-170">C#</span><span class="sxs-lookup"><span data-stu-id="ac6aa-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activeusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ac6aa-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ac6aa-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activeusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ac6aa-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ac6aa-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activeusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ac6aa-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac6aa-173">Response</span></span>

<span data-ttu-id="ac6aa-174">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ac6aa-174">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="ac6aa-175">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="ac6aa-175">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Office 365,Exchange,OneDrive,SharePoint,Skype For Business,Yammer,Teams,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="ac6aa-176">JSON</span><span class="sxs-lookup"><span data-stu-id="ac6aa-176">JSON</span></span>

<span data-ttu-id="ac6aa-177">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="ac6aa-177">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="ac6aa-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="ac6aa-178">Request</span></span>

<span data-ttu-id="ac6aa-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ac6aa-179">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ac6aa-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="ac6aa-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ac6aa-181">C#</span><span class="sxs-lookup"><span data-stu-id="ac6aa-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activeusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ac6aa-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ac6aa-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activeusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ac6aa-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ac6aa-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activeusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ac6aa-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac6aa-184">Response</span></span>

<span data-ttu-id="ac6aa-185">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ac6aa-185">The following is an example of the response.</span></span>

> <span data-ttu-id="ac6aa-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ac6aa-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ActiveUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 317

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365ActiveUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "office365": 1718, 
      "exchange": 1429, 
      "oneDrive": 350, 
      "sharePoint": 795, 
      "skypeForBusiness": 251, 
      "yammer": 47, 
      "teams": 10, 
      "reportDate": "2017-08-29", 
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
