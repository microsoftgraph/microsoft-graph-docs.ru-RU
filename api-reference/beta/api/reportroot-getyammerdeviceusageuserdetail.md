---
title: 'reportRoot: getYammerDeviceUsageUserDetail function'
description: Получение сведений об использовании устройства с Yammer с разбивкой по пользователям.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 5af33e93b542a4a6bafd285f93a639fd0a3a88a0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052986"
---
# <a name="reportroot-getyammerdeviceusageuserdetail-function"></a><span data-ttu-id="35121-103">reportRoot: getYammerDeviceUsageUserDetail function</span><span class="sxs-lookup"><span data-stu-id="35121-103">reportRoot: getYammerDeviceUsageUserDetail function</span></span>

<span data-ttu-id="35121-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35121-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35121-105">Получение сведений об использовании устройств с Yammer с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="35121-105">Get details about Yammer device usage by user.</span></span>

> <span data-ttu-id="35121-106">**Примечание:** Сведения о различных представлениях отчетов и их именах можно найти в [статье Microsoft 365 Reports-Device Device Usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="35121-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="35121-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="35121-107">Permissions</span></span>

<span data-ttu-id="35121-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35121-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="35121-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="35121-110">Permission type</span></span>                        | <span data-ttu-id="35121-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="35121-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="35121-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="35121-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="35121-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="35121-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="35121-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="35121-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35121-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35121-115">Not supported.</span></span>                           |
| <span data-ttu-id="35121-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="35121-116">Application</span></span>                            | <span data-ttu-id="35121-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="35121-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="35121-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="35121-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="35121-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="35121-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="35121-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="35121-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserDetail(period='{period_value}')
GET /reports/getYammerDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="35121-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="35121-121">Function parameters</span></span>

<span data-ttu-id="35121-122">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="35121-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="35121-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="35121-123">Parameter</span></span> | <span data-ttu-id="35121-124">Тип</span><span class="sxs-lookup"><span data-stu-id="35121-124">Type</span></span>   | <span data-ttu-id="35121-125">Описание</span><span class="sxs-lookup"><span data-stu-id="35121-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="35121-126">period</span><span class="sxs-lookup"><span data-stu-id="35121-126">period</span></span>    | <span data-ttu-id="35121-127">string</span><span class="sxs-lookup"><span data-stu-id="35121-127">string</span></span> | <span data-ttu-id="35121-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="35121-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="35121-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="35121-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="35121-130">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="35121-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="35121-131">date</span><span class="sxs-lookup"><span data-stu-id="35121-131">date</span></span>      | <span data-ttu-id="35121-132">Date</span><span class="sxs-lookup"><span data-stu-id="35121-132">Date</span></span>   | <span data-ttu-id="35121-133">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="35121-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="35121-134">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="35121-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="35121-135">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="35121-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="35121-136">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="35121-136">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="35121-137">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="35121-137">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="35121-138">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="35121-138">The default output type is text/csv.</span></span> <span data-ttu-id="35121-139">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="35121-139">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="35121-140">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="35121-140">Request headers</span></span>

| <span data-ttu-id="35121-141">Имя</span><span class="sxs-lookup"><span data-stu-id="35121-141">Name</span></span>          | <span data-ttu-id="35121-142">Описание</span><span class="sxs-lookup"><span data-stu-id="35121-142">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="35121-143">Авторизация</span><span class="sxs-lookup"><span data-stu-id="35121-143">Authorization</span></span> | <span data-ttu-id="35121-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="35121-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="35121-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="35121-146">Response</span></span>

### <a name="csv"></a><span data-ttu-id="35121-147">CSV</span><span class="sxs-lookup"><span data-stu-id="35121-147">CSV</span></span>

<span data-ttu-id="35121-148">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="35121-148">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="35121-149">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="35121-149">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="35121-150">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="35121-150">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="35121-151">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="35121-151">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="35121-152">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="35121-152">Report Refresh Date</span></span>
- <span data-ttu-id="35121-153">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="35121-153">User Principal Name</span></span>
- <span data-ttu-id="35121-154">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="35121-154">Display Name</span></span>
- <span data-ttu-id="35121-155">"User State" (Состояние пользователя);</span><span class="sxs-lookup"><span data-stu-id="35121-155">User State</span></span>
- <span data-ttu-id="35121-156">"State Change Date" (Дата изменения состояния);</span><span class="sxs-lookup"><span data-stu-id="35121-156">State Change Date</span></span>
- <span data-ttu-id="35121-157">"Last Activity Date" (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="35121-157">Last Activity Date</span></span>
- <span data-ttu-id="35121-158">"Used Web" (Используемое веб-приложение);</span><span class="sxs-lookup"><span data-stu-id="35121-158">Used Web</span></span>
- <span data-ttu-id="35121-159">"Used Windows Phone" (Используемое устройство Windows Phone);</span><span class="sxs-lookup"><span data-stu-id="35121-159">Used Windows Phone</span></span>
- <span data-ttu-id="35121-160">"Used Android Phone" (Используемый телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="35121-160">Used Android Phone</span></span>
- <span data-ttu-id="35121-161">"Used iPhone" (Используемый телефон iPhone);</span><span class="sxs-lookup"><span data-stu-id="35121-161">Used iPhone</span></span>
- <span data-ttu-id="35121-162">"Used iPad" (Используемое устройство iPad);</span><span class="sxs-lookup"><span data-stu-id="35121-162">Used iPad</span></span>
- <span data-ttu-id="35121-163">"Used Others" (Другое используемое);</span><span class="sxs-lookup"><span data-stu-id="35121-163">Used Others</span></span>
- <span data-ttu-id="35121-164">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="35121-164">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="35121-165">JSON</span><span class="sxs-lookup"><span data-stu-id="35121-165">JSON</span></span>

<span data-ttu-id="35121-166">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[яммердевицеусажеусердетаил](../resources/yammerdeviceusageuserdetail.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="35121-166">If successful, this method returns a `200 OK` response code and a **[yammerDeviceUsageUserDetail](../resources/yammerdeviceusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="35121-167">Размер страницы по умолчанию для этого запроса составляет 200 элементов.</span><span class="sxs-lookup"><span data-stu-id="35121-167">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="35121-168">Пример</span><span class="sxs-lookup"><span data-stu-id="35121-168">Example</span></span>

### <a name="csv"></a><span data-ttu-id="35121-169">CSV</span><span class="sxs-lookup"><span data-stu-id="35121-169">CSV</span></span>

<span data-ttu-id="35121-170">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="35121-170">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="35121-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="35121-171">Request</span></span>

<span data-ttu-id="35121-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="35121-172">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getyammerdeviceusageuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageUserDetail(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="35121-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="35121-173">Response</span></span>

<span data-ttu-id="35121-174">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="35121-174">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="35121-175">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="35121-175">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="35121-176">JSON</span><span class="sxs-lookup"><span data-stu-id="35121-176">JSON</span></span>

<span data-ttu-id="35121-177">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="35121-177">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="35121-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="35121-178">Request</span></span>

<span data-ttu-id="35121-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="35121-179">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getyammerdeviceusageuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageUserDetail(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="35121-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="35121-180">Response</span></span>

<span data-ttu-id="35121-181">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="35121-181">The following is an example of the response.</span></span>

> <span data-ttu-id="35121-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="35121-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


