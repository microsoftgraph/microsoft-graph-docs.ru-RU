---
title: 'reportRoot: getTeamsDeviceUsageDistributionUserCounts'
description: Получите количество уникальных лицензированных пользователей Microsoft Teams по типу устройства за выбранный период времени.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: c6d6e8cf10071b46d660f5e50e80a45b2a0c1e10
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766191"
---
# <a name="reportroot-getteamsdeviceusagedistributionusercounts"></a><span data-ttu-id="dd96a-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="dd96a-103">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span></span>

<span data-ttu-id="dd96a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd96a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd96a-105">Получите количество уникальных лицензированных пользователей Microsoft Teams по типу устройства за выбранный период времени.</span><span class="sxs-lookup"><span data-stu-id="dd96a-105">Get the number of unique Microsoft Teams licensed users by device type over the selected time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="dd96a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dd96a-106">Permissions</span></span>

<span data-ttu-id="dd96a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd96a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dd96a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd96a-109">Permission type</span></span>                        | <span data-ttu-id="dd96a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dd96a-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="dd96a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd96a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="dd96a-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="dd96a-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="dd96a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd96a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd96a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd96a-114">Not supported.</span></span>                           |
| <span data-ttu-id="dd96a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dd96a-115">Application</span></span>                            | <span data-ttu-id="dd96a-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="dd96a-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="dd96a-117">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="dd96a-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="dd96a-118">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="dd96a-118">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="dd96a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd96a-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="dd96a-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="dd96a-120">Function parameters</span></span>

<span data-ttu-id="dd96a-121">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="dd96a-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="dd96a-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="dd96a-122">Parameter</span></span> | <span data-ttu-id="dd96a-123">Тип</span><span class="sxs-lookup"><span data-stu-id="dd96a-123">Type</span></span>   | <span data-ttu-id="dd96a-124">Описание</span><span class="sxs-lookup"><span data-stu-id="dd96a-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="dd96a-125">period</span><span class="sxs-lookup"><span data-stu-id="dd96a-125">period</span></span>    | <span data-ttu-id="dd96a-126">string</span><span class="sxs-lookup"><span data-stu-id="dd96a-126">string</span></span> | <span data-ttu-id="dd96a-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="dd96a-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="dd96a-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="dd96a-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="dd96a-129">Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="dd96a-129">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="dd96a-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd96a-130">Required.</span></span> |

<span data-ttu-id="dd96a-131">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="dd96a-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="dd96a-132">Тип вывода по умолчанию — текст/csv.</span><span class="sxs-lookup"><span data-stu-id="dd96a-132">The default output type is text/csv.</span></span> <span data-ttu-id="dd96a-133">Однако, если требуется указать тип вывода, можно использовать параметр OData $format для параметра text/csv или application/json.</span><span class="sxs-lookup"><span data-stu-id="dd96a-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dd96a-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dd96a-134">Request headers</span></span>

| <span data-ttu-id="dd96a-135">Имя</span><span class="sxs-lookup"><span data-stu-id="dd96a-135">Name</span></span>          | <span data-ttu-id="dd96a-136">Описание</span><span class="sxs-lookup"><span data-stu-id="dd96a-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="dd96a-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dd96a-137">Authorization</span></span> | <span data-ttu-id="dd96a-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd96a-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="dd96a-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd96a-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="dd96a-141">CSV</span><span class="sxs-lookup"><span data-stu-id="dd96a-141">CSV</span></span>

<span data-ttu-id="dd96a-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="dd96a-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="dd96a-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="dd96a-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="dd96a-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="dd96a-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="dd96a-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="dd96a-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="dd96a-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="dd96a-146">Report Refresh Date</span></span>
- <span data-ttu-id="dd96a-147">"Web" (Интернет);</span><span class="sxs-lookup"><span data-stu-id="dd96a-147">Web</span></span>
- <span data-ttu-id="dd96a-148">"Windows Phone";</span><span class="sxs-lookup"><span data-stu-id="dd96a-148">Windows Phone</span></span>
- <span data-ttu-id="dd96a-149">"Android Phone" (Телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="dd96a-149">Android Phone</span></span>
- <span data-ttu-id="dd96a-150">"iOS";</span><span class="sxs-lookup"><span data-stu-id="dd96a-150">iOS</span></span>
- <span data-ttu-id="dd96a-151">"Mac";</span><span class="sxs-lookup"><span data-stu-id="dd96a-151">Mac</span></span>
- <span data-ttu-id="dd96a-152">"Windows";</span><span class="sxs-lookup"><span data-stu-id="dd96a-152">Windows</span></span>
- <span data-ttu-id="dd96a-153">Chrome OS</span><span class="sxs-lookup"><span data-stu-id="dd96a-153">Chrome OS</span></span>
- <span data-ttu-id="dd96a-154">Linux</span><span class="sxs-lookup"><span data-stu-id="dd96a-154">Linux</span></span>
- <span data-ttu-id="dd96a-155">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="dd96a-155">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="dd96a-156">JSON</span><span class="sxs-lookup"><span data-stu-id="dd96a-156">JSON</span></span>

<span data-ttu-id="dd96a-157">В случае успешной работы этот метод возвращает код ответа и `200 OK` **[объект teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md)** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="dd96a-157">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageDistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd96a-158">Пример</span><span class="sxs-lookup"><span data-stu-id="dd96a-158">Example</span></span>

### <a name="csv"></a><span data-ttu-id="dd96a-159">CSV</span><span class="sxs-lookup"><span data-stu-id="dd96a-159">CSV</span></span>

<span data-ttu-id="dd96a-160">Ниже приводится пример, который выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="dd96a-160">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="dd96a-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd96a-161">Request</span></span>

<span data-ttu-id="dd96a-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dd96a-162">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="dd96a-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd96a-163">Response</span></span>

<span data-ttu-id="dd96a-164">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dd96a-164">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="dd96a-165">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="dd96a-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iOS,Mac,Windows,Chrome OS,Linux,Report Period
```

### <a name="json"></a><span data-ttu-id="dd96a-166">JSON</span><span class="sxs-lookup"><span data-stu-id="dd96a-166">JSON</span></span>

<span data-ttu-id="dd96a-167">Ниже приводится пример, который возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="dd96a-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="dd96a-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd96a-168">Request</span></span>

<span data-ttu-id="dd96a-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dd96a-169">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="dd96a-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd96a-170">Response</span></span>

<span data-ttu-id="dd96a-171">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dd96a-171">The following is an example of the response.</span></span>

> <span data-ttu-id="dd96a-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dd96a-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "chromeOS": 100, 
      "linux": 60, 
      "windows": 491, 
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


