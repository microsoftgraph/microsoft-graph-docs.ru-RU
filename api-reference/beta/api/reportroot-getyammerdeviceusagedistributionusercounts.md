---
title: 'reportRoot: getYammerDeviceUsageDistributionUserCounts'
description: Получите сведения о количестве пользователей с разбивкой по типам устройств.
localization_priority: Normal
ms.openlocfilehash: 96e379c63f2f00ef3c6616df0405ae779f6bc8ff
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886179"
---
# <a name="reportroot-getyammerdeviceusagedistributionusercounts"></a><span data-ttu-id="618db-103">reportRoot: getYammerDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="618db-103">reportRoot: getYammerDeviceUsageDistributionUserCounts</span></span>

> <span data-ttu-id="618db-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="618db-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="618db-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="618db-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="618db-106">Получите сведения о количестве пользователей с разбивкой по типам устройств.</span><span class="sxs-lookup"><span data-stu-id="618db-106">Get the number of users by device type.</span></span>

> <span data-ttu-id="618db-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="618db-107">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="618db-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="618db-108">Permissions</span></span>

<span data-ttu-id="618db-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="618db-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="618db-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="618db-111">Permission type</span></span>                        | <span data-ttu-id="618db-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="618db-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="618db-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="618db-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="618db-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="618db-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="618db-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="618db-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="618db-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="618db-116">Not supported.</span></span>                           |
| <span data-ttu-id="618db-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="618db-117">Application</span></span>                            | <span data-ttu-id="618db-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="618db-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="618db-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="618db-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="618db-120">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="618db-120">Function parameters</span></span>

<span data-ttu-id="618db-121">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="618db-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="618db-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="618db-122">Parameter</span></span> | <span data-ttu-id="618db-123">Тип</span><span class="sxs-lookup"><span data-stu-id="618db-123">Type</span></span>   | <span data-ttu-id="618db-124">Описание</span><span class="sxs-lookup"><span data-stu-id="618db-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="618db-125">period</span><span class="sxs-lookup"><span data-stu-id="618db-125">period</span></span>    | <span data-ttu-id="618db-126">строка</span><span class="sxs-lookup"><span data-stu-id="618db-126">string</span></span> | <span data-ttu-id="618db-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="618db-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="618db-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="618db-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="618db-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="618db-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="618db-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="618db-130">Required.</span></span> |

<span data-ttu-id="618db-131">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="618db-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="618db-132">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="618db-132">The default output type is text/csv.</span></span> <span data-ttu-id="618db-133">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="618db-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="618db-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="618db-134">Request headers</span></span>

| <span data-ttu-id="618db-135">Имя</span><span class="sxs-lookup"><span data-stu-id="618db-135">Name</span></span>          | <span data-ttu-id="618db-136">Описание</span><span class="sxs-lookup"><span data-stu-id="618db-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="618db-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="618db-137">Authorization</span></span> | <span data-ttu-id="618db-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="618db-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="618db-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="618db-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="618db-141">CSV</span><span class="sxs-lookup"><span data-stu-id="618db-141">CSV</span></span>

<span data-ttu-id="618db-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="618db-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="618db-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="618db-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="618db-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="618db-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="618db-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="618db-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="618db-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="618db-146">Report Refresh Date</span></span>
- <span data-ttu-id="618db-147">"Web" (Интернет);</span><span class="sxs-lookup"><span data-stu-id="618db-147">Web</span></span>
- <span data-ttu-id="618db-148">"Windows Phone";</span><span class="sxs-lookup"><span data-stu-id="618db-148">Windows Phone</span></span>
- <span data-ttu-id="618db-149">"Android Phone" (Телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="618db-149">Android Phone</span></span>
- <span data-ttu-id="618db-150">"iPhone";</span><span class="sxs-lookup"><span data-stu-id="618db-150">iPhone</span></span>
- <span data-ttu-id="618db-151">iPad</span><span class="sxs-lookup"><span data-stu-id="618db-151">iPad</span></span>
- <span data-ttu-id="618db-152">Other (другие)</span><span class="sxs-lookup"><span data-stu-id="618db-152">Other</span></span>
- <span data-ttu-id="618db-153">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="618db-153">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="618db-154">JSON</span><span class="sxs-lookup"><span data-stu-id="618db-154">JSON</span></span>

<span data-ttu-id="618db-155">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[yammerDeviceUsageDistributionUserCounts](../resources/yammerdeviceusagedistributionusercounts.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="618db-155">If successful, this method returns a `200 OK` response code and a **[yammerDeviceUsageDistributionUserCounts](../resources/yammerdeviceusagedistributionusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="618db-156">Пример</span><span class="sxs-lookup"><span data-stu-id="618db-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="618db-157">CSV</span><span class="sxs-lookup"><span data-stu-id="618db-157">CSV</span></span>

<span data-ttu-id="618db-158">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="618db-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="618db-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="618db-159">Request</span></span>

<span data-ttu-id="618db-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="618db-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusagedistributionusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="618db-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="618db-161">Response</span></span>

<span data-ttu-id="618db-162">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="618db-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="618db-163">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="618db-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="618db-164">JSON</span><span class="sxs-lookup"><span data-stu-id="618db-164">JSON</span></span>

<span data-ttu-id="618db-165">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="618db-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="618db-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="618db-166">Request</span></span>

<span data-ttu-id="618db-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="618db-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusagedistributionusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageDistributionUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="618db-168">Ответ</span><span class="sxs-lookup"><span data-stu-id="618db-168">Response</span></span>

<span data-ttu-id="618db-169">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="618db-169">The following is an example of the response.</span></span>

> <span data-ttu-id="618db-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="618db-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
