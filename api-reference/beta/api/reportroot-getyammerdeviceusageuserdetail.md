---
title: 'reportRoot: getYammerDeviceUsageUserDetail function'
description: Получение сведений об использовании устройства с Yammer с разбивкой по пользователям.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 33b9b2a25da32de28179d9982dbd67ca820b3ce9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33331785"
---
# <a name="reportroot-getyammerdeviceusageuserdetail-function"></a><span data-ttu-id="90fcc-103">reportRoot: getYammerDeviceUsageUserDetail function</span><span class="sxs-lookup"><span data-stu-id="90fcc-103">reportRoot: getYammerDeviceUsageUserDetail function</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90fcc-104">Получение сведений об использовании устройства с Yammer с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="90fcc-104">Get details about Yammer device usage by user.</span></span>

> <span data-ttu-id="90fcc-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: использование устройств с Yammer](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="90fcc-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="90fcc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="90fcc-106">Permissions</span></span>

<span data-ttu-id="90fcc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90fcc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="90fcc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="90fcc-109">Permission type</span></span>                        | <span data-ttu-id="90fcc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="90fcc-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="90fcc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="90fcc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="90fcc-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="90fcc-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="90fcc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="90fcc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90fcc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90fcc-114">Not supported.</span></span>                           |
| <span data-ttu-id="90fcc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="90fcc-115">Application</span></span>                            | <span data-ttu-id="90fcc-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="90fcc-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="90fcc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="90fcc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserDetail(period='{period_value}')
GET /reports/getYammerDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="90fcc-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="90fcc-118">Function parameters</span></span>

<span data-ttu-id="90fcc-119">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="90fcc-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="90fcc-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="90fcc-120">Parameter</span></span> | <span data-ttu-id="90fcc-121">Тип</span><span class="sxs-lookup"><span data-stu-id="90fcc-121">Type</span></span>   | <span data-ttu-id="90fcc-122">Описание</span><span class="sxs-lookup"><span data-stu-id="90fcc-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="90fcc-123">period</span><span class="sxs-lookup"><span data-stu-id="90fcc-123">period</span></span>    | <span data-ttu-id="90fcc-124">string</span><span class="sxs-lookup"><span data-stu-id="90fcc-124">string</span></span> | <span data-ttu-id="90fcc-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="90fcc-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="90fcc-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="90fcc-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="90fcc-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="90fcc-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="90fcc-128">date</span><span class="sxs-lookup"><span data-stu-id="90fcc-128">date</span></span>      | <span data-ttu-id="90fcc-129">Date</span><span class="sxs-lookup"><span data-stu-id="90fcc-129">Date</span></span>   | <span data-ttu-id="90fcc-130">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="90fcc-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="90fcc-131">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="90fcc-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="90fcc-132">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="90fcc-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="90fcc-133">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="90fcc-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="90fcc-134">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="90fcc-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="90fcc-135">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="90fcc-135">The default output type is text/csv.</span></span> <span data-ttu-id="90fcc-136">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="90fcc-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="90fcc-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="90fcc-137">Request headers</span></span>

| <span data-ttu-id="90fcc-138">Имя</span><span class="sxs-lookup"><span data-stu-id="90fcc-138">Name</span></span>          | <span data-ttu-id="90fcc-139">Описание</span><span class="sxs-lookup"><span data-stu-id="90fcc-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="90fcc-140">Авторизация</span><span class="sxs-lookup"><span data-stu-id="90fcc-140">Authorization</span></span> | <span data-ttu-id="90fcc-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="90fcc-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="90fcc-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="90fcc-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="90fcc-144">CSV</span><span class="sxs-lookup"><span data-stu-id="90fcc-144">CSV</span></span>

