---
title: 'reportRoot: getSharePointSiteUsageSiteCounts'
description: Узнайте, сколько всего файлов на всех сайтах и сколько из них активны. Файл (пользователь или система) считается активным, если он был сохранен, синхронизирован, изменен в указанный период или им поделились в указанный период.
ms.openlocfilehash: 1689b43b4f3e90ca88d61e6b8bd4332d29ad1e5f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074820"
---
# <a name="reportroot-getsharepointsiteusagesitecounts"></a><span data-ttu-id="4cb98-104">reportRoot: getSharePointSiteUsageSiteCounts</span><span class="sxs-lookup"><span data-stu-id="4cb98-104">reportRoot: getSharePointSiteUsageSiteCounts</span></span>

> <span data-ttu-id="4cb98-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4cb98-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4cb98-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4cb98-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4cb98-107">Узнайте, сколько всего файлов на всех сайтах и сколько из них активны.</span><span class="sxs-lookup"><span data-stu-id="4cb98-107">Get the total number of files across all sites and the number of active files.</span></span> <span data-ttu-id="4cb98-108">Файл (пользователь или система) считается активным, если он был сохранен, синхронизирован, изменен в указанный период или им поделились в указанный период.</span><span class="sxs-lookup"><span data-stu-id="4cb98-108">A file (user or system) is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span>

> <span data-ttu-id="4cb98-109">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: использование сайтов SharePoint](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span><span class="sxs-lookup"><span data-stu-id="4cb98-109">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="4cb98-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4cb98-110">Permissions</span></span>

<span data-ttu-id="4cb98-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4cb98-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4cb98-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4cb98-113">Permission type</span></span>                        | <span data-ttu-id="4cb98-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4cb98-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="4cb98-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4cb98-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="4cb98-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4cb98-116">Reports.Read.All</span></span>                         |
| <span data-ttu-id="4cb98-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4cb98-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4cb98-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4cb98-118">Not supported.</span></span>                           |
| <span data-ttu-id="4cb98-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4cb98-119">Application</span></span>                            | <span data-ttu-id="4cb98-120">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4cb98-120">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="4cb98-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4cb98-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageSiteCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="4cb98-122">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="4cb98-122">Function parameters</span></span>

<span data-ttu-id="4cb98-123">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="4cb98-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="4cb98-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="4cb98-124">Parameter</span></span> | <span data-ttu-id="4cb98-125">Тип</span><span class="sxs-lookup"><span data-stu-id="4cb98-125">Type</span></span>   | <span data-ttu-id="4cb98-126">Описание</span><span class="sxs-lookup"><span data-stu-id="4cb98-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="4cb98-127">period</span><span class="sxs-lookup"><span data-stu-id="4cb98-127">period</span></span>    | <span data-ttu-id="4cb98-128">строка</span><span class="sxs-lookup"><span data-stu-id="4cb98-128">string</span></span> | <span data-ttu-id="4cb98-129">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="4cb98-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="4cb98-130">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="4cb98-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="4cb98-131">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="4cb98-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="4cb98-132">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4cb98-132">Required.</span></span> |

<span data-ttu-id="4cb98-133">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4cb98-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="4cb98-134">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="4cb98-134">The default output type is text/csv.</span></span> <span data-ttu-id="4cb98-135">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="4cb98-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4cb98-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4cb98-136">Request headers</span></span>

| <span data-ttu-id="4cb98-137">Имя</span><span class="sxs-lookup"><span data-stu-id="4cb98-137">Name</span></span>          | <span data-ttu-id="4cb98-138">Описание</span><span class="sxs-lookup"><span data-stu-id="4cb98-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="4cb98-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4cb98-139">Authorization</span></span> | <span data-ttu-id="4cb98-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4cb98-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="4cb98-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="4cb98-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="4cb98-143">CSV</span><span class="sxs-lookup"><span data-stu-id="4cb98-143">CSV</span></span>

<span data-ttu-id="4cb98-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="4cb98-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="4cb98-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="4cb98-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="4cb98-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="4cb98-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="4cb98-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="4cb98-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="4cb98-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="4cb98-148">Report Refresh Date</span></span>
- <span data-ttu-id="4cb98-149">"Site Type" (Тип сайта);</span><span class="sxs-lookup"><span data-stu-id="4cb98-149">Site Type</span></span>
- <span data-ttu-id="4cb98-150">Total (всего)</span><span class="sxs-lookup"><span data-stu-id="4cb98-150">Total</span></span>
- <span data-ttu-id="4cb98-151">Active (активные)</span><span class="sxs-lookup"><span data-stu-id="4cb98-151">Active</span></span>
- <span data-ttu-id="4cb98-152">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="4cb98-152">Report Date</span></span>
- <span data-ttu-id="4cb98-153">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="4cb98-153">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="4cb98-154">JSON</span><span class="sxs-lookup"><span data-stu-id="4cb98-154">JSON</span></span>

<span data-ttu-id="4cb98-155">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[sharePointSiteUsageSiteCounts](../resources/sharepointsiteusagesitecounts.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4cb98-155">If successful, this method returns a `200 OK` response code and a **[sharePointSiteUsageSiteCounts](../resources/sharepointsiteusagesitecounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4cb98-156">Пример</span><span class="sxs-lookup"><span data-stu-id="4cb98-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="4cb98-157">CSV</span><span class="sxs-lookup"><span data-stu-id="4cb98-157">CSV</span></span>

<span data-ttu-id="4cb98-158">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="4cb98-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="4cb98-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="4cb98-159">Request</span></span>

<span data-ttu-id="4cb98-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4cb98-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagesitecounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageSiteCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="4cb98-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="4cb98-161">Response</span></span>

<span data-ttu-id="4cb98-162">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4cb98-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="4cb98-163">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="4cb98-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="4cb98-164">JSON</span><span class="sxs-lookup"><span data-stu-id="4cb98-164">JSON</span></span>

<span data-ttu-id="4cb98-165">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="4cb98-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="4cb98-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="4cb98-166">Request</span></span>

<span data-ttu-id="4cb98-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4cb98-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagesitecounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageSiteCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="4cb98-168">Ответ</span><span class="sxs-lookup"><span data-stu-id="4cb98-168">Response</span></span>

<span data-ttu-id="4cb98-169">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4cb98-169">The following is an example of the response.</span></span>

> <span data-ttu-id="4cb98-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4cb98-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
