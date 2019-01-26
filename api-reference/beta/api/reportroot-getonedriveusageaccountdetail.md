---
title: 'reportRoot: getOneDriveUsageAccountDetail'
description: Получите сведения об использовании OneDrive с разбивкой по учетным записям.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 0cdc6e0ccdd79484a5edf964213883640e85de6a
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571459"
---
# <a name="reportroot-getonedriveusageaccountdetail"></a><span data-ttu-id="4cb8c-103">reportRoot: getOneDriveUsageAccountDetail</span><span class="sxs-lookup"><span data-stu-id="4cb8c-103">reportRoot: getOneDriveUsageAccountDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4cb8c-104">Получите сведения об использовании OneDrive с разбивкой по учетным записям.</span><span class="sxs-lookup"><span data-stu-id="4cb8c-104">Get details about OneDrive usage by account.</span></span>

> <span data-ttu-id="4cb8c-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span><span class="sxs-lookup"><span data-stu-id="4cb8c-105">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="4cb8c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4cb8c-106">Permissions</span></span>

<span data-ttu-id="4cb8c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4cb8c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4cb8c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4cb8c-109">Permission type</span></span>                        | <span data-ttu-id="4cb8c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4cb8c-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="4cb8c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4cb8c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4cb8c-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4cb8c-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="4cb8c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4cb8c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4cb8c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4cb8c-114">Not supported.</span></span>                           |
| <span data-ttu-id="4cb8c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4cb8c-115">Application</span></span>                            | <span data-ttu-id="4cb8c-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4cb8c-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="4cb8c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4cb8c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageAccountDetail(period='{period_value}')
GET /reports/getOneDriveUsageAccountDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="4cb8c-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="4cb8c-118">Function parameters</span></span>

<span data-ttu-id="4cb8c-119">В URL-адресе запроса укажите один из следующих параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="4cb8c-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="4cb8c-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="4cb8c-120">Parameter</span></span> | <span data-ttu-id="4cb8c-121">Тип</span><span class="sxs-lookup"><span data-stu-id="4cb8c-121">Type</span></span>   | <span data-ttu-id="4cb8c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="4cb8c-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="4cb8c-123">period</span><span class="sxs-lookup"><span data-stu-id="4cb8c-123">period</span></span>    | <span data-ttu-id="4cb8c-124">строка</span><span class="sxs-lookup"><span data-stu-id="4cb8c-124">string</span></span> | <span data-ttu-id="4cb8c-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="4cb8c-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="4cb8c-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="4cb8c-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="4cb8c-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="4cb8c-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="4cb8c-128">date</span><span class="sxs-lookup"><span data-stu-id="4cb8c-128">date</span></span>      | <span data-ttu-id="4cb8c-129">Date</span><span class="sxs-lookup"><span data-stu-id="4cb8c-129">Date</span></span>   | <span data-ttu-id="4cb8c-130">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="4cb8c-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="4cb8c-131">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="4cb8c-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="4cb8c-132">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="4cb8c-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="4cb8c-133">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="4cb8c-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="4cb8c-134">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4cb8c-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="4cb8c-135">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="4cb8c-135">The default output type is text/csv.</span></span> <span data-ttu-id="4cb8c-136">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="4cb8c-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4cb8c-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4cb8c-137">Request headers</span></span>

| <span data-ttu-id="4cb8c-138">Имя</span><span class="sxs-lookup"><span data-stu-id="4cb8c-138">Name</span></span>          | <span data-ttu-id="4cb8c-139">Описание</span><span class="sxs-lookup"><span data-stu-id="4cb8c-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="4cb8c-140">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4cb8c-140">Authorization</span></span> | <span data-ttu-id="4cb8c-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4cb8c-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="4cb8c-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="4cb8c-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="4cb8c-144">CSV</span><span class="sxs-lookup"><span data-stu-id="4cb8c-144">CSV</span></span>

