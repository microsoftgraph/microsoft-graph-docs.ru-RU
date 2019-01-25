---
title: 'reportRoot: getSharePointActivityUserCounts'
description: Отслеживайте, как меняется количество активных пользователей. Пользователь считается активным, если он сохранил, синхронизировал, изменил или отправил файл или посетил страницу в указанный период.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: e3c806c991375d140a07c1fa09e19493f9b41f5b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513440"
---
# <a name="reportroot-getsharepointactivityusercounts"></a><span data-ttu-id="8eb54-104">reportRoot: getSharePointActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="8eb54-104">reportRoot: getSharePointActivityUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8eb54-105">Отслеживайте, как меняется количество активных пользователей.</span><span class="sxs-lookup"><span data-stu-id="8eb54-105">Get the trend in the number of active users.</span></span> <span data-ttu-id="8eb54-106">Пользователь считается активным, если он сохранил, синхронизировал, изменил или отправил файл или посетил страницу в указанный период.</span><span class="sxs-lookup"><span data-stu-id="8eb54-106">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span>

> <span data-ttu-id="8eb54-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="8eb54-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="8eb54-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8eb54-108">Permissions</span></span>

<span data-ttu-id="8eb54-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8eb54-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8eb54-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8eb54-111">Permission type</span></span>                        | <span data-ttu-id="8eb54-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8eb54-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="8eb54-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8eb54-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="8eb54-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8eb54-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="8eb54-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8eb54-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8eb54-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8eb54-116">Not supported.</span></span>                           |
| <span data-ttu-id="8eb54-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8eb54-117">Application</span></span>                            | <span data-ttu-id="8eb54-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8eb54-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="8eb54-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8eb54-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="8eb54-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="8eb54-120">Function parameters</span></span>

<span data-ttu-id="8eb54-121">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="8eb54-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="8eb54-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="8eb54-122">Parameter</span></span> | <span data-ttu-id="8eb54-123">Тип</span><span class="sxs-lookup"><span data-stu-id="8eb54-123">Type</span></span>   | <span data-ttu-id="8eb54-124">Описание</span><span class="sxs-lookup"><span data-stu-id="8eb54-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="8eb54-125">period</span><span class="sxs-lookup"><span data-stu-id="8eb54-125">period</span></span>    | <span data-ttu-id="8eb54-126">строка</span><span class="sxs-lookup"><span data-stu-id="8eb54-126">string</span></span> | <span data-ttu-id="8eb54-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="8eb54-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="8eb54-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="8eb54-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="8eb54-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="8eb54-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="8eb54-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8eb54-130">Required.</span></span> |

<span data-ttu-id="8eb54-131">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8eb54-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="8eb54-132">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="8eb54-132">The default output type is text/csv.</span></span> <span data-ttu-id="8eb54-133">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="8eb54-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8eb54-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8eb54-134">Request headers</span></span>

| <span data-ttu-id="8eb54-135">Имя</span><span class="sxs-lookup"><span data-stu-id="8eb54-135">Name</span></span>          | <span data-ttu-id="8eb54-136">Описание</span><span class="sxs-lookup"><span data-stu-id="8eb54-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="8eb54-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8eb54-137">Authorization</span></span> | <span data-ttu-id="8eb54-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8eb54-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="8eb54-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="8eb54-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="8eb54-141">CSV</span><span class="sxs-lookup"><span data-stu-id="8eb54-141">CSV</span></span>

<span data-ttu-id="8eb54-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="8eb54-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="8eb54-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="8eb54-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="8eb54-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="8eb54-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="8eb54-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="8eb54-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="8eb54-146">Report Refresh Date (дата обновления отчета)</span><span class="sxs-lookup"><span data-stu-id="8eb54-146">Report Refresh Date</span></span>
- <span data-ttu-id="8eb54-147">Visited Page (посетило страницу)</span><span class="sxs-lookup"><span data-stu-id="8eb54-147">Visited Page</span></span>
- <span data-ttu-id="8eb54-148">Viewed Or Edited (просмотрело или изменило)</span><span class="sxs-lookup"><span data-stu-id="8eb54-148">Viewed Or Edited</span></span>
- <span data-ttu-id="8eb54-149">"Synced" (Синхронизированы);</span><span class="sxs-lookup"><span data-stu-id="8eb54-149">Synced</span></span>
- <span data-ttu-id="8eb54-150">"Shared Internally" (К чему предоставлен доступ внутренним пользователям);</span><span class="sxs-lookup"><span data-stu-id="8eb54-150">Shared Internally</span></span>
- <span data-ttu-id="8eb54-151">"Shared Externally" (К чему предоставлен доступ внешним пользователям);</span><span class="sxs-lookup"><span data-stu-id="8eb54-151">Shared Externally</span></span>
- <span data-ttu-id="8eb54-152">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="8eb54-152">Report Date</span></span>
- <span data-ttu-id="8eb54-153">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="8eb54-153">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="8eb54-154">JSON</span><span class="sxs-lookup"><span data-stu-id="8eb54-154">JSON</span></span>

<span data-ttu-id="8eb54-155">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8eb54-155">If successful, this method returns a `200 OK` response code and a **[sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8eb54-156">Пример</span><span class="sxs-lookup"><span data-stu-id="8eb54-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="8eb54-157">CSV</span><span class="sxs-lookup"><span data-stu-id="8eb54-157">CSV</span></span>

<span data-ttu-id="8eb54-158">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="8eb54-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="8eb54-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="8eb54-159">Request</span></span>

<span data-ttu-id="8eb54-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8eb54-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="8eb54-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="8eb54-161">Response</span></span>

<span data-ttu-id="8eb54-162">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8eb54-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="8eb54-163">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="8eb54-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Visited Page,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="8eb54-164">JSON</span><span class="sxs-lookup"><span data-stu-id="8eb54-164">JSON</span></span>

<span data-ttu-id="8eb54-165">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="8eb54-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="8eb54-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="8eb54-166">Request</span></span>

<span data-ttu-id="8eb54-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8eb54-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="8eb54-168">Ответ</span><span class="sxs-lookup"><span data-stu-id="8eb54-168">Response</span></span>

<span data-ttu-id="8eb54-169">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8eb54-169">The following is an example of the response.</span></span>

> <span data-ttu-id="8eb54-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8eb54-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointActivityUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 302

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.sharePointActivityUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "visitedPage": 56, 
      "viewedOrEdited": 163, 
      "synced": 7, 
      "sharedInternally": 10, 
      "sharedExternally": 1, 
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
    "Error: /api-reference/beta/api/reportroot-getsharepointactivityusercounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
