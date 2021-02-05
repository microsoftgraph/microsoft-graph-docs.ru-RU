---
title: 'reportRoot: getSharePointSiteUsageDetail'
description: Получение сведений об использовании сайтов SharePoint.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: be28e66a48462ec2bda64c3ae66b1f0cb6059548
ms.sourcegitcommit: 1b01c820be659f85f380fc883bbb36036b7daadf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/05/2021
ms.locfileid: "50115201"
---
# <a name="reportroot-getsharepointsiteusagedetail"></a><span data-ttu-id="d0d01-103">reportRoot: getSharePointSiteUsageDetail</span><span class="sxs-lookup"><span data-stu-id="d0d01-103">reportRoot: getSharePointSiteUsageDetail</span></span>

<span data-ttu-id="d0d01-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0d01-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0d01-105">Получите сведения об использовании сайтов SharePoint.</span><span class="sxs-lookup"><span data-stu-id="d0d01-105">Get details about SharePoint site usage.</span></span>

> <span data-ttu-id="d0d01-106">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [отчетах Microsoft 365 об использовании сайтов SharePoint.](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213)</span><span class="sxs-lookup"><span data-stu-id="d0d01-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="d0d01-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d0d01-107">Permissions</span></span>

<span data-ttu-id="d0d01-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0d01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d0d01-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d0d01-110">Permission type</span></span>                        | <span data-ttu-id="d0d01-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d0d01-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="d0d01-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d0d01-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="d0d01-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d0d01-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="d0d01-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d0d01-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0d01-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0d01-115">Not supported.</span></span>                           |
| <span data-ttu-id="d0d01-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d0d01-116">Application</span></span>                            | <span data-ttu-id="d0d01-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d0d01-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="d0d01-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d0d01-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="d0d01-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="d0d01-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="d0d01-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d0d01-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageDetail(period='{period_value}')
GET /reports/getSharePointSiteUsageDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="d0d01-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="d0d01-121">Function parameters</span></span>

<span data-ttu-id="d0d01-122">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="d0d01-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="d0d01-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="d0d01-123">Parameter</span></span> | <span data-ttu-id="d0d01-124">Тип</span><span class="sxs-lookup"><span data-stu-id="d0d01-124">Type</span></span>   | <span data-ttu-id="d0d01-125">Описание</span><span class="sxs-lookup"><span data-stu-id="d0d01-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="d0d01-126">period</span><span class="sxs-lookup"><span data-stu-id="d0d01-126">period</span></span>    | <span data-ttu-id="d0d01-127">string</span><span class="sxs-lookup"><span data-stu-id="d0d01-127">string</span></span> | <span data-ttu-id="d0d01-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="d0d01-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="d0d01-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="d0d01-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="d0d01-130">Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="d0d01-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="d0d01-131">date</span><span class="sxs-lookup"><span data-stu-id="d0d01-131">date</span></span>      | <span data-ttu-id="d0d01-132">Date</span><span class="sxs-lookup"><span data-stu-id="d0d01-132">Date</span></span>   | <span data-ttu-id="d0d01-133">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="d0d01-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="d0d01-134">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="d0d01-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="d0d01-135">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="d0d01-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="d0d01-136">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="d0d01-136">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="d0d01-137">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d0d01-137">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="d0d01-138">Тип выходных данных по умолчанию — text/csv.</span><span class="sxs-lookup"><span data-stu-id="d0d01-138">The default output type is text/csv.</span></span> <span data-ttu-id="d0d01-139">Однако если требуется указать тип выходных данных, можно использовать параметр запроса OData $format text/csv или application/json.</span><span class="sxs-lookup"><span data-stu-id="d0d01-139">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d0d01-140">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d0d01-140">Request headers</span></span>

| <span data-ttu-id="d0d01-141">Имя</span><span class="sxs-lookup"><span data-stu-id="d0d01-141">Name</span></span>          | <span data-ttu-id="d0d01-142">Описание</span><span class="sxs-lookup"><span data-stu-id="d0d01-142">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="d0d01-143">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d0d01-143">Authorization</span></span> | <span data-ttu-id="d0d01-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d0d01-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="d0d01-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0d01-146">Response</span></span>

