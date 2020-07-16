---
title: 'reportRoot: getSharePointSiteUsageFileCounts'
description: Узнайте, сколько всего файлов на всех сайтах и сколько из них активны. Файл (пользователь или система) считается активным, если он был сохранен, синхронизирован, изменен или отправлен в указанный период.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: c760ed84b3feaca4cfcb5329cd9aa28aeb292ec8
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896247"
---
# <a name="reportroot-getsharepointsiteusagefilecounts"></a><span data-ttu-id="84d59-104">reportRoot: getSharePointSiteUsageFileCounts</span><span class="sxs-lookup"><span data-stu-id="84d59-104">reportRoot: getSharePointSiteUsageFileCounts</span></span>

<span data-ttu-id="84d59-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84d59-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84d59-106">Узнайте, сколько всего файлов на всех сайтах и сколько из них активны.</span><span class="sxs-lookup"><span data-stu-id="84d59-106">Get the total number of files across all sites and the number of active files.</span></span> <span data-ttu-id="84d59-107">Файл (пользователь или система) считается активным, если он был сохранен, синхронизирован, изменен или отправлен в указанный период.</span><span class="sxs-lookup"><span data-stu-id="84d59-107">A file (user or system) is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span>

> <span data-ttu-id="84d59-108">**Примечание:** Сведения о различных представлениях и именах отчетов можно найти в [статье Microsoft 365 Reports-SharePoint site Usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span><span class="sxs-lookup"><span data-stu-id="84d59-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="84d59-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="84d59-109">Permissions</span></span>

<span data-ttu-id="84d59-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84d59-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="84d59-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="84d59-112">Permission type</span></span>                        | <span data-ttu-id="84d59-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="84d59-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="84d59-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="84d59-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="84d59-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="84d59-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="84d59-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="84d59-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84d59-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84d59-117">Not supported.</span></span>                           |
| <span data-ttu-id="84d59-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="84d59-118">Application</span></span>                            | <span data-ttu-id="84d59-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="84d59-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="84d59-120">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="84d59-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="84d59-121">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="84d59-121">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="84d59-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="84d59-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="84d59-123">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="84d59-123">Function parameters</span></span>

<span data-ttu-id="84d59-124">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="84d59-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="84d59-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="84d59-125">Parameter</span></span> | <span data-ttu-id="84d59-126">Тип</span><span class="sxs-lookup"><span data-stu-id="84d59-126">Type</span></span>   | <span data-ttu-id="84d59-127">Описание</span><span class="sxs-lookup"><span data-stu-id="84d59-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="84d59-128">period</span><span class="sxs-lookup"><span data-stu-id="84d59-128">period</span></span>    | <span data-ttu-id="84d59-129">string</span><span class="sxs-lookup"><span data-stu-id="84d59-129">string</span></span> | <span data-ttu-id="84d59-130">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="84d59-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="84d59-131">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="84d59-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="84d59-132">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="84d59-132">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="84d59-133">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="84d59-133">Required.</span></span> |

<span data-ttu-id="84d59-134">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="84d59-134">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="84d59-135">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="84d59-135">The default output type is text/csv.</span></span> <span data-ttu-id="84d59-136">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="84d59-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="84d59-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="84d59-137">Request headers</span></span>

| <span data-ttu-id="84d59-138">Имя</span><span class="sxs-lookup"><span data-stu-id="84d59-138">Name</span></span>          | <span data-ttu-id="84d59-139">Описание</span><span class="sxs-lookup"><span data-stu-id="84d59-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="84d59-140">Авторизация</span><span class="sxs-lookup"><span data-stu-id="84d59-140">Authorization</span></span> | <span data-ttu-id="84d59-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="84d59-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="84d59-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="84d59-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="84d59-144">CSV</span><span class="sxs-lookup"><span data-stu-id="84d59-144">CSV</span></span>

<span data-ttu-id="84d59-145">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="84d59-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="84d59-146">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="84d59-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="84d59-147">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="84d59-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="84d59-148">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="84d59-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="84d59-149">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="84d59-149">Report Refresh Date</span></span>
- <span data-ttu-id="84d59-150">"Site Type" (Тип сайта);</span><span class="sxs-lookup"><span data-stu-id="84d59-150">Site Type</span></span>
- <span data-ttu-id="84d59-151">"Total" (Всего);</span><span class="sxs-lookup"><span data-stu-id="84d59-151">Total</span></span>
- <span data-ttu-id="84d59-152">Active (активные)</span><span class="sxs-lookup"><span data-stu-id="84d59-152">Active</span></span>
- <span data-ttu-id="84d59-153">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="84d59-153">Report Date</span></span>
- <span data-ttu-id="84d59-154">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="84d59-154">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="84d59-155">JSON</span><span class="sxs-lookup"><span data-stu-id="84d59-155">JSON</span></span>

<span data-ttu-id="84d59-156">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[шарепоинтситеусажефилекаунтс](../resources/sharepointsiteusagefilecounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="84d59-156">If successful, this method returns a `200 OK` response code and a **[sharePointSiteUsageFileCounts](../resources/sharepointsiteusagefilecounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84d59-157">Пример</span><span class="sxs-lookup"><span data-stu-id="84d59-157">Example</span></span>

### <a name="csv"></a><span data-ttu-id="84d59-158">CSV</span><span class="sxs-lookup"><span data-stu-id="84d59-158">CSV</span></span>

<span data-ttu-id="84d59-159">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="84d59-159">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="84d59-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="84d59-160">Request</span></span>

<span data-ttu-id="84d59-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="84d59-161">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getsharepointsiteusagefilecounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageFileCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="84d59-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="84d59-162">Response</span></span>

<span data-ttu-id="84d59-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="84d59-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="84d59-164">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="84d59-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="84d59-165">JSON</span><span class="sxs-lookup"><span data-stu-id="84d59-165">JSON</span></span>

<span data-ttu-id="84d59-166">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="84d59-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="84d59-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="84d59-167">Request</span></span>

<span data-ttu-id="84d59-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="84d59-168">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getsharepointsiteusagefilecounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageFileCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="84d59-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="84d59-169">Response</span></span>

<span data-ttu-id="84d59-170">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="84d59-170">The following is an example of the response.</span></span>

> <span data-ttu-id="84d59-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="84d59-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointSiteUsageFileCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 255

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.sharePointSiteUsageFileCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteType": "All", 
      "total": 25687, 
      "active": 209, 
      "reportDate": "2017-09-01", 
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
