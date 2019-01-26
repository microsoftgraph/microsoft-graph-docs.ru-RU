---
title: 'reportRoot: getYammerDeviceUsageDistributionUserCounts'
description: Получите сведения о количестве пользователей с разбивкой по типам устройств.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 407960889f20178b03ad3865959d99cb8a1a417b
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577314"
---
# <a name="reportroot-getyammerdeviceusagedistributionusercounts"></a><span data-ttu-id="63c14-103">reportRoot: getYammerDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="63c14-103">reportRoot: getYammerDeviceUsageDistributionUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63c14-104">Получите сведения о количестве пользователей с разбивкой по типам устройств.</span><span class="sxs-lookup"><span data-stu-id="63c14-104">Get the number of users by device type.</span></span>

> <span data-ttu-id="63c14-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="63c14-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="63c14-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="63c14-106">Permissions</span></span>

<span data-ttu-id="63c14-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63c14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="63c14-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="63c14-109">Permission type</span></span>                        | <span data-ttu-id="63c14-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="63c14-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="63c14-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="63c14-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="63c14-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="63c14-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="63c14-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="63c14-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63c14-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63c14-114">Not supported.</span></span>                           |
| <span data-ttu-id="63c14-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="63c14-115">Application</span></span>                            | <span data-ttu-id="63c14-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="63c14-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="63c14-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="63c14-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="63c14-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="63c14-118">Function parameters</span></span>

<span data-ttu-id="63c14-119">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="63c14-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="63c14-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="63c14-120">Parameter</span></span> | <span data-ttu-id="63c14-121">Тип</span><span class="sxs-lookup"><span data-stu-id="63c14-121">Type</span></span>   | <span data-ttu-id="63c14-122">Описание</span><span class="sxs-lookup"><span data-stu-id="63c14-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="63c14-123">period</span><span class="sxs-lookup"><span data-stu-id="63c14-123">period</span></span>    | <span data-ttu-id="63c14-124">строка</span><span class="sxs-lookup"><span data-stu-id="63c14-124">string</span></span> | <span data-ttu-id="63c14-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="63c14-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="63c14-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="63c14-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="63c14-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="63c14-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="63c14-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="63c14-128">Required.</span></span> |

<span data-ttu-id="63c14-129">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="63c14-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="63c14-130">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="63c14-130">The default output type is text/csv.</span></span> <span data-ttu-id="63c14-131">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="63c14-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="63c14-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="63c14-132">Request headers</span></span>

| <span data-ttu-id="63c14-133">Имя</span><span class="sxs-lookup"><span data-stu-id="63c14-133">Name</span></span>          | <span data-ttu-id="63c14-134">Описание</span><span class="sxs-lookup"><span data-stu-id="63c14-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="63c14-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="63c14-135">Authorization</span></span> | <span data-ttu-id="63c14-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="63c14-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="63c14-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="63c14-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="63c14-139">CSV</span><span class="sxs-lookup"><span data-stu-id="63c14-139">CSV</span></span>

<span data-ttu-id="63c14-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="63c14-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="63c14-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="63c14-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="63c14-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="63c14-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="63c14-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="63c14-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="63c14-144">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="63c14-144">Report Refresh Date</span></span>
- <span data-ttu-id="63c14-145">"Web" (Интернет);</span><span class="sxs-lookup"><span data-stu-id="63c14-145">Web</span></span>
- <span data-ttu-id="63c14-146">"Windows Phone";</span><span class="sxs-lookup"><span data-stu-id="63c14-146">Windows Phone</span></span>
- <span data-ttu-id="63c14-147">"Android Phone" (Телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="63c14-147">Android Phone</span></span>
- <span data-ttu-id="63c14-148">"iPhone";</span><span class="sxs-lookup"><span data-stu-id="63c14-148">iPhone</span></span>
- <span data-ttu-id="63c14-149">iPad</span><span class="sxs-lookup"><span data-stu-id="63c14-149">iPad</span></span>
- <span data-ttu-id="63c14-150">Other (другие)</span><span class="sxs-lookup"><span data-stu-id="63c14-150">Other</span></span>
- <span data-ttu-id="63c14-151">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="63c14-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="63c14-152">JSON</span><span class="sxs-lookup"><span data-stu-id="63c14-152">JSON</span></span>

<span data-ttu-id="63c14-153">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[yammerDeviceUsageDistributionUserCounts](../resources/yammerdeviceusagedistributionusercounts.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="63c14-153">If successful, this method returns a `200 OK` response code and a **[yammerDeviceUsageDistributionUserCounts](../resources/yammerdeviceusagedistributionusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63c14-154">Пример</span><span class="sxs-lookup"><span data-stu-id="63c14-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="63c14-155">CSV</span><span class="sxs-lookup"><span data-stu-id="63c14-155">CSV</span></span>

<span data-ttu-id="63c14-156">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="63c14-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="63c14-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="63c14-157">Request</span></span>

<span data-ttu-id="63c14-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="63c14-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusagedistributionusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="63c14-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="63c14-159">Response</span></span>

<span data-ttu-id="63c14-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="63c14-160">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="63c14-161">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="63c14-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iPhone,iPad,Other,Report Period
```

### <a name="json"></a><span data-ttu-id="63c14-162">JSON</span><span class="sxs-lookup"><span data-stu-id="63c14-162">JSON</span></span>

<span data-ttu-id="63c14-163">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="63c14-163">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="63c14-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="63c14-164">Request</span></span>

<span data-ttu-id="63c14-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="63c14-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusagedistributionusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageDistributionUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="63c14-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="63c14-166">Response</span></span>

<span data-ttu-id="63c14-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="63c14-167">The following is an example of the response.</span></span>

> <span data-ttu-id="63c14-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="63c14-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerDeviceUsageDistributionUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 271

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerDeviceUsageDistributionUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "web": 138, 
      "windowsPhone": 1, 
      "androidPhone": 29, 
      "iPhone": 40, 
      "iPad": 2, 
      "other": 2, 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getyammerdeviceusagedistributionusercounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
