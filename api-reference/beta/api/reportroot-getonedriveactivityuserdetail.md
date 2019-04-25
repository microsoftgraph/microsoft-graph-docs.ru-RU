---
title: 'reportRoot: getOneDriveActivityUserDetail'
description: Получите сведения о действиях в OneDrive с разбивкой по пользователям.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 40b4d5485998ebc39d541977c56c2afaef203819
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32538156"
---
# <a name="reportroot-getonedriveactivityuserdetail"></a><span data-ttu-id="dc0a8-103">reportRoot: getOneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="dc0a8-103">reportRoot: getOneDriveActivityUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc0a8-104">Получите сведения о действиях в OneDrive с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="dc0a8-104">Get details about OneDrive activity by user.</span></span>

> <span data-ttu-id="dc0a8-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия в OneDrive для бизнеса](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span><span class="sxs-lookup"><span data-stu-id="dc0a8-105">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="permissions"></a><span data-ttu-id="dc0a8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dc0a8-106">Permissions</span></span>

<span data-ttu-id="dc0a8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc0a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dc0a8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dc0a8-109">Permission type</span></span>                        | <span data-ttu-id="dc0a8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dc0a8-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="dc0a8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dc0a8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="dc0a8-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="dc0a8-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="dc0a8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dc0a8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc0a8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc0a8-114">Not supported.</span></span>                           |
| <span data-ttu-id="dc0a8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dc0a8-115">Application</span></span>                            | <span data-ttu-id="dc0a8-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="dc0a8-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="dc0a8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dc0a8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveActivityUserDetail(period='{period_value}')
GET /reports/getOneDriveActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="dc0a8-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="dc0a8-118">Function parameters</span></span>

<span data-ttu-id="dc0a8-119">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="dc0a8-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="dc0a8-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="dc0a8-120">Parameter</span></span> | <span data-ttu-id="dc0a8-121">Тип</span><span class="sxs-lookup"><span data-stu-id="dc0a8-121">Type</span></span>   | <span data-ttu-id="dc0a8-122">Описание</span><span class="sxs-lookup"><span data-stu-id="dc0a8-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="dc0a8-123">period</span><span class="sxs-lookup"><span data-stu-id="dc0a8-123">period</span></span>    | <span data-ttu-id="dc0a8-124">string</span><span class="sxs-lookup"><span data-stu-id="dc0a8-124">string</span></span> | <span data-ttu-id="dc0a8-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="dc0a8-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="dc0a8-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="dc0a8-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="dc0a8-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="dc0a8-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="dc0a8-128">date</span><span class="sxs-lookup"><span data-stu-id="dc0a8-128">date</span></span>      | <span data-ttu-id="dc0a8-129">Date</span><span class="sxs-lookup"><span data-stu-id="dc0a8-129">Date</span></span>   | <span data-ttu-id="dc0a8-130">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="dc0a8-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="dc0a8-131">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="dc0a8-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="dc0a8-132">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="dc0a8-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="dc0a8-133">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="dc0a8-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="dc0a8-134">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="dc0a8-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="dc0a8-135">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="dc0a8-135">The default output type is text/csv.</span></span> <span data-ttu-id="dc0a8-136">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="dc0a8-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dc0a8-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dc0a8-137">Request headers</span></span>

| <span data-ttu-id="dc0a8-138">Имя</span><span class="sxs-lookup"><span data-stu-id="dc0a8-138">Name</span></span>          | <span data-ttu-id="dc0a8-139">Описание</span><span class="sxs-lookup"><span data-stu-id="dc0a8-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="dc0a8-140">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dc0a8-140">Authorization</span></span> | <span data-ttu-id="dc0a8-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dc0a8-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="dc0a8-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc0a8-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="dc0a8-144">CSV</span><span class="sxs-lookup"><span data-stu-id="dc0a8-144">CSV</span></span>

