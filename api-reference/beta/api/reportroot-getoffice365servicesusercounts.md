---
title: 'reportRoot: getOffice365ServicesUserCounts'
description: Узнайте, сколько пользователей были активны и неактивны в каждой службе.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: f9f117cb11280d573076cf9a7278c96f4f4e6dbe
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869110"
---
# <a name="reportroot-getoffice365servicesusercounts"></a><span data-ttu-id="8bcaf-103">reportRoot: getOffice365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="8bcaf-103">reportRoot: getOffice365ServicesUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8bcaf-104">Узнайте, сколько пользователей были активны и неактивны в каждой службе.</span><span class="sxs-lookup"><span data-stu-id="8bcaf-104">Get the count of users by activity type and service.</span></span>

> <span data-ttu-id="8bcaf-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: активные пользователи](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="8bcaf-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="8bcaf-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8bcaf-106">Permissions</span></span>

<span data-ttu-id="8bcaf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8bcaf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8bcaf-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8bcaf-109">Permission type</span></span>                        | <span data-ttu-id="8bcaf-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8bcaf-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="8bcaf-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8bcaf-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8bcaf-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8bcaf-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="8bcaf-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8bcaf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8bcaf-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8bcaf-114">Not supported.</span></span>                           |
| <span data-ttu-id="8bcaf-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8bcaf-115">Application</span></span>                            | <span data-ttu-id="8bcaf-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8bcaf-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="8bcaf-117">**Примечание**. для делегированных разрешений, чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя, администратору клиента необходимо назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8bcaf-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="8bcaf-118">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="8bcaf-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="8bcaf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8bcaf-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ServicesUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="8bcaf-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="8bcaf-120">Function parameters</span></span>

<span data-ttu-id="8bcaf-121">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="8bcaf-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="8bcaf-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="8bcaf-122">Parameter</span></span> | <span data-ttu-id="8bcaf-123">Тип</span><span class="sxs-lookup"><span data-stu-id="8bcaf-123">Type</span></span>   | <span data-ttu-id="8bcaf-124">Описание</span><span class="sxs-lookup"><span data-stu-id="8bcaf-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="8bcaf-125">period</span><span class="sxs-lookup"><span data-stu-id="8bcaf-125">period</span></span>    | <span data-ttu-id="8bcaf-126">string</span><span class="sxs-lookup"><span data-stu-id="8bcaf-126">string</span></span> | <span data-ttu-id="8bcaf-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="8bcaf-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="8bcaf-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="8bcaf-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="8bcaf-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="8bcaf-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="8bcaf-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8bcaf-130">Required.</span></span> |

<span data-ttu-id="8bcaf-131">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="8bcaf-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="8bcaf-132">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="8bcaf-132">The default output type is text/csv.</span></span> <span data-ttu-id="8bcaf-133">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="8bcaf-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8bcaf-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8bcaf-134">Request headers</span></span>

| <span data-ttu-id="8bcaf-135">Имя</span><span class="sxs-lookup"><span data-stu-id="8bcaf-135">Name</span></span>          | <span data-ttu-id="8bcaf-136">Описание</span><span class="sxs-lookup"><span data-stu-id="8bcaf-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="8bcaf-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8bcaf-137">Authorization</span></span> | <span data-ttu-id="8bcaf-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8bcaf-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="8bcaf-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="8bcaf-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="8bcaf-141">CSV</span><span class="sxs-lookup"><span data-stu-id="8bcaf-141">CSV</span></span>

