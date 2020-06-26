---
title: 'reportRoot: getSharePointActivityUserDetail'
description: Получите сведения об активности пользователей в SharePoint.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 8af4d7e961b8c36dddd71e3730e956bad2369762
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896261"
---
# <a name="reportroot-getsharepointactivityuserdetail"></a><span data-ttu-id="ee547-103">reportRoot: getSharePointActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="ee547-103">reportRoot: getSharePointActivityUserDetail</span></span>

<span data-ttu-id="ee547-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee547-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee547-105">Получите сведения о действиях в SharePoint с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="ee547-105">Get details about SharePoint activity by user.</span></span>

> <span data-ttu-id="ee547-106">**Примечание:** Сведения о различных представлениях отчетов и их именах можно найти в [статье Microsoft 365 Reports-SharePoint Activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="ee547-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="ee547-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ee547-107">Permissions</span></span>

<span data-ttu-id="ee547-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="ee547-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="ee547-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee547-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ee547-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ee547-110">Permission type</span></span>                        | <span data-ttu-id="ee547-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ee547-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ee547-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ee547-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="ee547-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee547-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ee547-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ee547-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee547-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee547-115">Not supported.</span></span>                           |
| <span data-ttu-id="ee547-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ee547-116">Application</span></span>                            | <span data-ttu-id="ee547-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee547-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="ee547-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ee547-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="ee547-119">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="ee547-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="ee547-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ee547-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityUserDetail(period='{period_value}')
GET /reports/getSharePointActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="ee547-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="ee547-121">Function parameters</span></span>

<span data-ttu-id="ee547-122">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="ee547-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="ee547-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="ee547-123">Parameter</span></span> | <span data-ttu-id="ee547-124">Тип</span><span class="sxs-lookup"><span data-stu-id="ee547-124">Type</span></span>   | <span data-ttu-id="ee547-125">Описание</span><span class="sxs-lookup"><span data-stu-id="ee547-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="ee547-126">period</span><span class="sxs-lookup"><span data-stu-id="ee547-126">period</span></span>    | <span data-ttu-id="ee547-127">string</span><span class="sxs-lookup"><span data-stu-id="ee547-127">string</span></span> | <span data-ttu-id="ee547-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="ee547-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="ee547-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="ee547-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="ee547-130">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="ee547-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="ee547-131">date</span><span class="sxs-lookup"><span data-stu-id="ee547-131">date</span></span>      | <span data-ttu-id="ee547-132">Date</span><span class="sxs-lookup"><span data-stu-id="ee547-132">Date</span></span>   | <span data-ttu-id="ee547-133">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="ee547-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="ee547-134">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="ee547-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="ee547-135">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="ee547-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="ee547-136">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="ee547-136">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="ee547-137">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ee547-137">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="ee547-138">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="ee547-138">The default output type is text/csv.</span></span> <span data-ttu-id="ee547-139">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="ee547-139">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ee547-140">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ee547-140">Request headers</span></span>

| <span data-ttu-id="ee547-141">Имя</span><span class="sxs-lookup"><span data-stu-id="ee547-141">Name</span></span>          | <span data-ttu-id="ee547-142">Описание</span><span class="sxs-lookup"><span data-stu-id="ee547-142">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="ee547-143">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ee547-143">Authorization</span></span> | <span data-ttu-id="ee547-144">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="ee547-144">Bearer {token}.</span></span> <span data-ttu-id="ee547-145">Required.</span><span class="sxs-lookup"><span data-stu-id="ee547-145">Required.</span></span> |

## <a name="response"></a><span data-ttu-id="ee547-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee547-146">Response</span></span>

### <a name="csv"></a><span data-ttu-id="ee547-147">CSV</span><span class="sxs-lookup"><span data-stu-id="ee547-147">CSV</span></span>

<span data-ttu-id="ee547-148">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="ee547-148">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ee547-149">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="ee547-149">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ee547-150">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="ee547-150">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ee547-151">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="ee547-151">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="ee547-152">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="ee547-152">Report Refresh Date</span></span>
- <span data-ttu-id="ee547-153">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="ee547-153">User Principal Name</span></span>
- <span data-ttu-id="ee547-154">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="ee547-154">Is Deleted</span></span>
- <span data-ttu-id="ee547-155">"Deleted Date" (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="ee547-155">Deleted Date</span></span>
- <span data-ttu-id="ee547-156">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="ee547-156">Last Activity Date</span></span>
- <span data-ttu-id="ee547-157">"Viewed Or Edited File Count" (Количество просмотренных или измененных файлов);</span><span class="sxs-lookup"><span data-stu-id="ee547-157">Viewed Or Edited File Count</span></span>
- <span data-ttu-id="ee547-158">"Synced File Count" (Количество синхронизированных файлов);</span><span class="sxs-lookup"><span data-stu-id="ee547-158">Synced File Count</span></span>
- <span data-ttu-id="ee547-159">"Shared Internally File Count" (Количество файлов, к которым предоставлен доступ внутренним пользователям);</span><span class="sxs-lookup"><span data-stu-id="ee547-159">Shared Internally File Count</span></span>
- <span data-ttu-id="ee547-160">Shared Externally File Count (количество файлов, отправленных за пределы организации)</span><span class="sxs-lookup"><span data-stu-id="ee547-160">Shared Externally File Count</span></span>
- <span data-ttu-id="ee547-161">Visited Page Count (количество посещенных страниц)</span><span class="sxs-lookup"><span data-stu-id="ee547-161">Visited Page Count</span></span>
- <span data-ttu-id="ee547-162">Assigned Products (назначенные продукты)</span><span class="sxs-lookup"><span data-stu-id="ee547-162">Assigned Products</span></span>
- <span data-ttu-id="ee547-163">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="ee547-163">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="ee547-164">JSON</span><span class="sxs-lookup"><span data-stu-id="ee547-164">JSON</span></span>

<span data-ttu-id="ee547-165">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[шарепоинтактивитюсердетаил](../resources/sharepointactivityuserdetail.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ee547-165">If successful, this method returns a `200 OK` response code and a **[sharePointActivityUserDetail](../resources/sharepointactivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="ee547-166">Размер страницы по умолчанию для этого запроса составляет 200 элементов.</span><span class="sxs-lookup"><span data-stu-id="ee547-166">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="ee547-167">Пример</span><span class="sxs-lookup"><span data-stu-id="ee547-167">Example</span></span>

### <a name="csv"></a><span data-ttu-id="ee547-168">CSV</span><span class="sxs-lookup"><span data-stu-id="ee547-168">CSV</span></span>

<span data-ttu-id="ee547-169">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="ee547-169">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="ee547-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="ee547-170">Request</span></span>

<span data-ttu-id="ee547-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ee547-171">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getsharepointactivityuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserDetail(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="ee547-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee547-172">Response</span></span>

<span data-ttu-id="ee547-173">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ee547-173">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="ee547-174">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="ee547-174">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Viewed Or Edited File Count,Synced File Count,Shared Internally File Count,Shared Externally File Count,Visited Page Count,Assigned Products,Report Period
```

### <a name="json"></a><span data-ttu-id="ee547-175">JSON</span><span class="sxs-lookup"><span data-stu-id="ee547-175">JSON</span></span>

<span data-ttu-id="ee547-176">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="ee547-176">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="ee547-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="ee547-177">Request</span></span>

<span data-ttu-id="ee547-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ee547-178">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getsharepointactivityuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserDetail(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="ee547-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee547-179">Response</span></span>

<span data-ttu-id="ee547-180">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ee547-180">The following is an example of the response.</span></span>

> <span data-ttu-id="ee547-181">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="ee547-181">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ee547-182">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="ee547-182">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointActivityUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 473

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.sharePointActivityUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "isDeleted": false, 
      "deletedDate": null, 
      "lastActivityDate": "2017-09-01", 
      "viewedOrEditedFileCount": 4, 
      "syncedFileCount": 0, 
      "sharedInternallyFileCount": 0, 
      "sharedExternallyFileCount": 0, 
      "visitedPageCount": 1, 
      "assignedProducts": [
        "Microsoft 365 ENTERPRISE E5"
      ], 
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