### <a name="csv"></a><span data-ttu-id="d0d01-147">CSV</span><span class="sxs-lookup"><span data-stu-id="d0d01-147">CSV</span></span>

<span data-ttu-id="d0d01-148">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="d0d01-148">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d0d01-149">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="d0d01-149">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d0d01-150">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="d0d01-150">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="d0d01-151">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="d0d01-151">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="d0d01-152">Report Refresh Date (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="d0d01-152">Report Refresh Date</span></span>
- <span data-ttu-id="d0d01-153">ИД сайта</span><span class="sxs-lookup"><span data-stu-id="d0d01-153">Site Id</span></span>
- <span data-ttu-id="d0d01-154">"Site URL" (URL-адрес сайта);</span><span class="sxs-lookup"><span data-stu-id="d0d01-154">Site URL</span></span>
- <span data-ttu-id="d0d01-155">"Owner Display Name" (Отображаемое имя владельца);</span><span class="sxs-lookup"><span data-stu-id="d0d01-155">Owner Display Name</span></span>
- <span data-ttu-id="d0d01-156">Is Deleted (удален)</span><span class="sxs-lookup"><span data-stu-id="d0d01-156">Is Deleted</span></span>
- <span data-ttu-id="d0d01-157">"Last Activity Date" (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="d0d01-157">Last Activity Date</span></span>
- <span data-ttu-id="d0d01-158">ИД метки конфиденциальности сайта</span><span class="sxs-lookup"><span data-stu-id="d0d01-158">Site Sensitivity Label Id</span></span>
- <span data-ttu-id="d0d01-159">Внешний общий доступ</span><span class="sxs-lookup"><span data-stu-id="d0d01-159">External Sharing</span></span>
- <span data-ttu-id="d0d01-160">Неугодная политика устройств</span><span class="sxs-lookup"><span data-stu-id="d0d01-160">Unmanaged Device Policy</span></span>
- <span data-ttu-id="d0d01-161">Географическое расположение</span><span class="sxs-lookup"><span data-stu-id="d0d01-161">Geo Location</span></span>
- <span data-ttu-id="d0d01-162">"File Count" (Количество файлов);</span><span class="sxs-lookup"><span data-stu-id="d0d01-162">File Count</span></span>
- <span data-ttu-id="d0d01-163">"Active File Count" (Количество активных файлов);</span><span class="sxs-lookup"><span data-stu-id="d0d01-163">Active File Count</span></span>
- <span data-ttu-id="d0d01-164">"Page View Count" (Количество просмотров страницы);</span><span class="sxs-lookup"><span data-stu-id="d0d01-164">Page View Count</span></span>
- <span data-ttu-id="d0d01-165">"Visited Page Count" (Количество посещенных страниц);</span><span class="sxs-lookup"><span data-stu-id="d0d01-165">Visited Page Count</span></span>
- <span data-ttu-id="d0d01-166">Anonymous Link Count</span><span class="sxs-lookup"><span data-stu-id="d0d01-166">Anonymous Link Count</span></span>
- <span data-ttu-id="d0d01-167">Company Link Count</span><span class="sxs-lookup"><span data-stu-id="d0d01-167">Company Link Count</span></span>
- <span data-ttu-id="d0d01-168">Безопасная ссылка для подсчета гостей</span><span class="sxs-lookup"><span data-stu-id="d0d01-168">Secure Link For Guest Count</span></span>
- <span data-ttu-id="d0d01-169">Безопасная ссылка для подсчета членов</span><span class="sxs-lookup"><span data-stu-id="d0d01-169">Secure Link For Member Count</span></span>
- <span data-ttu-id="d0d01-170">Storage Used (Byte) [использовано (байт)]</span><span class="sxs-lookup"><span data-stu-id="d0d01-170">Storage Used (Byte)</span></span>
- <span data-ttu-id="d0d01-171">"Storage Allocated (Byte)" (Объем выделенного хранилища в байтах);</span><span class="sxs-lookup"><span data-stu-id="d0d01-171">Storage Allocated (Byte)</span></span>
- <span data-ttu-id="d0d01-172">"Root Web Template" (Шаблон корневого веб-сайта);</span><span class="sxs-lookup"><span data-stu-id="d0d01-172">Root Web Template</span></span>
- <span data-ttu-id="d0d01-173">Owner Principal Name (имя участника-владельца)</span><span class="sxs-lookup"><span data-stu-id="d0d01-173">Owner Principal Name</span></span>
- <span data-ttu-id="d0d01-174">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="d0d01-174">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="d0d01-175">JSON</span><span class="sxs-lookup"><span data-stu-id="d0d01-175">JSON</span></span>

<span data-ttu-id="d0d01-176">В случае успеха этот метод возвращает код отклика и объект `200 OK` **[sharePointSiteUsageDetail](../resources/sharepointsiteusagedetail.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d0d01-176">If successful, this method returns a `200 OK` response code and a **[sharePointSiteUsageDetail](../resources/sharepointsiteusagedetail.md)** object in the response body.</span></span>

<span data-ttu-id="d0d01-177">Размер страницы по умолчанию для этого запроса составляет 200 элементов.</span><span class="sxs-lookup"><span data-stu-id="d0d01-177">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="d0d01-178">Пример</span><span class="sxs-lookup"><span data-stu-id="d0d01-178">Example</span></span>

### <a name="csv"></a><span data-ttu-id="d0d01-179">CSV</span><span class="sxs-lookup"><span data-stu-id="d0d01-179">CSV</span></span>

<span data-ttu-id="d0d01-180">Ниже приводится пример вывода CSV-данных.</span><span class="sxs-lookup"><span data-stu-id="d0d01-180">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="d0d01-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="d0d01-181">Request</span></span>

<span data-ttu-id="d0d01-182">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d0d01-182">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getsharepointsiteusagedetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageDetail(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="d0d01-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0d01-183">Response</span></span>

<span data-ttu-id="d0d01-184">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d0d01-184">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="d0d01-185">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="d0d01-185">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Id,Site URL,Owner Display Name,Is Deleted,Last Activity Date,Site Sensitivity Label Id,External Sharing,Unmanaged Device Policy,Geo Location,File Count,Active File Count,Page View Count,Visited Page Count,Anonymous Link Count,Company Link Count,Secure Link For Guest Count,Secure Link For Member Count,Storage Used (Byte),Storage Allocated (Byte),Root Web Template,Owner Principal Name,Report Period
```

### <a name="json"></a><span data-ttu-id="d0d01-186">JSON</span><span class="sxs-lookup"><span data-stu-id="d0d01-186">JSON</span></span>

<span data-ttu-id="d0d01-187">Ниже приводится пример, который возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="d0d01-187">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="d0d01-188">Запрос</span><span class="sxs-lookup"><span data-stu-id="d0d01-188">Request</span></span>

<span data-ttu-id="d0d01-189">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d0d01-189">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getsharepointsiteusagedetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageDetail(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="d0d01-190">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0d01-190">Response</span></span>

<span data-ttu-id="d0d01-191">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d0d01-191">The following is an example of the response.</span></span>

> <span data-ttu-id="d0d01-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d0d01-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointSiteUsageDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 484

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.sharePointSiteUsageDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteId": "siteId-value", 
      "siteUrl": "siteUrl-value", 
      "ownerDisplayName": "ownerDisplayName-value", 
      "ownerPrincipalName": "ownerPrincipalName-value", 
      "isDeleted": false, 
      "lastActivityDate": "2017-09-01", 
      "SiteSensitivityLabelId": "SiteSensitivityLabelId-value",
      "ExternalSharing": false,
      "UnmanagedDevicePolicy": "UnmanagedDevicePolicy-value",
      "GeoLocation": "GeoLocation-value",
      "fileCount": 170, 
      "activeFileCount": 25, 
      "pageViewCount": 7, 
      "visitedPageCount": 3, 
      "AnonymousLinkCount": 5,
      "CompanyLinkCount": 8,
      "SecureLinkForGuestCount": 13,
      "SecureLinkForMemberCount": 11,
      "storageUsedInBytes": 63442116, 
      "storageAllocatedInBytes": 2748779094400, 
      "rootWebTemplate": "Publishing Site", 
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


