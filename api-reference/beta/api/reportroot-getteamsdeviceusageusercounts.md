---
title: 'reportRoot: getTeamsDeviceUsageUserCounts'
description: Получение сведений о количестве уникальных пользователей Microsoft Teams в день с сортировкой по типам устройств.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 26198ffb967edda0c30823c58241828c95213e5c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957769"
---
# <a name="reportroot-getteamsdeviceusageusercounts"></a><span data-ttu-id="aa05c-103">reportRoot: getTeamsDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="aa05c-103">reportRoot: getTeamsDeviceUsageUserCounts</span></span>

> <span data-ttu-id="aa05c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="aa05c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aa05c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa05c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="aa05c-106">Получение сведений о количестве уникальных пользователей Microsoft Teams в день с сортировкой по типам устройств.</span><span class="sxs-lookup"><span data-stu-id="aa05c-106">Get the number of Microsoft Teams daily unique users by device type.</span></span>

## <a name="permissions"></a><span data-ttu-id="aa05c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aa05c-107">Permissions</span></span>

<span data-ttu-id="aa05c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa05c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="aa05c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aa05c-110">Permission type</span></span>                        | <span data-ttu-id="aa05c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aa05c-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="aa05c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aa05c-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="aa05c-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="aa05c-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="aa05c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aa05c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa05c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa05c-115">Not supported.</span></span>                           |
| <span data-ttu-id="aa05c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aa05c-116">Application</span></span>                            | <span data-ttu-id="aa05c-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="aa05c-117">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="aa05c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aa05c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="aa05c-119">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="aa05c-119">Function parameters</span></span>

<span data-ttu-id="aa05c-120">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="aa05c-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="aa05c-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="aa05c-121">Parameter</span></span> | <span data-ttu-id="aa05c-122">Тип</span><span class="sxs-lookup"><span data-stu-id="aa05c-122">Type</span></span>   | <span data-ttu-id="aa05c-123">Описание</span><span class="sxs-lookup"><span data-stu-id="aa05c-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="aa05c-124">period</span><span class="sxs-lookup"><span data-stu-id="aa05c-124">period</span></span>    | <span data-ttu-id="aa05c-125">строка</span><span class="sxs-lookup"><span data-stu-id="aa05c-125">string</span></span> | <span data-ttu-id="aa05c-126">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="aa05c-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="aa05c-127">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="aa05c-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="aa05c-128">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="aa05c-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="aa05c-129">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aa05c-129">Required.</span></span> |

<span data-ttu-id="aa05c-130">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="aa05c-130">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="aa05c-131">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="aa05c-131">The default output type is text/csv.</span></span> <span data-ttu-id="aa05c-132">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="aa05c-132">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aa05c-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aa05c-133">Request headers</span></span>

| <span data-ttu-id="aa05c-134">Имя</span><span class="sxs-lookup"><span data-stu-id="aa05c-134">Name</span></span>          | <span data-ttu-id="aa05c-135">Описание</span><span class="sxs-lookup"><span data-stu-id="aa05c-135">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="aa05c-136">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aa05c-136">Authorization</span></span> | <span data-ttu-id="aa05c-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aa05c-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="aa05c-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="aa05c-139">Response</span></span>

### <a name="csv"></a><span data-ttu-id="aa05c-140">CSV</span><span class="sxs-lookup"><span data-stu-id="aa05c-140">CSV</span></span>

<span data-ttu-id="aa05c-141">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="aa05c-141">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="aa05c-142">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="aa05c-142">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="aa05c-143">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="aa05c-143">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="aa05c-144">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="aa05c-144">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="aa05c-145">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="aa05c-145">Report Refresh Date</span></span>
- <span data-ttu-id="aa05c-146">"Web" (Интернет);</span><span class="sxs-lookup"><span data-stu-id="aa05c-146">Web</span></span>
- <span data-ttu-id="aa05c-147">"Windows Phone";</span><span class="sxs-lookup"><span data-stu-id="aa05c-147">Windows Phone</span></span>
- <span data-ttu-id="aa05c-148">"Android Phone" (Телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="aa05c-148">Android Phone</span></span>
- <span data-ttu-id="aa05c-149">"iOS";</span><span class="sxs-lookup"><span data-stu-id="aa05c-149">iOS</span></span>
- <span data-ttu-id="aa05c-150">"Mac";</span><span class="sxs-lookup"><span data-stu-id="aa05c-150">Mac</span></span>
- <span data-ttu-id="aa05c-151">"Windows";</span><span class="sxs-lookup"><span data-stu-id="aa05c-151">Windows</span></span>
- <span data-ttu-id="aa05c-152">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="aa05c-152">Report Date</span></span>
- <span data-ttu-id="aa05c-153">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="aa05c-153">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="aa05c-154">JSON</span><span class="sxs-lookup"><span data-stu-id="aa05c-154">JSON</span></span>

<span data-ttu-id="aa05c-155">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[teamsDeviceUsageUserCounts](../resources/teamsdeviceusageusercounts.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="aa05c-155">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageUserCounts](../resources/teamsdeviceusageusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa05c-156">Пример</span><span class="sxs-lookup"><span data-stu-id="aa05c-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="aa05c-157">CSV</span><span class="sxs-lookup"><span data-stu-id="aa05c-157">CSV</span></span>

<span data-ttu-id="aa05c-158">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="aa05c-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="aa05c-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="aa05c-159">Request</span></span>

<span data-ttu-id="aa05c-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aa05c-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="aa05c-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="aa05c-161">Response</span></span>

<span data-ttu-id="aa05c-162">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="aa05c-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="aa05c-163">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="aa05c-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iOS,Mac,Windows,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="aa05c-164">JSON</span><span class="sxs-lookup"><span data-stu-id="aa05c-164">JSON</span></span>

<span data-ttu-id="aa05c-165">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="aa05c-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="aa05c-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="aa05c-166">Request</span></span>

<span data-ttu-id="aa05c-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aa05c-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="aa05c-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="aa05c-168">Response</span></span>

<span data-ttu-id="aa05c-169">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="aa05c-169">The following is an example of the response.</span></span>

> <span data-ttu-id="aa05c-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aa05c-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 269

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsDeviceUsageUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "web": 13, 
      "windowsPhone": 0, 
      "androidPhone": 22, 
      "ios": 75, 
      "mac": 16, 
      "windows": 257, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
