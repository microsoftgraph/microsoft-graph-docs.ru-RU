---
title: 'reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts'
description: Узнайте, сколько сотрудников организации используют уникальные устройства. В отчете будет показано количество пользователей Windows, телефонов с Windows, телефонов с Android, iPhone и iPad.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: ccae9dd215c74fee6ebc2703d848bc563ff1b0c8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948046"
---
# <a name="reportroot-getskypeforbusinessdeviceusagedistributionusercounts"></a><span data-ttu-id="64dfe-104">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="64dfe-104">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span></span>

> <span data-ttu-id="64dfe-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="64dfe-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="64dfe-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64dfe-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="64dfe-107">Узнайте, сколько сотрудников организации используют уникальные устройства.</span><span class="sxs-lookup"><span data-stu-id="64dfe-107">Get the number of users using unique devices in your organization.</span></span> <span data-ttu-id="64dfe-108">В отчете будет показано количество пользователей Windows, телефонов с Windows, телефонов с Android, iPhone и iPad.</span><span class="sxs-lookup"><span data-stu-id="64dfe-108">The report will show you the number of users per device including Windows, Windows phone, Android phone, iPhone, and iPad.</span></span>

> <span data-ttu-id="64dfe-109">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span><span class="sxs-lookup"><span data-stu-id="64dfe-109">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="64dfe-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="64dfe-110">Permissions</span></span>

<span data-ttu-id="64dfe-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64dfe-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="64dfe-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64dfe-113">Permission type</span></span>                        | <span data-ttu-id="64dfe-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="64dfe-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="64dfe-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64dfe-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="64dfe-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="64dfe-116">Reports.Read.All</span></span>                         |
| <span data-ttu-id="64dfe-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64dfe-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64dfe-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64dfe-118">Not supported.</span></span>                           |
| <span data-ttu-id="64dfe-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="64dfe-119">Application</span></span>                            | <span data-ttu-id="64dfe-120">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="64dfe-120">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="64dfe-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64dfe-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="64dfe-122">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="64dfe-122">Function parameters</span></span>

<span data-ttu-id="64dfe-123">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="64dfe-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="64dfe-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="64dfe-124">Parameter</span></span> | <span data-ttu-id="64dfe-125">Тип</span><span class="sxs-lookup"><span data-stu-id="64dfe-125">Type</span></span>   | <span data-ttu-id="64dfe-126">Описание</span><span class="sxs-lookup"><span data-stu-id="64dfe-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="64dfe-127">period</span><span class="sxs-lookup"><span data-stu-id="64dfe-127">period</span></span>    | <span data-ttu-id="64dfe-128">строка</span><span class="sxs-lookup"><span data-stu-id="64dfe-128">string</span></span> | <span data-ttu-id="64dfe-129">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="64dfe-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="64dfe-130">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="64dfe-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="64dfe-131">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="64dfe-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="64dfe-132">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64dfe-132">Required.</span></span> |

<span data-ttu-id="64dfe-133">Этот метод поддерживает `$format` [параметр запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="64dfe-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="64dfe-134">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="64dfe-134">The default output type is text/csv.</span></span> <span data-ttu-id="64dfe-135">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="64dfe-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="64dfe-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="64dfe-136">Request headers</span></span>

| <span data-ttu-id="64dfe-137">Имя</span><span class="sxs-lookup"><span data-stu-id="64dfe-137">Name</span></span>          | <span data-ttu-id="64dfe-138">Описание</span><span class="sxs-lookup"><span data-stu-id="64dfe-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="64dfe-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="64dfe-139">Authorization</span></span> | <span data-ttu-id="64dfe-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64dfe-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="64dfe-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="64dfe-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="64dfe-143">CSV</span><span class="sxs-lookup"><span data-stu-id="64dfe-143">CSV</span></span>

<span data-ttu-id="64dfe-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="64dfe-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="64dfe-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="64dfe-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="64dfe-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="64dfe-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="64dfe-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="64dfe-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="64dfe-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="64dfe-148">Report Refresh Date</span></span>
- <span data-ttu-id="64dfe-149">Windows</span><span class="sxs-lookup"><span data-stu-id="64dfe-149">Windows</span></span>
- <span data-ttu-id="64dfe-150">"Windows Phone";</span><span class="sxs-lookup"><span data-stu-id="64dfe-150">Windows Phone</span></span>
- <span data-ttu-id="64dfe-151">"Android Phone" (Телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="64dfe-151">Android Phone</span></span>
- <span data-ttu-id="64dfe-152">"iPhone";</span><span class="sxs-lookup"><span data-stu-id="64dfe-152">iPhone</span></span>
- <span data-ttu-id="64dfe-153">iPad</span><span class="sxs-lookup"><span data-stu-id="64dfe-153">iPad</span></span>
- <span data-ttu-id="64dfe-154">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="64dfe-154">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="64dfe-155">JSON</span><span class="sxs-lookup"><span data-stu-id="64dfe-155">JSON</span></span>

<span data-ttu-id="64dfe-156">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[skypeForBusinessDeviceUsageDistributionUserCounts](../resources/skypeforbusinessdeviceusagedistributionusercounts.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="64dfe-156">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessDeviceUsageDistributionUserCounts](../resources/skypeforbusinessdeviceusagedistributionusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64dfe-157">Пример</span><span class="sxs-lookup"><span data-stu-id="64dfe-157">Example</span></span>

### <a name="csv"></a><span data-ttu-id="64dfe-158">CSV</span><span class="sxs-lookup"><span data-stu-id="64dfe-158">CSV</span></span>

<span data-ttu-id="64dfe-159">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="64dfe-159">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="64dfe-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="64dfe-160">Request</span></span>

<span data-ttu-id="64dfe-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="64dfe-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusagedistributionusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="64dfe-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="64dfe-162">Response</span></span>

<span data-ttu-id="64dfe-163">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="64dfe-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="64dfe-164">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="64dfe-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="64dfe-165">JSON</span><span class="sxs-lookup"><span data-stu-id="64dfe-165">JSON</span></span>

<span data-ttu-id="64dfe-166">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="64dfe-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="64dfe-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="64dfe-167">Request</span></span>

<span data-ttu-id="64dfe-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="64dfe-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusagedistributionusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="64dfe-169">Ответ</span><span class="sxs-lookup"><span data-stu-id="64dfe-169">Response</span></span>

<span data-ttu-id="64dfe-170">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="64dfe-170">The following is an example of the response.</span></span>

> <span data-ttu-id="64dfe-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="64dfe-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
