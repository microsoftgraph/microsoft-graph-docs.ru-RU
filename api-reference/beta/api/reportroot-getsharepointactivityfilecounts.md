---
title: 'reportRoot: getSharePointActivityFileCounts'
description: Узнайте, сколько уникальных пользователей с лицензиями работали с хранящимися на сайтах SharePoint файлами.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 17da8c3229e21904bd46d2661ec2dff442b4aa05
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520727"
---
# <a name="reportroot-getsharepointactivityfilecounts"></a><span data-ttu-id="6cec2-103">reportRoot: getSharePointActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="6cec2-103">reportRoot: getSharePointActivityFileCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6cec2-104">Узнайте, сколько уникальных пользователей с лицензиями работали с хранящимися на сайтах SharePoint файлами.</span><span class="sxs-lookup"><span data-stu-id="6cec2-104">Get the number of unique, licensed users who interacted with files stored on SharePoint sites.</span></span>

> <span data-ttu-id="6cec2-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="6cec2-105">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="6cec2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6cec2-106">Permissions</span></span>

<span data-ttu-id="6cec2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6cec2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6cec2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6cec2-109">Permission type</span></span>                        | <span data-ttu-id="6cec2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6cec2-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="6cec2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6cec2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6cec2-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6cec2-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="6cec2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6cec2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6cec2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6cec2-114">Not supported.</span></span>                           |
| <span data-ttu-id="6cec2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6cec2-115">Application</span></span>                            | <span data-ttu-id="6cec2-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6cec2-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="6cec2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6cec2-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="6cec2-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="6cec2-118">Function parameters</span></span>

<span data-ttu-id="6cec2-119">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="6cec2-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="6cec2-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="6cec2-120">Parameter</span></span> | <span data-ttu-id="6cec2-121">Тип</span><span class="sxs-lookup"><span data-stu-id="6cec2-121">Type</span></span>   | <span data-ttu-id="6cec2-122">Описание</span><span class="sxs-lookup"><span data-stu-id="6cec2-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="6cec2-123">period</span><span class="sxs-lookup"><span data-stu-id="6cec2-123">period</span></span>    | <span data-ttu-id="6cec2-124">строка</span><span class="sxs-lookup"><span data-stu-id="6cec2-124">string</span></span> | <span data-ttu-id="6cec2-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="6cec2-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="6cec2-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="6cec2-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="6cec2-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="6cec2-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="6cec2-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6cec2-128">Required.</span></span> |

<span data-ttu-id="6cec2-129">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6cec2-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="6cec2-130">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="6cec2-130">The default output type is text/csv.</span></span> <span data-ttu-id="6cec2-131">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="6cec2-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6cec2-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6cec2-132">Request headers</span></span>

| <span data-ttu-id="6cec2-133">Имя</span><span class="sxs-lookup"><span data-stu-id="6cec2-133">Name</span></span>          | <span data-ttu-id="6cec2-134">Описание</span><span class="sxs-lookup"><span data-stu-id="6cec2-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="6cec2-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6cec2-135">Authorization</span></span> | <span data-ttu-id="6cec2-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6cec2-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="6cec2-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="6cec2-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="6cec2-139">CSV</span><span class="sxs-lookup"><span data-stu-id="6cec2-139">CSV</span></span>

<span data-ttu-id="6cec2-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="6cec2-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="6cec2-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="6cec2-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="6cec2-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="6cec2-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="6cec2-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="6cec2-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="6cec2-144">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="6cec2-144">Report Refresh Date</span></span>
- <span data-ttu-id="6cec2-145">"Viewed Or Edited" (Просмотрены или изменены);</span><span class="sxs-lookup"><span data-stu-id="6cec2-145">Viewed Or Edited</span></span>
- <span data-ttu-id="6cec2-146">"Synced" (Синхронизированы);</span><span class="sxs-lookup"><span data-stu-id="6cec2-146">Synced</span></span>
- <span data-ttu-id="6cec2-147">"Shared Internally" (К чему предоставлен доступ внутренним пользователям);</span><span class="sxs-lookup"><span data-stu-id="6cec2-147">Shared Internally</span></span>
- <span data-ttu-id="6cec2-148">"Shared Externally" (К чему предоставлен доступ внешним пользователям);</span><span class="sxs-lookup"><span data-stu-id="6cec2-148">Shared Externally</span></span>
- <span data-ttu-id="6cec2-149">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="6cec2-149">Report Date</span></span>
- <span data-ttu-id="6cec2-150">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="6cec2-150">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="6cec2-151">JSON</span><span class="sxs-lookup"><span data-stu-id="6cec2-151">JSON</span></span>

<span data-ttu-id="6cec2-152">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[siteActivitySummary](../resources/siteactivitysummary.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6cec2-152">If successful, this method returns a `200 OK` response code and a **[siteActivitySummary](../resources/siteactivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6cec2-153">Пример</span><span class="sxs-lookup"><span data-stu-id="6cec2-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="6cec2-154">CSV</span><span class="sxs-lookup"><span data-stu-id="6cec2-154">CSV</span></span>

<span data-ttu-id="6cec2-155">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="6cec2-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="6cec2-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="6cec2-156">Request</span></span>

<span data-ttu-id="6cec2-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6cec2-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityfilecounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityFileCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="6cec2-158">Ответ</span><span class="sxs-lookup"><span data-stu-id="6cec2-158">Response</span></span>

<span data-ttu-id="6cec2-159">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6cec2-159">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="6cec2-160">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="6cec2-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="6cec2-161">JSON</span><span class="sxs-lookup"><span data-stu-id="6cec2-161">JSON</span></span>

<span data-ttu-id="6cec2-162">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="6cec2-162">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="6cec2-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="6cec2-163">Request</span></span>

<span data-ttu-id="6cec2-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6cec2-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="6cec2-165">Ответ</span><span class="sxs-lookup"><span data-stu-id="6cec2-165">Response</span></span>

<span data-ttu-id="6cec2-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6cec2-166">The following is an example of the response.</span></span>

> <span data-ttu-id="6cec2-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6cec2-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.siteActivitySummary"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 278

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.siteActivitySummary)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "viewedOrEdited": 2141, 
      "synced": 614, 
      "sharedInternally": 9, 
      "sharedExternally": 0, 
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
    "Error: /api-reference/beta/api/reportroot-getsharepointactivityfilecounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
