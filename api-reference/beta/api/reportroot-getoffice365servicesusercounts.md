---
title: 'reportRoot: getOffice365ServicesUserCounts'
description: Узнайте, сколько пользователей были активны и неактивны в каждой службе.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: e3c57848f2295c9854d00da828c1c4ad844fce9e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052014"
---
# <a name="reportroot-getoffice365servicesusercounts"></a><span data-ttu-id="89dc9-103">reportRoot: getOffice365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="89dc9-103">reportRoot: getOffice365ServicesUserCounts</span></span>

<span data-ttu-id="89dc9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89dc9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89dc9-105">Узнайте, сколько пользователей были активны и неактивны в каждой службе.</span><span class="sxs-lookup"><span data-stu-id="89dc9-105">Get the count of users by activity type and service.</span></span>

> <span data-ttu-id="89dc9-106">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты Microsoft 365 — Активные Пользователи](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="89dc9-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="89dc9-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="89dc9-107">Permissions</span></span>

<span data-ttu-id="89dc9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89dc9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="89dc9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="89dc9-110">Permission type</span></span>                        | <span data-ttu-id="89dc9-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="89dc9-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="89dc9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="89dc9-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="89dc9-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="89dc9-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="89dc9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="89dc9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89dc9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89dc9-115">Not supported.</span></span>                           |
| <span data-ttu-id="89dc9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="89dc9-116">Application</span></span>                            | <span data-ttu-id="89dc9-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="89dc9-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="89dc9-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="89dc9-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="89dc9-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="89dc9-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="89dc9-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="89dc9-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ServicesUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="89dc9-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="89dc9-121">Function parameters</span></span>

<span data-ttu-id="89dc9-122">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="89dc9-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="89dc9-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="89dc9-123">Parameter</span></span> | <span data-ttu-id="89dc9-124">Тип</span><span class="sxs-lookup"><span data-stu-id="89dc9-124">Type</span></span>   | <span data-ttu-id="89dc9-125">Описание</span><span class="sxs-lookup"><span data-stu-id="89dc9-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="89dc9-126">period</span><span class="sxs-lookup"><span data-stu-id="89dc9-126">period</span></span>    | <span data-ttu-id="89dc9-127">string</span><span class="sxs-lookup"><span data-stu-id="89dc9-127">string</span></span> | <span data-ttu-id="89dc9-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="89dc9-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="89dc9-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="89dc9-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="89dc9-130">Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="89dc9-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="89dc9-131">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="89dc9-131">Required.</span></span> |

<span data-ttu-id="89dc9-132">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="89dc9-132">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="89dc9-133">Тип вывода по умолчанию — текст/csv.</span><span class="sxs-lookup"><span data-stu-id="89dc9-133">The default output type is text/csv.</span></span> <span data-ttu-id="89dc9-134">Однако, если требуется указать тип вывода, можно использовать параметр OData $format для параметра text/csv или application/json.</span><span class="sxs-lookup"><span data-stu-id="89dc9-134">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="89dc9-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="89dc9-135">Request headers</span></span>

| <span data-ttu-id="89dc9-136">Имя</span><span class="sxs-lookup"><span data-stu-id="89dc9-136">Name</span></span>          | <span data-ttu-id="89dc9-137">Описание</span><span class="sxs-lookup"><span data-stu-id="89dc9-137">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="89dc9-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="89dc9-138">Authorization</span></span> | <span data-ttu-id="89dc9-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="89dc9-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="89dc9-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="89dc9-141">Response</span></span>

### <a name="csv"></a><span data-ttu-id="89dc9-142">CSV</span><span class="sxs-lookup"><span data-stu-id="89dc9-142">CSV</span></span>

<span data-ttu-id="89dc9-143">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="89dc9-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="89dc9-144">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="89dc9-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="89dc9-145">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="89dc9-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="89dc9-146">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="89dc9-146">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="89dc9-147">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="89dc9-147">Report Refresh Date</span></span>
- <span data-ttu-id="89dc9-148">Exchange Active (активны в Exchange)</span><span class="sxs-lookup"><span data-stu-id="89dc9-148">Exchange Active</span></span>
- <span data-ttu-id="89dc9-149">Exchange Inactive (неактивны в Exchange)</span><span class="sxs-lookup"><span data-stu-id="89dc9-149">Exchange Inactive</span></span>
- <span data-ttu-id="89dc9-150">OneDrive Active (активны в OneDrive)</span><span class="sxs-lookup"><span data-stu-id="89dc9-150">OneDrive Active</span></span>
- <span data-ttu-id="89dc9-151">OneDrive Inactive (неактивны в OneDrive)</span><span class="sxs-lookup"><span data-stu-id="89dc9-151">OneDrive Inactive</span></span>
- <span data-ttu-id="89dc9-152">SharePoint Active (активны в SharePoint)</span><span class="sxs-lookup"><span data-stu-id="89dc9-152">SharePoint Active</span></span>
- <span data-ttu-id="89dc9-153">SharePoint Inactive (неактивны в SharePoint)</span><span class="sxs-lookup"><span data-stu-id="89dc9-153">SharePoint Inactive</span></span>
- <span data-ttu-id="89dc9-154">Skype For Business Active (активны в Skype для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="89dc9-154">Skype For Business Active</span></span>
- <span data-ttu-id="89dc9-155">Skype For Business Inactive (неактивны в Skype для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="89dc9-155">Skype For Business Inactive</span></span>
- <span data-ttu-id="89dc9-156">Yammer Active (активны в Yammer)</span><span class="sxs-lookup"><span data-stu-id="89dc9-156">Yammer Active</span></span>
- <span data-ttu-id="89dc9-157">Yammer Inactive (неактивны в Yammer)</span><span class="sxs-lookup"><span data-stu-id="89dc9-157">Yammer Inactive</span></span>
- <span data-ttu-id="89dc9-158">Teams Active (активны в Teams)</span><span class="sxs-lookup"><span data-stu-id="89dc9-158">Teams Active</span></span>
- <span data-ttu-id="89dc9-159">Teams Inactive (неактивны в Teams)</span><span class="sxs-lookup"><span data-stu-id="89dc9-159">Teams Inactive</span></span>
- <span data-ttu-id="89dc9-160">Office 365 Active</span><span class="sxs-lookup"><span data-stu-id="89dc9-160">Office 365 Active</span></span>
- <span data-ttu-id="89dc9-161">Office 365 Неактивный</span><span class="sxs-lookup"><span data-stu-id="89dc9-161">Office 365 Inactive</span></span>
- <span data-ttu-id="89dc9-162">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="89dc9-162">Report Period</span></span>

<span data-ttu-id="89dc9-163">Следующие столбцы не поддерживаются в Microsoft Graph Китае, выполняемых 21Vianet:</span><span class="sxs-lookup"><span data-stu-id="89dc9-163">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="89dc9-164">Yammer Active (активны в Yammer)</span><span class="sxs-lookup"><span data-stu-id="89dc9-164">Yammer Active</span></span>
- <span data-ttu-id="89dc9-165">Yammer Inactive (неактивны в Yammer)</span><span class="sxs-lookup"><span data-stu-id="89dc9-165">Yammer Inactive</span></span>
- <span data-ttu-id="89dc9-166">Teams Active (активны в Teams)</span><span class="sxs-lookup"><span data-stu-id="89dc9-166">Teams Active</span></span>
- <span data-ttu-id="89dc9-167">Teams Inactive (неактивны в Teams)</span><span class="sxs-lookup"><span data-stu-id="89dc9-167">Teams Inactive</span></span>

### <a name="json"></a><span data-ttu-id="89dc9-168">JSON</span><span class="sxs-lookup"><span data-stu-id="89dc9-168">JSON</span></span>

<span data-ttu-id="89dc9-169">В случае успешной работы этот метод возвращает код отклика и `200 OK` **[объект Office365ServicesUserCounts](../resources/office365servicesusercounts.md)** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="89dc9-169">If successful, this method returns a `200 OK` response code and an **[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** object in the response body.</span></span>

<span data-ttu-id="89dc9-170">Следующие свойства в **[объекте Office365ServicesUserCounts](../resources/office365servicesusercounts.md)** не поддерживаются в Microsoft Graph Китае под управлением 21Vianet:</span><span class="sxs-lookup"><span data-stu-id="89dc9-170">The following properties in **[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="89dc9-171">yammerActive</span><span class="sxs-lookup"><span data-stu-id="89dc9-171">yammerActive</span></span>
- <span data-ttu-id="89dc9-172">yammerInactive</span><span class="sxs-lookup"><span data-stu-id="89dc9-172">yammerInactive</span></span>
- <span data-ttu-id="89dc9-173">teamsActive</span><span class="sxs-lookup"><span data-stu-id="89dc9-173">teamsActive</span></span>
- <span data-ttu-id="89dc9-174">teamsInactive</span><span class="sxs-lookup"><span data-stu-id="89dc9-174">teamsInactive</span></span>

## <a name="example"></a><span data-ttu-id="89dc9-175">Пример</span><span class="sxs-lookup"><span data-stu-id="89dc9-175">Example</span></span>

### <a name="csv"></a><span data-ttu-id="89dc9-176">CSV</span><span class="sxs-lookup"><span data-stu-id="89dc9-176">CSV</span></span>

<span data-ttu-id="89dc9-177">Ниже приводится пример, который выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="89dc9-177">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="89dc9-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="89dc9-178">Request</span></span>

<span data-ttu-id="89dc9-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="89dc9-179">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getoffice365servicesusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ServicesUserCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="89dc9-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="89dc9-180">Response</span></span>

<span data-ttu-id="89dc9-181">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="89dc9-181">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="89dc9-182">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="89dc9-182">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="89dc9-183">JSON</span><span class="sxs-lookup"><span data-stu-id="89dc9-183">JSON</span></span> 

<span data-ttu-id="89dc9-184">Ниже приводится пример, который возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="89dc9-184">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="89dc9-185">Запрос</span><span class="sxs-lookup"><span data-stu-id="89dc9-185">Request</span></span>

<span data-ttu-id="89dc9-186">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="89dc9-186">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getoffice365servicesusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ServicesUserCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="89dc9-187">Отклик</span><span class="sxs-lookup"><span data-stu-id="89dc9-187">Response</span></span>

<span data-ttu-id="89dc9-188">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="89dc9-188">The following is an example of the response.</span></span>

> <span data-ttu-id="89dc9-189">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="89dc9-189">**Note:** The response object shown here might be shortened for readability.</span></span>

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


