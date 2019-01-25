---
title: 'reportRoot: getYammerDeviceUsageDistributionUserCounts'
description: Получите сведения о количестве пользователей с разбивкой по типам устройств.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 5d8f74926d6cbfee6a22f9a6789fb232f1166b55
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511375"
---
# <a name="reportroot-getyammerdeviceusagedistributionusercounts"></a><span data-ttu-id="5b579-103">reportRoot: getYammerDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="5b579-103">reportRoot: getYammerDeviceUsageDistributionUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b579-104">Получите сведения о количестве пользователей с разбивкой по типам устройств.</span><span class="sxs-lookup"><span data-stu-id="5b579-104">Get the number of users by device type.</span></span>

> <span data-ttu-id="5b579-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="5b579-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="5b579-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5b579-106">Permissions</span></span>

<span data-ttu-id="5b579-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b579-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5b579-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5b579-109">Permission type</span></span>                        | <span data-ttu-id="5b579-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5b579-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="5b579-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5b579-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5b579-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b579-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="5b579-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5b579-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b579-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b579-114">Not supported.</span></span>                           |
| <span data-ttu-id="5b579-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5b579-115">Application</span></span>                            | <span data-ttu-id="5b579-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b579-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="5b579-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b579-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="5b579-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="5b579-118">Function parameters</span></span>

<span data-ttu-id="5b579-119">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="5b579-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="5b579-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="5b579-120">Parameter</span></span> | <span data-ttu-id="5b579-121">Тип</span><span class="sxs-lookup"><span data-stu-id="5b579-121">Type</span></span>   | <span data-ttu-id="5b579-122">Описание</span><span class="sxs-lookup"><span data-stu-id="5b579-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="5b579-123">period</span><span class="sxs-lookup"><span data-stu-id="5b579-123">period</span></span>    | <span data-ttu-id="5b579-124">строка</span><span class="sxs-lookup"><span data-stu-id="5b579-124">string</span></span> | <span data-ttu-id="5b579-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="5b579-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="5b579-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="5b579-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="5b579-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="5b579-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="5b579-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b579-128">Required.</span></span> |

<span data-ttu-id="5b579-129">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5b579-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="5b579-130">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="5b579-130">The default output type is text/csv.</span></span> <span data-ttu-id="5b579-131">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="5b579-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5b579-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5b579-132">Request headers</span></span>

| <span data-ttu-id="5b579-133">Имя</span><span class="sxs-lookup"><span data-stu-id="5b579-133">Name</span></span>          | <span data-ttu-id="5b579-134">Описание</span><span class="sxs-lookup"><span data-stu-id="5b579-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="5b579-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5b579-135">Authorization</span></span> | <span data-ttu-id="5b579-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b579-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="5b579-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="5b579-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="5b579-139">CSV</span><span class="sxs-lookup"><span data-stu-id="5b579-139">CSV</span></span>

<span data-ttu-id="5b579-140">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="5b579-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="5b579-141">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="5b579-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="5b579-142">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="5b579-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="5b579-143">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="5b579-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="5b579-144">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="5b579-144">Report Refresh Date</span></span>
- <span data-ttu-id="5b579-145">"Web" (Интернет);</span><span class="sxs-lookup"><span data-stu-id="5b579-145">Web</span></span>
- <span data-ttu-id="5b579-146">"Windows Phone";</span><span class="sxs-lookup"><span data-stu-id="5b579-146">Windows Phone</span></span>
- <span data-ttu-id="5b579-147">"Android Phone" (Телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="5b579-147">Android Phone</span></span>
- <span data-ttu-id="5b579-148">"iPhone";</span><span class="sxs-lookup"><span data-stu-id="5b579-148">iPhone</span></span>
- <span data-ttu-id="5b579-149">iPad</span><span class="sxs-lookup"><span data-stu-id="5b579-149">iPad</span></span>
- <span data-ttu-id="5b579-150">Other (другие)</span><span class="sxs-lookup"><span data-stu-id="5b579-150">Other</span></span>
- <span data-ttu-id="5b579-151">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="5b579-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="5b579-152">JSON</span><span class="sxs-lookup"><span data-stu-id="5b579-152">JSON</span></span>

<span data-ttu-id="5b579-153">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[yammerDeviceUsageDistributionUserCounts](../resources/yammerdeviceusagedistributionusercounts.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5b579-153">If successful, this method returns a `200 OK` response code and a **[yammerDeviceUsageDistributionUserCounts](../resources/yammerdeviceusagedistributionusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b579-154">Пример</span><span class="sxs-lookup"><span data-stu-id="5b579-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="5b579-155">CSV</span><span class="sxs-lookup"><span data-stu-id="5b579-155">CSV</span></span>

<span data-ttu-id="5b579-156">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="5b579-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="5b579-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b579-157">Request</span></span>

<span data-ttu-id="5b579-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5b579-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusagedistributionusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="5b579-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="5b579-159">Response</span></span>

<span data-ttu-id="5b579-160">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5b579-160">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="5b579-161">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="5b579-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="5b579-162">JSON</span><span class="sxs-lookup"><span data-stu-id="5b579-162">JSON</span></span>

<span data-ttu-id="5b579-163">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="5b579-163">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="5b579-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b579-164">Request</span></span>

<span data-ttu-id="5b579-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5b579-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusagedistributionusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageDistributionUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="5b579-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="5b579-166">Response</span></span>

<span data-ttu-id="5b579-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5b579-167">The following is an example of the response.</span></span>

> <span data-ttu-id="5b579-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5b579-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