<span data-ttu-id="dc0a8-145">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="dc0a8-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="dc0a8-146">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="dc0a8-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="dc0a8-147">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="dc0a8-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="dc0a8-148">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="dc0a8-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="dc0a8-149">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="dc0a8-149">Report Refresh Date</span></span>
- <span data-ttu-id="dc0a8-150">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="dc0a8-150">User Principal Name</span></span>
- <span data-ttu-id="dc0a8-151">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="dc0a8-151">Is Deleted</span></span>
- <span data-ttu-id="dc0a8-152">"Deleted Date" (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="dc0a8-152">Deleted Date</span></span>
- <span data-ttu-id="dc0a8-153">"Last Activity Date" (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="dc0a8-153">Last Activity Date</span></span>
- <span data-ttu-id="dc0a8-154">"Viewed Or Edited File Count" (Количество просмотренных или измененных файлов);</span><span class="sxs-lookup"><span data-stu-id="dc0a8-154">Viewed Or Edited File Count</span></span>
- <span data-ttu-id="dc0a8-155">"Synced File Count" (Количество синхронизированных файлов);</span><span class="sxs-lookup"><span data-stu-id="dc0a8-155">Synced File Count</span></span>
- <span data-ttu-id="dc0a8-156">"Shared Internally File Count" (Количество файлов, к которым предоставлен доступ внутренним пользователям);</span><span class="sxs-lookup"><span data-stu-id="dc0a8-156">Shared Internally File Count</span></span>
- <span data-ttu-id="dc0a8-157">"Shared Externally File Count" (Количество файлов, к которым предоставлен доступ внешним пользователям);</span><span class="sxs-lookup"><span data-stu-id="dc0a8-157">Shared Externally File Count</span></span>
- <span data-ttu-id="dc0a8-158">"Assigned Products" (Назначенные продукты);</span><span class="sxs-lookup"><span data-stu-id="dc0a8-158">Assigned Products</span></span>
- <span data-ttu-id="dc0a8-159">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="dc0a8-159">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="dc0a8-160">JSON</span><span class="sxs-lookup"><span data-stu-id="dc0a8-160">JSON</span></span>

<span data-ttu-id="dc0a8-161">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[онедривеактивитюсердетаил](../resources/onedriveactivityuserdetail.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dc0a8-161">If successful, this method returns a `200 OK` response code and a **[oneDriveActivityUserDetail](../resources/onedriveactivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="dc0a8-162">Размер страницы по умолчанию для этого запроса составляет 200 элементов.</span><span class="sxs-lookup"><span data-stu-id="dc0a8-162">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="dc0a8-163">Пример</span><span class="sxs-lookup"><span data-stu-id="dc0a8-163">Example</span></span>

### <a name="csv"></a><span data-ttu-id="dc0a8-164">CSV</span><span class="sxs-lookup"><span data-stu-id="dc0a8-164">CSV</span></span>

<span data-ttu-id="dc0a8-165">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="dc0a8-165">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="dc0a8-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="dc0a8-166">Request</span></span>

<span data-ttu-id="dc0a8-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dc0a8-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveactivityuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveActivityUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="dc0a8-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc0a8-168">Response</span></span>

<span data-ttu-id="dc0a8-169">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dc0a8-169">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="dc0a8-170">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="dc0a8-170">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="dc0a8-171">JSON</span><span class="sxs-lookup"><span data-stu-id="dc0a8-171">JSON</span></span>

<span data-ttu-id="dc0a8-172">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="dc0a8-172">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="dc0a8-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="dc0a8-173">Request</span></span>

<span data-ttu-id="dc0a8-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dc0a8-174">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveactivityuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveActivityUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="dc0a8-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc0a8-175">Response</span></span>

<span data-ttu-id="dc0a8-176">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dc0a8-176">The following is an example of the response.</span></span>

> <span data-ttu-id="dc0a8-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dc0a8-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "Error: /api-reference/beta/api/reportroot-getonedriveactivityuserdetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
