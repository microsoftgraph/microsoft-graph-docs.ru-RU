---
title: 'reportRoot: getOffice365ServicesUserCounts'
description: Узнайте, сколько пользователей были активны и неактивны в каждой службе.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 77a715c9a212b214e121f7ccbe6044ebf92a96ca
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35988225"
---
# <a name="reportroot-getoffice365servicesusercounts"></a><span data-ttu-id="6b61f-103">reportRoot: getOffice365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="6b61f-103">reportRoot: getOffice365ServicesUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b61f-104">Узнайте, сколько пользователей были активны и неактивны в каждой службе.</span><span class="sxs-lookup"><span data-stu-id="6b61f-104">Get the count of users by activity type and service.</span></span>

> <span data-ttu-id="6b61f-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: активные пользователи](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="6b61f-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="6b61f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6b61f-106">Permissions</span></span>

<span data-ttu-id="6b61f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b61f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6b61f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6b61f-109">Permission type</span></span>                        | <span data-ttu-id="6b61f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6b61f-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="6b61f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6b61f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6b61f-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6b61f-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="6b61f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6b61f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b61f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b61f-114">Not supported.</span></span>                           |
| <span data-ttu-id="6b61f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6b61f-115">Application</span></span>                            | <span data-ttu-id="6b61f-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6b61f-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="6b61f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6b61f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ServicesUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="6b61f-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="6b61f-118">Function parameters</span></span>

<span data-ttu-id="6b61f-119">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="6b61f-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="6b61f-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="6b61f-120">Parameter</span></span> | <span data-ttu-id="6b61f-121">Тип</span><span class="sxs-lookup"><span data-stu-id="6b61f-121">Type</span></span>   | <span data-ttu-id="6b61f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="6b61f-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="6b61f-123">period</span><span class="sxs-lookup"><span data-stu-id="6b61f-123">period</span></span>    | <span data-ttu-id="6b61f-124">string</span><span class="sxs-lookup"><span data-stu-id="6b61f-124">string</span></span> | <span data-ttu-id="6b61f-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="6b61f-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="6b61f-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="6b61f-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="6b61f-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="6b61f-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="6b61f-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6b61f-128">Required.</span></span> |

<span data-ttu-id="6b61f-129">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="6b61f-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="6b61f-130">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="6b61f-130">The default output type is text/csv.</span></span> <span data-ttu-id="6b61f-131">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="6b61f-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6b61f-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6b61f-132">Request headers</span></span>

| <span data-ttu-id="6b61f-133">Имя</span><span class="sxs-lookup"><span data-stu-id="6b61f-133">Name</span></span>          | <span data-ttu-id="6b61f-134">Описание</span><span class="sxs-lookup"><span data-stu-id="6b61f-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="6b61f-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6b61f-135">Authorization</span></span> | <span data-ttu-id="6b61f-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6b61f-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="6b61f-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b61f-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="6b61f-139">CSV</span><span class="sxs-lookup"><span data-stu-id="6b61f-139">CSV</span></span>

