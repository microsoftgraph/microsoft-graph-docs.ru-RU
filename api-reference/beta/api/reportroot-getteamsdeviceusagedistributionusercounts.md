---
title: 'reportRoot: getTeamsDeviceUsageDistributionUserCounts'
description: Получение количества уникальных пользователей Microsoft Teams с сортировкой по типам устройств за выбранный период.
localization_priority: Normal
ms.openlocfilehash: 274fd212d936df75122c5c7acafeae12a2e528b1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830340"
---
# <a name="reportroot-getteamsdeviceusagedistributionusercounts"></a><span data-ttu-id="25037-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="25037-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span></span>

> <span data-ttu-id="25037-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="25037-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="25037-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25037-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="25037-106">Получение количества уникальных пользователей Microsoft Teams с сортировкой по типам устройств за выбранный период.</span><span class="sxs-lookup"><span data-stu-id="25037-106">Get the number of Microsoft Teams unique users by device type over the selected time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="25037-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="25037-107">Permissions</span></span>

<span data-ttu-id="25037-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25037-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="25037-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="25037-110">Permission type</span></span>                        | <span data-ttu-id="25037-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="25037-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="25037-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="25037-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="25037-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="25037-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="25037-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="25037-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25037-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25037-115">Not supported.</span></span>                           |
| <span data-ttu-id="25037-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="25037-116">Application</span></span>                            | <span data-ttu-id="25037-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="25037-117">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="25037-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="25037-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="25037-119">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="25037-119">Function parameters</span></span>

<span data-ttu-id="25037-120">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="25037-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="25037-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="25037-121">Parameter</span></span> | <span data-ttu-id="25037-122">Тип</span><span class="sxs-lookup"><span data-stu-id="25037-122">Type</span></span>   | <span data-ttu-id="25037-123">Описание</span><span class="sxs-lookup"><span data-stu-id="25037-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="25037-124">period</span><span class="sxs-lookup"><span data-stu-id="25037-124">period</span></span>    | <span data-ttu-id="25037-125">строка</span><span class="sxs-lookup"><span data-stu-id="25037-125">string</span></span> | <span data-ttu-id="25037-126">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="25037-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="25037-127">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="25037-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="25037-128">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="25037-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="25037-129">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="25037-129">Required.</span></span> |

<span data-ttu-id="25037-130">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="25037-130">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="25037-131">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="25037-131">The default output type is text/csv.</span></span> <span data-ttu-id="25037-132">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="25037-132">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="25037-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="25037-133">Request headers</span></span>

| <span data-ttu-id="25037-134">Имя</span><span class="sxs-lookup"><span data-stu-id="25037-134">Name</span></span>          | <span data-ttu-id="25037-135">Описание</span><span class="sxs-lookup"><span data-stu-id="25037-135">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="25037-136">Авторизация</span><span class="sxs-lookup"><span data-stu-id="25037-136">Authorization</span></span> | <span data-ttu-id="25037-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="25037-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="25037-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="25037-139">Response</span></span>

### <a name="csv"></a><span data-ttu-id="25037-140">CSV</span><span class="sxs-lookup"><span data-stu-id="25037-140">CSV</span></span>

<span data-ttu-id="25037-141">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="25037-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="25037-142">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="25037-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="25037-143">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="25037-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="25037-144">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="25037-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="25037-145">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="25037-145">Report Refresh Date</span></span>
- <span data-ttu-id="25037-146">"Web" (Интернет);</span><span class="sxs-lookup"><span data-stu-id="25037-146">Web</span></span>
- <span data-ttu-id="25037-147">"Windows Phone";</span><span class="sxs-lookup"><span data-stu-id="25037-147">Windows Phone</span></span>
- <span data-ttu-id="25037-148">"Android Phone" (Телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="25037-148">Android Phone</span></span>
- <span data-ttu-id="25037-149">"iOS";</span><span class="sxs-lookup"><span data-stu-id="25037-149">iOS</span></span>
- <span data-ttu-id="25037-150">"Mac";</span><span class="sxs-lookup"><span data-stu-id="25037-150">Mac</span></span>
- <span data-ttu-id="25037-151">"Windows";</span><span class="sxs-lookup"><span data-stu-id="25037-151">Windows</span></span>
- <span data-ttu-id="25037-152">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="25037-152">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="25037-153">JSON</span><span class="sxs-lookup"><span data-stu-id="25037-153">JSON</span></span>

<span data-ttu-id="25037-154">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="25037-154">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25037-155">Пример</span><span class="sxs-lookup"><span data-stu-id="25037-155">Example</span></span>

### <a name="csv"></a><span data-ttu-id="25037-156">CSV</span><span class="sxs-lookup"><span data-stu-id="25037-156">CSV</span></span>

<span data-ttu-id="25037-157">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="25037-157">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="25037-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="25037-158">Request</span></span>

<span data-ttu-id="25037-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="25037-159">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="25037-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="25037-160">Response</span></span>

<span data-ttu-id="25037-161">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="25037-161">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="25037-162">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="25037-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="25037-163">JSON</span><span class="sxs-lookup"><span data-stu-id="25037-163">JSON</span></span>

<span data-ttu-id="25037-164">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="25037-164">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="25037-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="25037-165">Request</span></span>

<span data-ttu-id="25037-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="25037-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="25037-167">Ответ</span><span class="sxs-lookup"><span data-stu-id="25037-167">Response</span></span>

<span data-ttu-id="25037-168">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="25037-168">The following is an example of the response.</span></span>

> <span data-ttu-id="25037-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="25037-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