<span data-ttu-id="8bcaf-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="8bcaf-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="8bcaf-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="8bcaf-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="8bcaf-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="8bcaf-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="8bcaf-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="8bcaf-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="8bcaf-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="8bcaf-146">Report Refresh Date</span></span>
- <span data-ttu-id="8bcaf-147">Exchange Active (активны в Exchange)</span><span class="sxs-lookup"><span data-stu-id="8bcaf-147">Exchange Active</span></span>
- <span data-ttu-id="8bcaf-148">Exchange Inactive (неактивны в Exchange)</span><span class="sxs-lookup"><span data-stu-id="8bcaf-148">Exchange Inactive</span></span>
- <span data-ttu-id="8bcaf-149">OneDrive Active (активны в OneDrive)</span><span class="sxs-lookup"><span data-stu-id="8bcaf-149">OneDrive Active</span></span>
- <span data-ttu-id="8bcaf-150">OneDrive Inactive (неактивны в OneDrive)</span><span class="sxs-lookup"><span data-stu-id="8bcaf-150">OneDrive Inactive</span></span>
- <span data-ttu-id="8bcaf-151">SharePoint Active (активны в SharePoint)</span><span class="sxs-lookup"><span data-stu-id="8bcaf-151">SharePoint Active</span></span>
- <span data-ttu-id="8bcaf-152">SharePoint Inactive (неактивны в SharePoint)</span><span class="sxs-lookup"><span data-stu-id="8bcaf-152">SharePoint Inactive</span></span>
- <span data-ttu-id="8bcaf-153">Skype For Business Active (активны в Skype для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="8bcaf-153">Skype For Business Active</span></span>
- <span data-ttu-id="8bcaf-154">Skype For Business Inactive (неактивны в Skype для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="8bcaf-154">Skype For Business Inactive</span></span>
- <span data-ttu-id="8bcaf-155">Yammer Active (активны в Yammer)</span><span class="sxs-lookup"><span data-stu-id="8bcaf-155">Yammer Active</span></span>
- <span data-ttu-id="8bcaf-156">Yammer Inactive (неактивны в Yammer)</span><span class="sxs-lookup"><span data-stu-id="8bcaf-156">Yammer Inactive</span></span>
- <span data-ttu-id="8bcaf-157">Teams Active (активны в Teams)</span><span class="sxs-lookup"><span data-stu-id="8bcaf-157">Teams Active</span></span>
- <span data-ttu-id="8bcaf-158">Teams Inactive (неактивны в Teams)</span><span class="sxs-lookup"><span data-stu-id="8bcaf-158">Teams Inactive</span></span>
- <span data-ttu-id="8bcaf-159">Office 365 активен</span><span class="sxs-lookup"><span data-stu-id="8bcaf-159">Office 365 Active</span></span>
- <span data-ttu-id="8bcaf-160">Office 365 неактивен</span><span class="sxs-lookup"><span data-stu-id="8bcaf-160">Office 365 Inactive</span></span>
- <span data-ttu-id="8bcaf-161">Report Period (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="8bcaf-161">Report Period</span></span>

<span data-ttu-id="8bcaf-162">Следующие столбцы не поддерживаются в Китае Microsoft Graph, предоставляемом компанией 21Vianet:</span><span class="sxs-lookup"><span data-stu-id="8bcaf-162">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="8bcaf-163">Yammer Active (активны в Yammer)</span><span class="sxs-lookup"><span data-stu-id="8bcaf-163">Yammer Active</span></span>
- <span data-ttu-id="8bcaf-164">Yammer Inactive (неактивны в Yammer)</span><span class="sxs-lookup"><span data-stu-id="8bcaf-164">Yammer Inactive</span></span>
- <span data-ttu-id="8bcaf-165">Teams Active (активны в Teams)</span><span class="sxs-lookup"><span data-stu-id="8bcaf-165">Teams Active</span></span>
- <span data-ttu-id="8bcaf-166">Teams Inactive (неактивны в Teams)</span><span class="sxs-lookup"><span data-stu-id="8bcaf-166">Teams Inactive</span></span>

### <a name="json"></a><span data-ttu-id="8bcaf-167">JSON</span><span class="sxs-lookup"><span data-stu-id="8bcaf-167">JSON</span></span>

<span data-ttu-id="8bcaf-168">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8bcaf-168">If successful, this method returns a `200 OK` response code and an **[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** object in the response body.</span></span>

<span data-ttu-id="8bcaf-169">Следующие свойства в объекте **[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** не поддерживаются в Китае Microsoft Graph, предоставляемом компанией 21vianet:</span><span class="sxs-lookup"><span data-stu-id="8bcaf-169">The following properties in **[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="8bcaf-170">яммерактиве</span><span class="sxs-lookup"><span data-stu-id="8bcaf-170">yammerActive</span></span>
- <span data-ttu-id="8bcaf-171">яммеринактиве</span><span class="sxs-lookup"><span data-stu-id="8bcaf-171">yammerInactive</span></span>
- <span data-ttu-id="8bcaf-172">теамсактиве</span><span class="sxs-lookup"><span data-stu-id="8bcaf-172">teamsActive</span></span>
- <span data-ttu-id="8bcaf-173">теамсинактиве</span><span class="sxs-lookup"><span data-stu-id="8bcaf-173">teamsInactive</span></span>

## <a name="example"></a><span data-ttu-id="8bcaf-174">Пример</span><span class="sxs-lookup"><span data-stu-id="8bcaf-174">Example</span></span>

### <a name="csv"></a><span data-ttu-id="8bcaf-175">CSV</span><span class="sxs-lookup"><span data-stu-id="8bcaf-175">CSV</span></span>

<span data-ttu-id="8bcaf-176">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="8bcaf-176">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="8bcaf-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="8bcaf-177">Request</span></span>

<span data-ttu-id="8bcaf-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8bcaf-178">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8bcaf-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="8bcaf-179">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365servicesusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ServicesUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8bcaf-180">C#</span><span class="sxs-lookup"><span data-stu-id="8bcaf-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365servicesusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8bcaf-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8bcaf-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365servicesusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8bcaf-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8bcaf-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365servicesusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8bcaf-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="8bcaf-183">Response</span></span>

<span data-ttu-id="8bcaf-184">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8bcaf-184">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="8bcaf-185">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="8bcaf-185">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Exchange Active,Exchange Inactive,OneDrive Active,OneDrive Inactive,SharePoint Active,SharePoint Inactive,Skype For Business Active,Skype For Business Inactive,Yammer Active,Yammer Inactive,Teams Active,Teams Inactive,Office 365 Active,Office 365 Inactive,Report Period
```

### <a name="json"></a><span data-ttu-id="8bcaf-186">JSON</span><span class="sxs-lookup"><span data-stu-id="8bcaf-186">JSON</span></span> 

<span data-ttu-id="8bcaf-187">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="8bcaf-187">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="8bcaf-188">Запрос</span><span class="sxs-lookup"><span data-stu-id="8bcaf-188">Request</span></span>

<span data-ttu-id="8bcaf-189">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8bcaf-189">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8bcaf-190">HTTP</span><span class="sxs-lookup"><span data-stu-id="8bcaf-190">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365servicesusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ServicesUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8bcaf-191">C#</span><span class="sxs-lookup"><span data-stu-id="8bcaf-191">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365servicesusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8bcaf-192">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8bcaf-192">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365servicesusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8bcaf-193">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8bcaf-193">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365servicesusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8bcaf-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="8bcaf-194">Response</span></span>

<span data-ttu-id="8bcaf-195">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8bcaf-195">The following is an example of the response.</span></span>

> <span data-ttu-id="8bcaf-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8bcaf-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ServicesUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 458

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365ServicesUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "exchangeActive": 2591, 
      "exchangeInactive": 1426, 
      "oneDriveActive": 1800, 
      "oneDriveInactive": 2451, 
      "sharePointActive": 2286, 
      "sharePointInactive": 1815, 
      "skypeForBusinessActive": 2463, 
      "skypeForBusinessInactive": 1947, 
      "yammerActive": 473, 
      "yammerInactive": 2526, 
      "teamsActive": 846, 
      "teamsInactive": 1960, 
      "office365Active": 2791,
      "office365Inactive": 503,
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
