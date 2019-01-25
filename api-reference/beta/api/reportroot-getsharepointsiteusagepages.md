---
title: 'reportRoot: getSharePointSiteUsagePages'
description: Узнайте, сколько страниц было просмотрено на всех сайтах.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: ca7e036826a02323d2a7aa4cc9e58471c16ce6f0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522562"
---
# <a name="reportroot-getsharepointsiteusagepages"></a><span data-ttu-id="09877-103">reportRoot: getSharePointSiteUsagePages</span><span class="sxs-lookup"><span data-stu-id="09877-103">reportRoot: getSharePointSiteUsagePages</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09877-104">Узнайте, сколько страниц было просмотрено на всех сайтах.</span><span class="sxs-lookup"><span data-stu-id="09877-104">Get the number of pages viewed across all sites.</span></span>

> <span data-ttu-id="09877-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: использование сайтов SharePoint](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span><span class="sxs-lookup"><span data-stu-id="09877-105">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="09877-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="09877-106">Permissions</span></span>

<span data-ttu-id="09877-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09877-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="09877-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="09877-109">Permission type</span></span>                        | <span data-ttu-id="09877-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="09877-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="09877-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="09877-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="09877-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="09877-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="09877-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="09877-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09877-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09877-114">Not supported.</span></span>                           |
| <span data-ttu-id="09877-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="09877-115">Application</span></span>                            | <span data-ttu-id="09877-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="09877-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="09877-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="09877-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsagePages(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="09877-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="09877-118">Function parameters</span></span>

<span data-ttu-id="09877-119">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="09877-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="09877-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="09877-120">Parameter</span></span> | <span data-ttu-id="09877-121">Тип</span><span class="sxs-lookup"><span data-stu-id="09877-121">Type</span></span>   | <span data-ttu-id="09877-122">Описание</span><span class="sxs-lookup"><span data-stu-id="09877-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="09877-123">period</span><span class="sxs-lookup"><span data-stu-id="09877-123">period</span></span>    | <span data-ttu-id="09877-124">строка</span><span class="sxs-lookup"><span data-stu-id="09877-124">string</span></span> | <span data-ttu-id="09877-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="09877-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="09877-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="09877-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="09877-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="09877-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="09877-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="09877-128">Required.</span></span> |

<span data-ttu-id="09877-129">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="09877-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="09877-130">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="09877-130">The default output type is text/csv.</span></span> <span data-ttu-id="09877-131">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="09877-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="09877-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="09877-132">Request headers</span></span>

| <span data-ttu-id="09877-133">Имя</span><span class="sxs-lookup"><span data-stu-id="09877-133">Name</span></span>          | <span data-ttu-id="09877-134">Описание</span><span class="sxs-lookup"><span data-stu-id="09877-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="09877-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="09877-135">Authorization</span></span> | <span data-ttu-id="09877-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="09877-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="09877-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="09877-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="09877-139">CSV</span><span class="sxs-lookup"><span data-stu-id="09877-139">CSV</span></span>

<span data-ttu-id="09877-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="09877-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="09877-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="09877-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="09877-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="09877-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="09877-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="09877-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="09877-144">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="09877-144">Report Refresh Date</span></span>
- <span data-ttu-id="09877-145">"Site Type" (Тип сайта);</span><span class="sxs-lookup"><span data-stu-id="09877-145">Site Type</span></span>
- <span data-ttu-id="09877-146">"Page View Count" (Количество просмотров страницы);</span><span class="sxs-lookup"><span data-stu-id="09877-146">Page View Count</span></span>
- <span data-ttu-id="09877-147">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="09877-147">Report Date</span></span>
- <span data-ttu-id="09877-148">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="09877-148">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="09877-149">JSON</span><span class="sxs-lookup"><span data-stu-id="09877-149">JSON</span></span>

<span data-ttu-id="09877-150">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[sharePointSiteUsagePages](../resources/sharepointsiteusagepages.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="09877-150">If successful, this method returns a `200 OK` response code and a **[sharePointSiteUsagePages](../resources/sharepointsiteusagepages.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09877-151">Пример</span><span class="sxs-lookup"><span data-stu-id="09877-151">Example</span></span>

### <a name="csv"></a><span data-ttu-id="09877-152">CSV</span><span class="sxs-lookup"><span data-stu-id="09877-152">CSV</span></span>

<span data-ttu-id="09877-153">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="09877-153">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="09877-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="09877-154">Request</span></span>

<span data-ttu-id="09877-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="09877-155">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagepages_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsagePages(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="09877-156">Ответ</span><span class="sxs-lookup"><span data-stu-id="09877-156">Response</span></span>

<span data-ttu-id="09877-157">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="09877-157">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="09877-158">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="09877-158">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Page View Count,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="09877-159">JSON</span><span class="sxs-lookup"><span data-stu-id="09877-159">JSON</span></span>

<span data-ttu-id="09877-160">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="09877-160">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="09877-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="09877-161">Request</span></span>

<span data-ttu-id="09877-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="09877-162">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagepages_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsagePages(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="09877-163">Ответ</span><span class="sxs-lookup"><span data-stu-id="09877-163">Response</span></span>

<span data-ttu-id="09877-164">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="09877-164">The following is an example of the response.</span></span>

> <span data-ttu-id="09877-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="09877-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointSiteUsagePages"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 243

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.sharePointSiteUsagePages)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteType": "All", 
      "pageViewCount": 183, 
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
    "Error: /api-reference/beta/api/reportroot-getsharepointsiteusagepages.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