<span data-ttu-id="90fcc-145">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="90fcc-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="90fcc-146">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="90fcc-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="90fcc-147">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="90fcc-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="90fcc-148">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="90fcc-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="90fcc-149">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="90fcc-149">Report Refresh Date</span></span>
- <span data-ttu-id="90fcc-150">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="90fcc-150">User Principal Name</span></span>
- <span data-ttu-id="90fcc-151">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="90fcc-151">Display Name</span></span>
- <span data-ttu-id="90fcc-152">"User State" (Состояние пользователя);</span><span class="sxs-lookup"><span data-stu-id="90fcc-152">User State</span></span>
- <span data-ttu-id="90fcc-153">"State Change Date" (Дата изменения состояния);</span><span class="sxs-lookup"><span data-stu-id="90fcc-153">State Change Date</span></span>
- <span data-ttu-id="90fcc-154">"Last Activity Date" (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="90fcc-154">Last Activity Date</span></span>
- <span data-ttu-id="90fcc-155">"Used Web" (Используемое веб-приложение);</span><span class="sxs-lookup"><span data-stu-id="90fcc-155">Used Web</span></span>
- <span data-ttu-id="90fcc-156">"Used Windows Phone" (Используемое устройство Windows Phone);</span><span class="sxs-lookup"><span data-stu-id="90fcc-156">Used Windows Phone</span></span>
- <span data-ttu-id="90fcc-157">"Used Android Phone" (Используемый телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="90fcc-157">Used Android Phone</span></span>
- <span data-ttu-id="90fcc-158">"Used iPhone" (Используемый телефон iPhone);</span><span class="sxs-lookup"><span data-stu-id="90fcc-158">Used iPhone</span></span>
- <span data-ttu-id="90fcc-159">"Used iPad" (Используемое устройство iPad);</span><span class="sxs-lookup"><span data-stu-id="90fcc-159">Used iPad</span></span>
- <span data-ttu-id="90fcc-160">"Used Others" (Другое используемое);</span><span class="sxs-lookup"><span data-stu-id="90fcc-160">Used Others</span></span>
- <span data-ttu-id="90fcc-161">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="90fcc-161">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="90fcc-162">JSON</span><span class="sxs-lookup"><span data-stu-id="90fcc-162">JSON</span></span>

<span data-ttu-id="90fcc-163">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[яммердевицеусажеусердетаил](../resources/yammerdeviceusageuserdetail.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="90fcc-163">If successful, this method returns a `200 OK` response code and a **[yammerDeviceUsageUserDetail](../resources/yammerdeviceusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="90fcc-164">Размер страницы по умолчанию для этого запроса составляет 200 элементов.</span><span class="sxs-lookup"><span data-stu-id="90fcc-164">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="90fcc-165">Пример</span><span class="sxs-lookup"><span data-stu-id="90fcc-165">Example</span></span>

### <a name="csv"></a><span data-ttu-id="90fcc-166">CSV</span><span class="sxs-lookup"><span data-stu-id="90fcc-166">CSV</span></span>

<span data-ttu-id="90fcc-167">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="90fcc-167">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="90fcc-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="90fcc-168">Request</span></span>

<span data-ttu-id="90fcc-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="90fcc-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusageuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="90fcc-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="90fcc-170">Response</span></span>

<span data-ttu-id="90fcc-171">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="90fcc-171">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="90fcc-172">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="90fcc-172">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,User State,State Change Date,Last Activity Date,Used Web,Used Windows Phone,Used Android Phone,Used iPhone,Used iPad,Used Others,Report Period
```

### <a name="json"></a><span data-ttu-id="90fcc-173">JSON</span><span class="sxs-lookup"><span data-stu-id="90fcc-173">JSON</span></span>

<span data-ttu-id="90fcc-174">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="90fcc-174">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="90fcc-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="90fcc-175">Request</span></span>

<span data-ttu-id="90fcc-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="90fcc-176">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusageuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="90fcc-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="90fcc-177">Response</span></span>

<span data-ttu-id="90fcc-178">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="90fcc-178">The following is an example of the response.</span></span>

> <span data-ttu-id="90fcc-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="90fcc-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerDeviceUsageUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 442

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerDeviceUsageUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-06", 
      "userPrincipalName": "userPrincipalName-value", 
      "displayName": "displayName-value", 
      "userState": "active", 
      "stateChangeDate": "2012-06-26", 
      "lastActivityDate": "2017-09-06", 
      "usedWeb": true, 
      "usedWindowsPhone": false, 
      "usedAndroidPhone": false, 
      "usediPhone": false, 
      "usediPad": false, 
      "usedOthers": false, 
      "reportPeriod": "7"
    }
  ]
}
```
