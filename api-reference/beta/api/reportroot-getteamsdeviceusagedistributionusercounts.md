---
title: 'reportRoot: getTeamsDeviceUsageDistributionUserCounts'
description: Получение количества уникальных пользователей Microsoft Teams с сортировкой по типам устройств за выбранный период.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 397592a7333a9aee9435a3e2e073645d6e5cacd0
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33336457"
---
# <a name="reportroot-getteamsdeviceusagedistributionusercounts"></a><span data-ttu-id="2393a-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="2393a-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2393a-104">Получение количества уникальных пользователей Microsoft Teams с сортировкой по типам устройств за выбранный период.</span><span class="sxs-lookup"><span data-stu-id="2393a-104">Get the number of Microsoft Teams unique users by device type over the selected time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="2393a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2393a-105">Permissions</span></span>

<span data-ttu-id="2393a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2393a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2393a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2393a-108">Permission type</span></span>                        | <span data-ttu-id="2393a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2393a-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="2393a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2393a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="2393a-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2393a-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="2393a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2393a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2393a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2393a-113">Not supported.</span></span>                           |
| <span data-ttu-id="2393a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2393a-114">Application</span></span>                            | <span data-ttu-id="2393a-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2393a-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="2393a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2393a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="2393a-117">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="2393a-117">Function parameters</span></span>

<span data-ttu-id="2393a-118">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="2393a-118">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="2393a-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="2393a-119">Parameter</span></span> | <span data-ttu-id="2393a-120">Тип</span><span class="sxs-lookup"><span data-stu-id="2393a-120">Type</span></span>   | <span data-ttu-id="2393a-121">Описание</span><span class="sxs-lookup"><span data-stu-id="2393a-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="2393a-122">period</span><span class="sxs-lookup"><span data-stu-id="2393a-122">period</span></span>    | <span data-ttu-id="2393a-123">string</span><span class="sxs-lookup"><span data-stu-id="2393a-123">string</span></span> | <span data-ttu-id="2393a-124">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="2393a-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="2393a-125">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="2393a-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="2393a-126">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="2393a-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="2393a-127">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2393a-127">Required.</span></span> |

<span data-ttu-id="2393a-128">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="2393a-128">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="2393a-129">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="2393a-129">The default output type is text/csv.</span></span> <span data-ttu-id="2393a-130">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="2393a-130">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2393a-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2393a-131">Request headers</span></span>

| <span data-ttu-id="2393a-132">Имя</span><span class="sxs-lookup"><span data-stu-id="2393a-132">Name</span></span>          | <span data-ttu-id="2393a-133">Описание</span><span class="sxs-lookup"><span data-stu-id="2393a-133">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="2393a-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2393a-134">Authorization</span></span> | <span data-ttu-id="2393a-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2393a-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="2393a-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="2393a-137">Response</span></span>

### <a name="csv"></a><span data-ttu-id="2393a-138">CSV</span><span class="sxs-lookup"><span data-stu-id="2393a-138">CSV</span></span>

<span data-ttu-id="2393a-139">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="2393a-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="2393a-140">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="2393a-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="2393a-141">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="2393a-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="2393a-142">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="2393a-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="2393a-143">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="2393a-143">Report Refresh Date</span></span>
- <span data-ttu-id="2393a-144">"Web" (Интернет);</span><span class="sxs-lookup"><span data-stu-id="2393a-144">Web</span></span>
- <span data-ttu-id="2393a-145">"Windows Phone";</span><span class="sxs-lookup"><span data-stu-id="2393a-145">Windows Phone</span></span>
- <span data-ttu-id="2393a-146">"Android Phone" (Телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="2393a-146">Android Phone</span></span>
- <span data-ttu-id="2393a-147">"iOS";</span><span class="sxs-lookup"><span data-stu-id="2393a-147">iOS</span></span>
- <span data-ttu-id="2393a-148">"Mac";</span><span class="sxs-lookup"><span data-stu-id="2393a-148">Mac</span></span>
- <span data-ttu-id="2393a-149">"Windows";</span><span class="sxs-lookup"><span data-stu-id="2393a-149">Windows</span></span>
- <span data-ttu-id="2393a-150">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="2393a-150">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="2393a-151">JSON</span><span class="sxs-lookup"><span data-stu-id="2393a-151">JSON</span></span>

<span data-ttu-id="2393a-152">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[теамсдевицеусажедистрибутионусеркаунтс](../resources/teamsdeviceusagedistributionusercounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2393a-152">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2393a-153">Пример</span><span class="sxs-lookup"><span data-stu-id="2393a-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="2393a-154">CSV</span><span class="sxs-lookup"><span data-stu-id="2393a-154">CSV</span></span>

<span data-ttu-id="2393a-155">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="2393a-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="2393a-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="2393a-156">Request</span></span>

<span data-ttu-id="2393a-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2393a-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="2393a-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="2393a-158">Response</span></span>

<span data-ttu-id="2393a-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2393a-159">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="2393a-160">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="2393a-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="2393a-161">JSON</span><span class="sxs-lookup"><span data-stu-id="2393a-161">JSON</span></span>

<span data-ttu-id="2393a-162">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="2393a-162">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="2393a-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="2393a-163">Request</span></span>

<span data-ttu-id="2393a-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2393a-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="2393a-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="2393a-165">Response</span></span>

<span data-ttu-id="2393a-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2393a-166">The following is an example of the response.</span></span>

> <span data-ttu-id="2393a-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2393a-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
