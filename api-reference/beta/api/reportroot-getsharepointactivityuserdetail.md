---
title: 'reportRoot: getSharePointActivityUserDetail'
description: Получите сведения об активности пользователей в SharePoint.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: af63d1b995dd182ce37b0f39b6a0533c25f56f3d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521854"
---
# <a name="reportroot-getsharepointactivityuserdetail"></a><span data-ttu-id="898e5-103">reportRoot: getSharePointActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="898e5-103">reportRoot: getSharePointActivityUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="898e5-104">Получите сведения об активности пользователей в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="898e5-104">Get details about SharePoint activity by user.</span></span>

> <span data-ttu-id="898e5-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="898e5-105">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="898e5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="898e5-106">Permissions</span></span>

<span data-ttu-id="898e5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="898e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="898e5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="898e5-109">Permission type</span></span>                        | <span data-ttu-id="898e5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="898e5-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="898e5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="898e5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="898e5-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="898e5-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="898e5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="898e5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="898e5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="898e5-114">Not supported.</span></span>                           |
| <span data-ttu-id="898e5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="898e5-115">Application</span></span>                            | <span data-ttu-id="898e5-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="898e5-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="898e5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="898e5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityUserDetail(period='{period_value}')
GET /reports/getSharePointActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="898e5-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="898e5-118">Function parameters</span></span>

<span data-ttu-id="898e5-119">В URL-адресе запроса укажите один из следующих параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="898e5-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="898e5-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="898e5-120">Parameter</span></span> | <span data-ttu-id="898e5-121">Тип</span><span class="sxs-lookup"><span data-stu-id="898e5-121">Type</span></span>   | <span data-ttu-id="898e5-122">Описание</span><span class="sxs-lookup"><span data-stu-id="898e5-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="898e5-123">period</span><span class="sxs-lookup"><span data-stu-id="898e5-123">period</span></span>    | <span data-ttu-id="898e5-124">строка</span><span class="sxs-lookup"><span data-stu-id="898e5-124">string</span></span> | <span data-ttu-id="898e5-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="898e5-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="898e5-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="898e5-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="898e5-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="898e5-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="898e5-128">date</span><span class="sxs-lookup"><span data-stu-id="898e5-128">date</span></span>      | <span data-ttu-id="898e5-129">Date</span><span class="sxs-lookup"><span data-stu-id="898e5-129">Date</span></span>   | <span data-ttu-id="898e5-130">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="898e5-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="898e5-131">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="898e5-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="898e5-132">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="898e5-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="898e5-133">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="898e5-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="898e5-134">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="898e5-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="898e5-135">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="898e5-135">The default output type is text/csv.</span></span> <span data-ttu-id="898e5-136">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="898e5-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="898e5-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="898e5-137">Request headers</span></span>

| <span data-ttu-id="898e5-138">Имя</span><span class="sxs-lookup"><span data-stu-id="898e5-138">Name</span></span>          | <span data-ttu-id="898e5-139">Описание</span><span class="sxs-lookup"><span data-stu-id="898e5-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="898e5-140">Авторизация</span><span class="sxs-lookup"><span data-stu-id="898e5-140">Authorization</span></span> | <span data-ttu-id="898e5-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="898e5-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="898e5-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="898e5-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="898e5-144">CSV</span><span class="sxs-lookup"><span data-stu-id="898e5-144">CSV</span></span>

<span data-ttu-id="898e5-145">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="898e5-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="898e5-146">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="898e5-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="898e5-147">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="898e5-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="898e5-148">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="898e5-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="898e5-149">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="898e5-149">Report Refresh Date</span></span>
- <span data-ttu-id="898e5-150">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="898e5-150">User Principal Name</span></span>
- <span data-ttu-id="898e5-151">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="898e5-151">Is Deleted</span></span>
- <span data-ttu-id="898e5-152">"Deleted Date" (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="898e5-152">Deleted Date</span></span>
- <span data-ttu-id="898e5-153">"Last Activity Date" (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="898e5-153">Last Activity Date</span></span>
- <span data-ttu-id="898e5-154">"Viewed Or Edited File Count" (Количество просмотренных или измененных файлов);</span><span class="sxs-lookup"><span data-stu-id="898e5-154">Viewed Or Edited File Count</span></span>
- <span data-ttu-id="898e5-155">"Synced File Count" (Количество синхронизированных файлов);</span><span class="sxs-lookup"><span data-stu-id="898e5-155">Synced File Count</span></span>
- <span data-ttu-id="898e5-156">"Shared Internally File Count" (Количество файлов, к которым предоставлен доступ внутренним пользователям);</span><span class="sxs-lookup"><span data-stu-id="898e5-156">Shared Internally File Count</span></span>
- <span data-ttu-id="898e5-157">Shared Externally File Count (количество файлов, отправленных за пределы организации)</span><span class="sxs-lookup"><span data-stu-id="898e5-157">Shared Externally File Count</span></span>
- <span data-ttu-id="898e5-158">Visited Page Count (количество посещенных страниц)</span><span class="sxs-lookup"><span data-stu-id="898e5-158">Visited Page Count</span></span>
- <span data-ttu-id="898e5-159">Assigned Products (назначенные продукты)</span><span class="sxs-lookup"><span data-stu-id="898e5-159">Assigned Products</span></span>
- <span data-ttu-id="898e5-160">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="898e5-160">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="898e5-161">JSON</span><span class="sxs-lookup"><span data-stu-id="898e5-161">JSON</span></span>

<span data-ttu-id="898e5-162">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[sharePointActivityUserDetail](../resources/sharepointactivityuserdetail.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="898e5-162">If successful, this method returns a `200 OK` response code and a **[sharePointActivityUserDetail](../resources/sharepointactivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="898e5-163">Размер страницы по умолчанию для этого запроса — 200 элементов.</span><span class="sxs-lookup"><span data-stu-id="898e5-163">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="898e5-164">Пример</span><span class="sxs-lookup"><span data-stu-id="898e5-164">Example</span></span>

### <a name="csv"></a><span data-ttu-id="898e5-165">CSV</span><span class="sxs-lookup"><span data-stu-id="898e5-165">CSV</span></span>

<span data-ttu-id="898e5-166">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="898e5-166">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="898e5-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="898e5-167">Request</span></span>

<span data-ttu-id="898e5-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="898e5-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="898e5-169">Ответ</span><span class="sxs-lookup"><span data-stu-id="898e5-169">Response</span></span>

<span data-ttu-id="898e5-170">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="898e5-170">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="898e5-171">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="898e5-171">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="898e5-172">JSON</span><span class="sxs-lookup"><span data-stu-id="898e5-172">JSON</span></span>

<span data-ttu-id="898e5-173">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="898e5-173">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="898e5-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="898e5-174">Request</span></span>

<span data-ttu-id="898e5-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="898e5-175">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="898e5-176">Ответ</span><span class="sxs-lookup"><span data-stu-id="898e5-176">Response</span></span>

<span data-ttu-id="898e5-177">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="898e5-177">The following is an example of the response.</span></span>

> <span data-ttu-id="898e5-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="898e5-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
        "OFFICE 365 ENTERPRISE E5"
      ], 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getsharepointactivityuserdetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
