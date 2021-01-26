---
title: 'reportRoot: getOneDriveActivityUserDetail'
description: Получите сведения о действиях в OneDrive с разбивкой по пользователям.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 1ca242a4c0b653f347ac46d2c6b01435bf1d1d36
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981279"
---
# <a name="reportroot-getonedriveactivityuserdetail"></a><span data-ttu-id="3086b-103">reportRoot: getOneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="3086b-103">reportRoot: getOneDriveActivityUserDetail</span></span>

<span data-ttu-id="3086b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3086b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3086b-105">Получите сведения о действиях в OneDrive с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="3086b-105">Get details about OneDrive activity by user.</span></span>

> <span data-ttu-id="3086b-106">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [отчетах Microsoft 365: действия в OneDrive для бизнеса.](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353)</span><span class="sxs-lookup"><span data-stu-id="3086b-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="permissions"></a><span data-ttu-id="3086b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3086b-107">Permissions</span></span>

<span data-ttu-id="3086b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3086b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3086b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3086b-110">Permission type</span></span>                        | <span data-ttu-id="3086b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3086b-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="3086b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3086b-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="3086b-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3086b-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="3086b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3086b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3086b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3086b-115">Not supported.</span></span>                           |
| <span data-ttu-id="3086b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3086b-116">Application</span></span>                            | <span data-ttu-id="3086b-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3086b-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="3086b-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3086b-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="3086b-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="3086b-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="3086b-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3086b-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveActivityUserDetail(period='{period_value}')
GET /reports/getOneDriveActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="3086b-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="3086b-121">Function parameters</span></span>

<span data-ttu-id="3086b-122">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="3086b-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="3086b-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="3086b-123">Parameter</span></span> | <span data-ttu-id="3086b-124">Тип</span><span class="sxs-lookup"><span data-stu-id="3086b-124">Type</span></span>   | <span data-ttu-id="3086b-125">Описание</span><span class="sxs-lookup"><span data-stu-id="3086b-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="3086b-126">period</span><span class="sxs-lookup"><span data-stu-id="3086b-126">period</span></span>    | <span data-ttu-id="3086b-127">string</span><span class="sxs-lookup"><span data-stu-id="3086b-127">string</span></span> | <span data-ttu-id="3086b-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="3086b-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="3086b-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="3086b-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="3086b-130">Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="3086b-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="3086b-131">date</span><span class="sxs-lookup"><span data-stu-id="3086b-131">date</span></span>      | <span data-ttu-id="3086b-132">Date</span><span class="sxs-lookup"><span data-stu-id="3086b-132">Date</span></span>   | <span data-ttu-id="3086b-133">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="3086b-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="3086b-134">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="3086b-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="3086b-135">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="3086b-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="3086b-136">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="3086b-136">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="3086b-137">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3086b-137">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="3086b-138">Тип выходных данных по умолчанию — text/csv.</span><span class="sxs-lookup"><span data-stu-id="3086b-138">The default output type is text/csv.</span></span> <span data-ttu-id="3086b-139">Однако если требуется указать тип выходных данных, можно использовать параметр запроса OData $format text/csv или application/json.</span><span class="sxs-lookup"><span data-stu-id="3086b-139">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3086b-140">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3086b-140">Request headers</span></span>

| <span data-ttu-id="3086b-141">Имя</span><span class="sxs-lookup"><span data-stu-id="3086b-141">Name</span></span>          | <span data-ttu-id="3086b-142">Описание</span><span class="sxs-lookup"><span data-stu-id="3086b-142">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="3086b-143">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3086b-143">Authorization</span></span> | <span data-ttu-id="3086b-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3086b-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="3086b-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="3086b-146">Response</span></span>

### <a name="csv"></a><span data-ttu-id="3086b-147">CSV</span><span class="sxs-lookup"><span data-stu-id="3086b-147">CSV</span></span>

