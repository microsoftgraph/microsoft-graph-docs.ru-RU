---
title: 'reportRoot: getTeamsDeviceUsageDistributionUserCounts'
description: Получение количества уникальных пользователей Microsoft Teams с сортировкой по типам устройств за выбранный период.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: d0e83451b0be65e689549d415ef66fe5c9534687
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575879"
---
# <a name="reportroot-getteamsdeviceusagedistributionusercounts"></a><span data-ttu-id="0f74b-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="0f74b-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f74b-104">Получение количества уникальных пользователей Microsoft Teams с сортировкой по типам устройств за выбранный период.</span><span class="sxs-lookup"><span data-stu-id="0f74b-104">Get the number of Microsoft Teams unique users by device type over the selected time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="0f74b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0f74b-105">Permissions</span></span>

<span data-ttu-id="0f74b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f74b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0f74b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0f74b-108">Permission type</span></span>                        | <span data-ttu-id="0f74b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0f74b-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="0f74b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0f74b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0f74b-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0f74b-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="0f74b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0f74b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f74b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f74b-113">Not supported.</span></span>                           |
| <span data-ttu-id="0f74b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0f74b-114">Application</span></span>                            | <span data-ttu-id="0f74b-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0f74b-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="0f74b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0f74b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="0f74b-117">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="0f74b-117">Function parameters</span></span>

<span data-ttu-id="0f74b-118">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="0f74b-118">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="0f74b-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="0f74b-119">Parameter</span></span> | <span data-ttu-id="0f74b-120">Тип</span><span class="sxs-lookup"><span data-stu-id="0f74b-120">Type</span></span>   | <span data-ttu-id="0f74b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="0f74b-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="0f74b-122">period</span><span class="sxs-lookup"><span data-stu-id="0f74b-122">period</span></span>    | <span data-ttu-id="0f74b-123">строка</span><span class="sxs-lookup"><span data-stu-id="0f74b-123">string</span></span> | <span data-ttu-id="0f74b-124">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="0f74b-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="0f74b-125">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="0f74b-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="0f74b-126">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="0f74b-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="0f74b-127">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0f74b-127">Required.</span></span> |

<span data-ttu-id="0f74b-128">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0f74b-128">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="0f74b-129">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="0f74b-129">The default output type is text/csv.</span></span> <span data-ttu-id="0f74b-130">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="0f74b-130">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0f74b-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0f74b-131">Request headers</span></span>

| <span data-ttu-id="0f74b-132">Имя</span><span class="sxs-lookup"><span data-stu-id="0f74b-132">Name</span></span>          | <span data-ttu-id="0f74b-133">Описание</span><span class="sxs-lookup"><span data-stu-id="0f74b-133">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="0f74b-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0f74b-134">Authorization</span></span> | <span data-ttu-id="0f74b-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0f74b-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="0f74b-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f74b-137">Response</span></span>

### <a name="csv"></a><span data-ttu-id="0f74b-138">CSV</span><span class="sxs-lookup"><span data-stu-id="0f74b-138">CSV</span></span>

<span data-ttu-id="0f74b-139">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="0f74b-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="0f74b-140">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="0f74b-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="0f74b-141">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="0f74b-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="0f74b-142">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="0f74b-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="0f74b-143">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="0f74b-143">Report Refresh Date</span></span>
- <span data-ttu-id="0f74b-144">"Web" (Интернет);</span><span class="sxs-lookup"><span data-stu-id="0f74b-144">Web</span></span>
- <span data-ttu-id="0f74b-145">"Windows Phone";</span><span class="sxs-lookup"><span data-stu-id="0f74b-145">Windows Phone</span></span>
- <span data-ttu-id="0f74b-146">"Android Phone" (Телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="0f74b-146">Android Phone</span></span>
- <span data-ttu-id="0f74b-147">"iOS";</span><span class="sxs-lookup"><span data-stu-id="0f74b-147">iOS</span></span>
- <span data-ttu-id="0f74b-148">"Mac";</span><span class="sxs-lookup"><span data-stu-id="0f74b-148">Mac</span></span>
- <span data-ttu-id="0f74b-149">"Windows";</span><span class="sxs-lookup"><span data-stu-id="0f74b-149">Windows</span></span>
- <span data-ttu-id="0f74b-150">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="0f74b-150">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="0f74b-151">JSON</span><span class="sxs-lookup"><span data-stu-id="0f74b-151">JSON</span></span>

<span data-ttu-id="0f74b-152">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0f74b-152">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f74b-153">Пример</span><span class="sxs-lookup"><span data-stu-id="0f74b-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="0f74b-154">CSV</span><span class="sxs-lookup"><span data-stu-id="0f74b-154">CSV</span></span>

<span data-ttu-id="0f74b-155">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="0f74b-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="0f74b-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="0f74b-156">Request</span></span>

<span data-ttu-id="0f74b-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0f74b-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="0f74b-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f74b-158">Response</span></span>

<span data-ttu-id="0f74b-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0f74b-159">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="0f74b-160">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="0f74b-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iOS,Mac,Windows,Report Period
```

### <a name="json"></a><span data-ttu-id="0f74b-161">JSON</span><span class="sxs-lookup"><span data-stu-id="0f74b-161">JSON</span></span>

<span data-ttu-id="0f74b-162">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="0f74b-162">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="0f74b-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="0f74b-163">Request</span></span>

<span data-ttu-id="0f74b-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0f74b-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="0f74b-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f74b-165">Response</span></span>

<span data-ttu-id="0f74b-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0f74b-166">The following is an example of the response.</span></span>

> <span data-ttu-id="0f74b-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0f74b-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsDeviceUsageDistributionUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 243

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsDeviceUsageDistributionUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "web": 51, 
      "windowsPhone": 2, 
      "androidPhone": 34, 
      "ios": 76, 
      "mac": 40, 
      "windows": 491, 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getteamsdeviceusagedistributionusercounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
