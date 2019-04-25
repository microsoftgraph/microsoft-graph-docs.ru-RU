---
title: 'reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts'
description: Узнайте, сколько сотрудников организации используют уникальные устройства. В отчете будет показано количество пользователей устройств с Windows, телефонов с Windows, телефонов с Android, iPhone и iPad.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: c31dd67e40d1fc4933847db874cfdf81f72479bf
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537906"
---
# <a name="reportroot-getskypeforbusinessdeviceusagedistributionusercounts"></a><span data-ttu-id="2969b-104">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="2969b-104">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2969b-105">Узнайте, сколько сотрудников организации используют уникальные устройства.</span><span class="sxs-lookup"><span data-stu-id="2969b-105">Get the number of users using unique devices in your organization.</span></span> <span data-ttu-id="2969b-106">В отчете будет показано количество пользователей Windows, телефонов с Windows, телефонов с Android, iPhone и iPad.</span><span class="sxs-lookup"><span data-stu-id="2969b-106">The report will show you the number of users per device including Windows, Windows phone, Android phone, iPhone, and iPad.</span></span>

> <span data-ttu-id="2969b-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span><span class="sxs-lookup"><span data-stu-id="2969b-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="2969b-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2969b-108">Permissions</span></span>

<span data-ttu-id="2969b-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2969b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2969b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2969b-111">Permission type</span></span>                        | <span data-ttu-id="2969b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2969b-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="2969b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2969b-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="2969b-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2969b-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="2969b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2969b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2969b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2969b-116">Not supported.</span></span>                           |
| <span data-ttu-id="2969b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2969b-117">Application</span></span>                            | <span data-ttu-id="2969b-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2969b-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="2969b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2969b-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="2969b-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="2969b-120">Function parameters</span></span>

<span data-ttu-id="2969b-121">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="2969b-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="2969b-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="2969b-122">Parameter</span></span> | <span data-ttu-id="2969b-123">Тип</span><span class="sxs-lookup"><span data-stu-id="2969b-123">Type</span></span>   | <span data-ttu-id="2969b-124">Описание</span><span class="sxs-lookup"><span data-stu-id="2969b-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="2969b-125">period</span><span class="sxs-lookup"><span data-stu-id="2969b-125">period</span></span>    | <span data-ttu-id="2969b-126">string</span><span class="sxs-lookup"><span data-stu-id="2969b-126">string</span></span> | <span data-ttu-id="2969b-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="2969b-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="2969b-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="2969b-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="2969b-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="2969b-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="2969b-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2969b-130">Required.</span></span> |

<span data-ttu-id="2969b-131">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="2969b-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="2969b-132">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="2969b-132">The default output type is text/csv.</span></span> <span data-ttu-id="2969b-133">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="2969b-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2969b-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2969b-134">Request headers</span></span>

| <span data-ttu-id="2969b-135">Имя</span><span class="sxs-lookup"><span data-stu-id="2969b-135">Name</span></span>          | <span data-ttu-id="2969b-136">Описание</span><span class="sxs-lookup"><span data-stu-id="2969b-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="2969b-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2969b-137">Authorization</span></span> | <span data-ttu-id="2969b-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2969b-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="2969b-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="2969b-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="2969b-141">CSV</span><span class="sxs-lookup"><span data-stu-id="2969b-141">CSV</span></span>

<span data-ttu-id="2969b-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="2969b-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="2969b-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="2969b-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="2969b-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="2969b-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="2969b-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="2969b-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="2969b-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="2969b-146">Report Refresh Date</span></span>
- <span data-ttu-id="2969b-147">"Windows";</span><span class="sxs-lookup"><span data-stu-id="2969b-147">Windows</span></span>
- <span data-ttu-id="2969b-148">"Windows Phone";</span><span class="sxs-lookup"><span data-stu-id="2969b-148">Windows Phone</span></span>
- <span data-ttu-id="2969b-149">"Android Phone" (Телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="2969b-149">Android Phone</span></span>
- <span data-ttu-id="2969b-150">iPhone</span><span class="sxs-lookup"><span data-stu-id="2969b-150">iPhone</span></span>
- <span data-ttu-id="2969b-151">iPad</span><span class="sxs-lookup"><span data-stu-id="2969b-151">iPad</span></span>
- <span data-ttu-id="2969b-152">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="2969b-152">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="2969b-153">JSON</span><span class="sxs-lookup"><span data-stu-id="2969b-153">JSON</span></span>

<span data-ttu-id="2969b-154">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[скипефорбусинессдевицеусажедистрибутионусеркаунтс](../resources/skypeforbusinessdeviceusagedistributionusercounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2969b-154">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessDeviceUsageDistributionUserCounts](../resources/skypeforbusinessdeviceusagedistributionusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2969b-155">Пример</span><span class="sxs-lookup"><span data-stu-id="2969b-155">Example</span></span>

### <a name="csv"></a><span data-ttu-id="2969b-156">CSV</span><span class="sxs-lookup"><span data-stu-id="2969b-156">CSV</span></span>

<span data-ttu-id="2969b-157">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="2969b-157">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="2969b-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="2969b-158">Request</span></span>

<span data-ttu-id="2969b-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2969b-159">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusagedistributionusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="2969b-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="2969b-160">Response</span></span>

<span data-ttu-id="2969b-161">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2969b-161">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="2969b-162">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="2969b-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Windows,Windows Phone,Android Phone,iPhone,iPad,Report Period
```

### <a name="json"></a><span data-ttu-id="2969b-163">JSON</span><span class="sxs-lookup"><span data-stu-id="2969b-163">JSON</span></span>

<span data-ttu-id="2969b-164">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="2969b-164">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="2969b-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="2969b-165">Request</span></span>

<span data-ttu-id="2969b-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2969b-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusagedistributionusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="2969b-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="2969b-167">Response</span></span>

<span data-ttu-id="2969b-168">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2969b-168">The following is an example of the response.</span></span>

> <span data-ttu-id="2969b-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2969b-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageDistributionUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 275

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessDeviceUsageDistributionUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "windows": 122, 
      "windowsPhone": 8, 
      "androidPhone": 19, 
      "iPhone": 28, 
      "iPad": 1, 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