<span data-ttu-id="6b61f-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="6b61f-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="6b61f-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="6b61f-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="6b61f-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="6b61f-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="6b61f-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="6b61f-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="6b61f-144">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="6b61f-144">Report Refresh Date</span></span>
- <span data-ttu-id="6b61f-145">Exchange Active (активны в Exchange)</span><span class="sxs-lookup"><span data-stu-id="6b61f-145">Exchange Active</span></span>
- <span data-ttu-id="6b61f-146">Exchange Inactive (неактивны в Exchange)</span><span class="sxs-lookup"><span data-stu-id="6b61f-146">Exchange Inactive</span></span>
- <span data-ttu-id="6b61f-147">OneDrive Active (активны в OneDrive)</span><span class="sxs-lookup"><span data-stu-id="6b61f-147">OneDrive Active</span></span>
- <span data-ttu-id="6b61f-148">OneDrive Inactive (неактивны в OneDrive)</span><span class="sxs-lookup"><span data-stu-id="6b61f-148">OneDrive Inactive</span></span>
- <span data-ttu-id="6b61f-149">SharePoint Active (активны в SharePoint)</span><span class="sxs-lookup"><span data-stu-id="6b61f-149">SharePoint Active</span></span>
- <span data-ttu-id="6b61f-150">SharePoint Inactive (неактивны в SharePoint)</span><span class="sxs-lookup"><span data-stu-id="6b61f-150">SharePoint Inactive</span></span>
- <span data-ttu-id="6b61f-151">Skype For Business Active (активны в Skype для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="6b61f-151">Skype For Business Active</span></span>
- <span data-ttu-id="6b61f-152">Skype For Business Inactive (неактивны в Skype для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="6b61f-152">Skype For Business Inactive</span></span>
- <span data-ttu-id="6b61f-153">Yammer Active (активны в Yammer)</span><span class="sxs-lookup"><span data-stu-id="6b61f-153">Yammer Active</span></span>
- <span data-ttu-id="6b61f-154">Yammer Inactive (неактивны в Yammer)</span><span class="sxs-lookup"><span data-stu-id="6b61f-154">Yammer Inactive</span></span>
- <span data-ttu-id="6b61f-155">Teams Active (активны в Teams)</span><span class="sxs-lookup"><span data-stu-id="6b61f-155">Teams Active</span></span>
- <span data-ttu-id="6b61f-156">Teams Inactive (неактивны в Teams)</span><span class="sxs-lookup"><span data-stu-id="6b61f-156">Teams Inactive</span></span>
- <span data-ttu-id="6b61f-157">Office 365 активен</span><span class="sxs-lookup"><span data-stu-id="6b61f-157">Office 365 Active</span></span>
- <span data-ttu-id="6b61f-158">Office 365 неактивен</span><span class="sxs-lookup"><span data-stu-id="6b61f-158">Office 365 Inactive</span></span>
- <span data-ttu-id="6b61f-159">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="6b61f-159">Report Period</span></span>

<span data-ttu-id="6b61f-160">Следующие столбцы не поддерживаются в Китае Microsoft Graph, предоставляемом компанией 21Vianet:</span><span class="sxs-lookup"><span data-stu-id="6b61f-160">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="6b61f-161">Yammer Active (активны в Yammer)</span><span class="sxs-lookup"><span data-stu-id="6b61f-161">Yammer Active</span></span>
- <span data-ttu-id="6b61f-162">Yammer Inactive (неактивны в Yammer)</span><span class="sxs-lookup"><span data-stu-id="6b61f-162">Yammer Inactive</span></span>
- <span data-ttu-id="6b61f-163">Teams Active (активны в Teams)</span><span class="sxs-lookup"><span data-stu-id="6b61f-163">Teams Active</span></span>
- <span data-ttu-id="6b61f-164">Teams Inactive (неактивны в Teams)</span><span class="sxs-lookup"><span data-stu-id="6b61f-164">Teams Inactive</span></span>

### <a name="json"></a><span data-ttu-id="6b61f-165">JSON</span><span class="sxs-lookup"><span data-stu-id="6b61f-165">JSON</span></span>

<span data-ttu-id="6b61f-166">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6b61f-166">If successful, this method returns a `200 OK` response code and an **[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** object in the response body.</span></span>

<span data-ttu-id="6b61f-167">Следующие свойства в объекте **[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** не поддерживаются в Китае Microsoft Graph, предоставляемом компанией 21vianet:</span><span class="sxs-lookup"><span data-stu-id="6b61f-167">The following properties in **[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="6b61f-168">Яммерактиве</span><span class="sxs-lookup"><span data-stu-id="6b61f-168">yammerActive</span></span>
- <span data-ttu-id="6b61f-169">Яммеринактиве</span><span class="sxs-lookup"><span data-stu-id="6b61f-169">yammerInactive</span></span>
- <span data-ttu-id="6b61f-170">Теамсактиве</span><span class="sxs-lookup"><span data-stu-id="6b61f-170">teamsActive</span></span>
- <span data-ttu-id="6b61f-171">Теамсинактиве</span><span class="sxs-lookup"><span data-stu-id="6b61f-171">teamsInactive</span></span>

## <a name="example"></a><span data-ttu-id="6b61f-172">Пример</span><span class="sxs-lookup"><span data-stu-id="6b61f-172">Example</span></span>

### <a name="csv"></a><span data-ttu-id="6b61f-173">CSV</span><span class="sxs-lookup"><span data-stu-id="6b61f-173">CSV</span></span>

<span data-ttu-id="6b61f-174">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="6b61f-174">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="6b61f-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="6b61f-175">Request</span></span>

<span data-ttu-id="6b61f-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6b61f-176">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6b61f-177">HTTP</span><span class="sxs-lookup"><span data-stu-id="6b61f-177">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365servicesusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ServicesUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6b61f-178">C#</span><span class="sxs-lookup"><span data-stu-id="6b61f-178">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365servicesusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6b61f-179">Javascript</span><span class="sxs-lookup"><span data-stu-id="6b61f-179">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365servicesusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6b61f-180">Цель — C</span><span class="sxs-lookup"><span data-stu-id="6b61f-180">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365servicesusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6b61f-181">Java</span><span class="sxs-lookup"><span data-stu-id="6b61f-181">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getoffice365servicesusercounts-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6b61f-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b61f-182">Response</span></span>

<span data-ttu-id="6b61f-183">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6b61f-183">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="6b61f-184">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="6b61f-184">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Exchange Active,Exchange Inactive,OneDrive Active,OneDrive Inactive,SharePoint Active,SharePoint Inactive,Skype For Business Active,Skype For Business Inactive,Yammer Active,Yammer Inactive,Teams Active,Teams Inactive,Report Period
```

### <a name="json"></a><span data-ttu-id="6b61f-185">JSON</span><span class="sxs-lookup"><span data-stu-id="6b61f-185">JSON</span></span> 

<span data-ttu-id="6b61f-186">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="6b61f-186">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="6b61f-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="6b61f-187">Request</span></span>

<span data-ttu-id="6b61f-188">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6b61f-188">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6b61f-189">HTTP</span><span class="sxs-lookup"><span data-stu-id="6b61f-189">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365servicesusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ServicesUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6b61f-190">C#</span><span class="sxs-lookup"><span data-stu-id="6b61f-190">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365servicesusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6b61f-191">Javascript</span><span class="sxs-lookup"><span data-stu-id="6b61f-191">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365servicesusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6b61f-192">Цель — C</span><span class="sxs-lookup"><span data-stu-id="6b61f-192">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365servicesusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6b61f-193">Java</span><span class="sxs-lookup"><span data-stu-id="6b61f-193">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getoffice365servicesusercounts-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6b61f-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b61f-194">Response</span></span>

<span data-ttu-id="6b61f-195">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6b61f-195">The following is an example of the response.</span></span>

> <span data-ttu-id="6b61f-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6b61f-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
