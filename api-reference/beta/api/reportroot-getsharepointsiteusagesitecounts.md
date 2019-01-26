---
title: 'reportRoot: getSharePointSiteUsageSiteCounts'
description: Узнайте, сколько всего файлов на всех сайтах и сколько из них активны. Файл (пользователь или система) считается активным, если он был сохранен, синхронизирован, изменен в указанный период или им поделились в указанный период.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: d1286b1904c2e9d89fc4d629c7a635f76cf43d62
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575473"
---
# <a name="reportroot-getsharepointsiteusagesitecounts"></a><span data-ttu-id="b719d-104">reportRoot: getSharePointSiteUsageSiteCounts</span><span class="sxs-lookup"><span data-stu-id="b719d-104">reportRoot: getSharePointSiteUsageSiteCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b719d-105">Узнайте, сколько всего файлов на всех сайтах и сколько из них активны.</span><span class="sxs-lookup"><span data-stu-id="b719d-105">Get the total number of files across all sites and the number of active files.</span></span> <span data-ttu-id="b719d-106">Файл (пользователь или система) считается активным, если он был сохранен, синхронизирован, изменен в указанный период или им поделились в указанный период.</span><span class="sxs-lookup"><span data-stu-id="b719d-106">A file (user or system) is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span>

> <span data-ttu-id="b719d-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: использование сайтов SharePoint](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span><span class="sxs-lookup"><span data-stu-id="b719d-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="b719d-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b719d-108">Permissions</span></span>

<span data-ttu-id="b719d-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b719d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b719d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b719d-111">Permission type</span></span>                        | <span data-ttu-id="b719d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b719d-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b719d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b719d-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="b719d-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b719d-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b719d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b719d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b719d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b719d-116">Not supported.</span></span>                           |
| <span data-ttu-id="b719d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b719d-117">Application</span></span>                            | <span data-ttu-id="b719d-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b719d-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="b719d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b719d-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageSiteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="b719d-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="b719d-120">Function parameters</span></span>

<span data-ttu-id="b719d-121">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="b719d-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="b719d-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="b719d-122">Parameter</span></span> | <span data-ttu-id="b719d-123">Тип</span><span class="sxs-lookup"><span data-stu-id="b719d-123">Type</span></span>   | <span data-ttu-id="b719d-124">Описание</span><span class="sxs-lookup"><span data-stu-id="b719d-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b719d-125">period</span><span class="sxs-lookup"><span data-stu-id="b719d-125">period</span></span>    | <span data-ttu-id="b719d-126">строка</span><span class="sxs-lookup"><span data-stu-id="b719d-126">string</span></span> | <span data-ttu-id="b719d-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="b719d-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b719d-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="b719d-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b719d-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="b719d-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="b719d-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b719d-130">Required.</span></span> |

<span data-ttu-id="b719d-131">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b719d-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="b719d-132">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="b719d-132">The default output type is text/csv.</span></span> <span data-ttu-id="b719d-133">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="b719d-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b719d-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b719d-134">Request headers</span></span>

| <span data-ttu-id="b719d-135">Имя</span><span class="sxs-lookup"><span data-stu-id="b719d-135">Name</span></span>          | <span data-ttu-id="b719d-136">Описание</span><span class="sxs-lookup"><span data-stu-id="b719d-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="b719d-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b719d-137">Authorization</span></span> | <span data-ttu-id="b719d-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b719d-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="b719d-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="b719d-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="b719d-141">CSV</span><span class="sxs-lookup"><span data-stu-id="b719d-141">CSV</span></span>

<span data-ttu-id="b719d-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="b719d-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b719d-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="b719d-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b719d-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="b719d-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b719d-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="b719d-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b719d-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="b719d-146">Report Refresh Date</span></span>
- <span data-ttu-id="b719d-147">"Site Type" (Тип сайта);</span><span class="sxs-lookup"><span data-stu-id="b719d-147">Site Type</span></span>
- <span data-ttu-id="b719d-148">Total (всего)</span><span class="sxs-lookup"><span data-stu-id="b719d-148">Total</span></span>
- <span data-ttu-id="b719d-149">Active (активные)</span><span class="sxs-lookup"><span data-stu-id="b719d-149">Active</span></span>
- <span data-ttu-id="b719d-150">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="b719d-150">Report Date</span></span>
- <span data-ttu-id="b719d-151">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="b719d-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="b719d-152">JSON</span><span class="sxs-lookup"><span data-stu-id="b719d-152">JSON</span></span>

<span data-ttu-id="b719d-153">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[sharePointSiteUsageSiteCounts](../resources/sharepointsiteusagesitecounts.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b719d-153">If successful, this method returns a `200 OK` response code and a **[sharePointSiteUsageSiteCounts](../resources/sharepointsiteusagesitecounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b719d-154">Пример</span><span class="sxs-lookup"><span data-stu-id="b719d-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="b719d-155">CSV</span><span class="sxs-lookup"><span data-stu-id="b719d-155">CSV</span></span>

<span data-ttu-id="b719d-156">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="b719d-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="b719d-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="b719d-157">Request</span></span>

<span data-ttu-id="b719d-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b719d-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagesitecounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageSiteCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="b719d-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="b719d-159">Response</span></span>

<span data-ttu-id="b719d-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b719d-160">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="b719d-161">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="b719d-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Total,Active,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="b719d-162">JSON</span><span class="sxs-lookup"><span data-stu-id="b719d-162">JSON</span></span>

<span data-ttu-id="b719d-163">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="b719d-163">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="b719d-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="b719d-164">Request</span></span>

<span data-ttu-id="b719d-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b719d-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagesitecounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageSiteCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="b719d-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="b719d-166">Response</span></span>

<span data-ttu-id="b719d-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b719d-167">The following is an example of the response.</span></span>

> <span data-ttu-id="b719d-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b719d-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointSiteUsageSiteCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 251

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.sharePointSiteUsageSiteCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteType": "All", 
      "total": 47, 
      "active": 15, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getsharepointsiteusagesitecounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