<span data-ttu-id="4cb8c-145">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="4cb8c-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="4cb8c-146">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="4cb8c-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="4cb8c-147">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="4cb8c-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="4cb8c-148">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="4cb8c-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="4cb8c-149">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="4cb8c-149">Report Refresh Date</span></span>
- <span data-ttu-id="4cb8c-150">"Site URL" (URL-адрес сайта);</span><span class="sxs-lookup"><span data-stu-id="4cb8c-150">Site URL</span></span>
- <span data-ttu-id="4cb8c-151">"Owner Display Name" (Отображаемое имя владельца);</span><span class="sxs-lookup"><span data-stu-id="4cb8c-151">Owner Display Name</span></span>
- <span data-ttu-id="4cb8c-152">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="4cb8c-152">Is Deleted</span></span>
- <span data-ttu-id="4cb8c-153">"Last Activity Date" (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="4cb8c-153">Last Activity Date</span></span>
- <span data-ttu-id="4cb8c-154">"File Count" (Количество файлов);</span><span class="sxs-lookup"><span data-stu-id="4cb8c-154">File Count</span></span>
- <span data-ttu-id="4cb8c-155">Active File Count (количество активных файлов)</span><span class="sxs-lookup"><span data-stu-id="4cb8c-155">Active File Count</span></span>
- <span data-ttu-id="4cb8c-156">Storage Used (Byte) [использовано (байт)]</span><span class="sxs-lookup"><span data-stu-id="4cb8c-156">Storage Used (Byte)</span></span>
- <span data-ttu-id="4cb8c-157">Storage Allocated (Byte) [выделено (байт)]</span><span class="sxs-lookup"><span data-stu-id="4cb8c-157">Storage Allocated (Byte)</span></span>
- <span data-ttu-id="4cb8c-158">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="4cb8c-158">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="4cb8c-159">JSON</span><span class="sxs-lookup"><span data-stu-id="4cb8c-159">JSON</span></span>

<span data-ttu-id="4cb8c-160">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[oneDriveUsageAccountDetail](../resources/onedriveusageaccountdetail.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4cb8c-160">If successful, this method returns a `200 OK` response code and a **[oneDriveUsageAccountDetail](../resources/onedriveusageaccountdetail.md)** object in the response body.</span></span>

<span data-ttu-id="4cb8c-161">Размер страницы по умолчанию для этого запроса — 200 элементов.</span><span class="sxs-lookup"><span data-stu-id="4cb8c-161">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="4cb8c-162">Пример</span><span class="sxs-lookup"><span data-stu-id="4cb8c-162">Example</span></span>

<span data-ttu-id="4cb8c-163">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="4cb8c-163">The following is an example that outputs CSV.</span></span>

### <a name="csv"></a><span data-ttu-id="4cb8c-164">CSV</span><span class="sxs-lookup"><span data-stu-id="4cb8c-164">CSV</span></span>

#### <a name="request"></a><span data-ttu-id="4cb8c-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="4cb8c-165">Request</span></span>

<span data-ttu-id="4cb8c-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4cb8c-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="4cb8c-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="4cb8c-167">Response</span></span>

<span data-ttu-id="4cb8c-168">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4cb8c-168">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="4cb8c-169">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="4cb8c-169">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site URL,Owner Display Name,Is Deleted,Last Activity Date,File Count,Active File Count,Storage Used (Byte),Storage Allocated (Byte),Report Period
```

### <a name="json"></a><span data-ttu-id="4cb8c-170">JSON</span><span class="sxs-lookup"><span data-stu-id="4cb8c-170">JSON</span></span>

<span data-ttu-id="4cb8c-171">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="4cb8c-171">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="4cb8c-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="4cb8c-172">Request</span></span>

<span data-ttu-id="4cb8c-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4cb8c-173">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="4cb8c-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="4cb8c-174">Response</span></span>

<span data-ttu-id="4cb8c-175">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4cb8c-175">The following is an example of the response.</span></span>

> <span data-ttu-id="4cb8c-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4cb8c-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oneDriveUsageAccountDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 400

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.oneDriveUsageAccountDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteUrl": "siteUrl-value", 
      "ownerDisplayName": "ownerDisplayName-value", 
      "isDeleted": false, 
      "lastActivityDate": "2017-09-01", 
      "fileCount": 9, 
      "activeFileCount": 5, 
      "storageUsedInBytes": 12190375, 
      "storageAllocatedInBytes": 549755813880, 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getonedriveusageaccountdetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
