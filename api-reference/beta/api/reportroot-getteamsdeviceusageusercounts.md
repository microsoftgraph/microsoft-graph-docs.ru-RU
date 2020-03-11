---
title: 'reportRoot: getTeamsDeviceUsageUserCounts'
description: Получение сведений о количестве уникальных пользователей Microsoft Teams в день с сортировкой по типам устройств.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: f6a6ec7637bea82b7f14c48a0bd2e9cda9d6b6f4
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2020
ms.locfileid: "42589489"
---
# <a name="reportroot-getteamsdeviceusageusercounts"></a><span data-ttu-id="47957-103">reportRoot: getTeamsDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="47957-103">reportRoot: getTeamsDeviceUsageUserCounts</span></span>

<span data-ttu-id="47957-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47957-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47957-105">Получение сведений о количестве уникальных пользователей Microsoft Teams в день с сортировкой по типам устройств.</span><span class="sxs-lookup"><span data-stu-id="47957-105">Get the number of Microsoft Teams daily unique users by device type.</span></span>

## <a name="permissions"></a><span data-ttu-id="47957-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="47957-106">Permissions</span></span>

<span data-ttu-id="47957-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47957-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="47957-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47957-109">Permission type</span></span>                        | <span data-ttu-id="47957-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="47957-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="47957-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47957-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="47957-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="47957-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="47957-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47957-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47957-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47957-114">Not supported.</span></span>                           |
| <span data-ttu-id="47957-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="47957-115">Application</span></span>                            | <span data-ttu-id="47957-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="47957-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="47957-117">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="47957-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="47957-118">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="47957-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="47957-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47957-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="47957-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="47957-120">Function parameters</span></span>

<span data-ttu-id="47957-121">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="47957-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="47957-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="47957-122">Parameter</span></span> | <span data-ttu-id="47957-123">Тип</span><span class="sxs-lookup"><span data-stu-id="47957-123">Type</span></span>   | <span data-ttu-id="47957-124">Описание</span><span class="sxs-lookup"><span data-stu-id="47957-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="47957-125">period</span><span class="sxs-lookup"><span data-stu-id="47957-125">period</span></span>    | <span data-ttu-id="47957-126">string</span><span class="sxs-lookup"><span data-stu-id="47957-126">string</span></span> | <span data-ttu-id="47957-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="47957-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="47957-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="47957-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="47957-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="47957-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="47957-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="47957-130">Required.</span></span> |

<span data-ttu-id="47957-131">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="47957-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="47957-132">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="47957-132">The default output type is text/csv.</span></span> <span data-ttu-id="47957-133">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="47957-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="47957-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="47957-134">Request headers</span></span>

| <span data-ttu-id="47957-135">Имя</span><span class="sxs-lookup"><span data-stu-id="47957-135">Name</span></span>          | <span data-ttu-id="47957-136">Описание</span><span class="sxs-lookup"><span data-stu-id="47957-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="47957-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="47957-137">Authorization</span></span> | <span data-ttu-id="47957-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="47957-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="47957-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="47957-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="47957-141">CSV</span><span class="sxs-lookup"><span data-stu-id="47957-141">CSV</span></span>

<span data-ttu-id="47957-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="47957-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="47957-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="47957-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="47957-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="47957-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="47957-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="47957-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="47957-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="47957-146">Report Refresh Date</span></span>
- <span data-ttu-id="47957-147">"Web" (Интернет);</span><span class="sxs-lookup"><span data-stu-id="47957-147">Web</span></span>
- <span data-ttu-id="47957-148">"Windows Phone";</span><span class="sxs-lookup"><span data-stu-id="47957-148">Windows Phone</span></span>
- <span data-ttu-id="47957-149">"Android Phone" (Телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="47957-149">Android Phone</span></span>
- <span data-ttu-id="47957-150">"iOS";</span><span class="sxs-lookup"><span data-stu-id="47957-150">iOS</span></span>
- <span data-ttu-id="47957-151">"Mac";</span><span class="sxs-lookup"><span data-stu-id="47957-151">Mac</span></span>
- <span data-ttu-id="47957-152">"Windows";</span><span class="sxs-lookup"><span data-stu-id="47957-152">Windows</span></span>
- <span data-ttu-id="47957-153">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="47957-153">Report Date</span></span>
- <span data-ttu-id="47957-154">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="47957-154">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="47957-155">JSON</span><span class="sxs-lookup"><span data-stu-id="47957-155">JSON</span></span>

<span data-ttu-id="47957-156">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[теамсдевицеусажеусеркаунтс](../resources/teamsdeviceusageusercounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="47957-156">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageUserCounts](../resources/teamsdeviceusageusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47957-157">Пример</span><span class="sxs-lookup"><span data-stu-id="47957-157">Example</span></span>

### <a name="csv"></a><span data-ttu-id="47957-158">CSV</span><span class="sxs-lookup"><span data-stu-id="47957-158">CSV</span></span>

<span data-ttu-id="47957-159">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="47957-159">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="47957-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="47957-160">Request</span></span>

<span data-ttu-id="47957-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47957-161">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsdeviceusageusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="47957-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="47957-162">Response</span></span>

<span data-ttu-id="47957-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="47957-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="47957-164">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="47957-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="47957-165">JSON</span><span class="sxs-lookup"><span data-stu-id="47957-165">JSON</span></span>

<span data-ttu-id="47957-166">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="47957-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="47957-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="47957-167">Request</span></span>

<span data-ttu-id="47957-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47957-168">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsdeviceusageusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="47957-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="47957-169">Response</span></span>

<span data-ttu-id="47957-170">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="47957-170">The following is an example of the response.</span></span>

> <span data-ttu-id="47957-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="47957-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