<span data-ttu-id="3086b-148">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="3086b-148">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="3086b-149">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="3086b-149">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="3086b-150">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="3086b-150">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="3086b-151">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="3086b-151">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="3086b-152">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="3086b-152">Report Refresh Date</span></span>
- <span data-ttu-id="3086b-153">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="3086b-153">User Principal Name</span></span>
- <span data-ttu-id="3086b-154">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="3086b-154">Is Deleted</span></span>
- <span data-ttu-id="3086b-155">"Deleted Date" (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="3086b-155">Deleted Date</span></span>
- <span data-ttu-id="3086b-156">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="3086b-156">Last Activity Date</span></span>
- <span data-ttu-id="3086b-157">"Viewed Or Edited File Count" (Количество просмотренных или измененных файлов);</span><span class="sxs-lookup"><span data-stu-id="3086b-157">Viewed Or Edited File Count</span></span>
- <span data-ttu-id="3086b-158">"Synced File Count" (Количество синхронизированных файлов);</span><span class="sxs-lookup"><span data-stu-id="3086b-158">Synced File Count</span></span>
- <span data-ttu-id="3086b-159">"Shared Internally File Count" (Количество файлов, к которым предоставлен доступ внутренним пользователям);</span><span class="sxs-lookup"><span data-stu-id="3086b-159">Shared Internally File Count</span></span>
- <span data-ttu-id="3086b-160">"Shared Externally File Count" (Количество файлов, к которым предоставлен доступ внешним пользователям);</span><span class="sxs-lookup"><span data-stu-id="3086b-160">Shared Externally File Count</span></span>
- <span data-ttu-id="3086b-161">Assigned Products (назначенные продукты)</span><span class="sxs-lookup"><span data-stu-id="3086b-161">Assigned Products</span></span>
- <span data-ttu-id="3086b-162">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="3086b-162">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="3086b-163">JSON</span><span class="sxs-lookup"><span data-stu-id="3086b-163">JSON</span></span>

<span data-ttu-id="3086b-164">В случае успеха этот метод возвращает код отклика и объект `200 OK` **[oneDriveActivityUserDetail](../resources/onedriveactivityuserdetail.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3086b-164">If successful, this method returns a `200 OK` response code and a **[oneDriveActivityUserDetail](../resources/onedriveactivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="3086b-165">Размер страницы по умолчанию для этого запроса составляет 200 элементов.</span><span class="sxs-lookup"><span data-stu-id="3086b-165">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="3086b-166">Пример</span><span class="sxs-lookup"><span data-stu-id="3086b-166">Example</span></span>

### <a name="csv"></a><span data-ttu-id="3086b-167">CSV</span><span class="sxs-lookup"><span data-stu-id="3086b-167">CSV</span></span>

<span data-ttu-id="3086b-168">Ниже приводится пример вывода CSV-данных.</span><span class="sxs-lookup"><span data-stu-id="3086b-168">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="3086b-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="3086b-169">Request</span></span>

<span data-ttu-id="3086b-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3086b-170">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getonedriveactivityuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOneDriveActivityUserDetail(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="3086b-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="3086b-171">Response</span></span>

<span data-ttu-id="3086b-172">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3086b-172">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="3086b-173">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="3086b-173">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Viewed Or Edited File Count,Synced File Count,Shared Internally File Count,Shared Externally File Count,Assigned Products,Report Period
```

### <a name="json"></a><span data-ttu-id="3086b-174">JSON</span><span class="sxs-lookup"><span data-stu-id="3086b-174">JSON</span></span>

<span data-ttu-id="3086b-175">Ниже приводится пример, который возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="3086b-175">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="3086b-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="3086b-176">Request</span></span>

<span data-ttu-id="3086b-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3086b-177">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getonedriveactivityuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOneDriveActivityUserDetail(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="3086b-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="3086b-178">Response</span></span>

<span data-ttu-id="3086b-179">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3086b-179">The following is an example of the response.</span></span>

> <span data-ttu-id="3086b-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3086b-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oneDriveActivityUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 450

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.oneDriveActivityUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "isDeleted": false, 
      "deletedDate": null, 
      "lastActivityDate": "2017-09-01", 
      "viewedOrEditedFileCount": 1, 
      "syncedFileCount": 0, 
      "sharedInternallyFileCount": 0, 
      "sharedExternallyFileCount": 0, 
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


