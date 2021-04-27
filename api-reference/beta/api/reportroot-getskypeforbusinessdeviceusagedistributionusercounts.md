---
title: 'reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts'
description: Узнайте, сколько сотрудников организации используют уникальные устройства. В отчете будет показано количество пользователей устройств с Windows, телефонов с Windows, телефонов с Android, iPhone и iPad.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 4a842a378aabf55171b3ca69b0a114793ced4577
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052833"
---
# <a name="reportroot-getskypeforbusinessdeviceusagedistributionusercounts"></a><span data-ttu-id="cf522-104">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="cf522-104">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span></span>

<span data-ttu-id="cf522-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf522-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf522-106">Узнайте, сколько сотрудников организации используют уникальные устройства.</span><span class="sxs-lookup"><span data-stu-id="cf522-106">Get the number of users using unique devices in your organization.</span></span> <span data-ttu-id="cf522-107">В отчете будет показано количество пользователей устройств с Windows, телефонов с Windows, телефонов с Android, iPhone и iPad.</span><span class="sxs-lookup"><span data-stu-id="cf522-107">The report will show you the number of users per device including Windows, Windows phone, Android phone, iPhone, and iPad.</span></span>

> <span data-ttu-id="cf522-108">**Примечание:** Подробные сведения о различных представлениях отчетов и [именах см. в Microsoft 365 отчетов — Skype для бизнеса используемых клиентов.](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3)</span><span class="sxs-lookup"><span data-stu-id="cf522-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="cf522-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cf522-109">Permissions</span></span>

<span data-ttu-id="cf522-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf522-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cf522-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cf522-112">Permission type</span></span>                        | <span data-ttu-id="cf522-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cf522-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="cf522-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cf522-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="cf522-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf522-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="cf522-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cf522-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf522-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf522-117">Not supported.</span></span>                           |
| <span data-ttu-id="cf522-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cf522-118">Application</span></span>                            | <span data-ttu-id="cf522-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf522-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="cf522-120">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="cf522-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="cf522-121">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="cf522-121">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="cf522-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cf522-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="cf522-123">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="cf522-123">Function parameters</span></span>

<span data-ttu-id="cf522-124">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="cf522-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="cf522-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="cf522-125">Parameter</span></span> | <span data-ttu-id="cf522-126">Тип</span><span class="sxs-lookup"><span data-stu-id="cf522-126">Type</span></span>   | <span data-ttu-id="cf522-127">Описание</span><span class="sxs-lookup"><span data-stu-id="cf522-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="cf522-128">period</span><span class="sxs-lookup"><span data-stu-id="cf522-128">period</span></span>    | <span data-ttu-id="cf522-129">string</span><span class="sxs-lookup"><span data-stu-id="cf522-129">string</span></span> | <span data-ttu-id="cf522-130">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="cf522-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="cf522-131">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="cf522-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="cf522-132">Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="cf522-132">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="cf522-133">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cf522-133">Required.</span></span> |

<span data-ttu-id="cf522-134">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="cf522-134">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="cf522-135">Тип вывода по умолчанию — текст/csv.</span><span class="sxs-lookup"><span data-stu-id="cf522-135">The default output type is text/csv.</span></span> <span data-ttu-id="cf522-136">Однако, если требуется указать тип вывода, можно использовать параметр OData $format для параметра text/csv или application/json.</span><span class="sxs-lookup"><span data-stu-id="cf522-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cf522-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cf522-137">Request headers</span></span>

| <span data-ttu-id="cf522-138">Имя</span><span class="sxs-lookup"><span data-stu-id="cf522-138">Name</span></span>          | <span data-ttu-id="cf522-139">Описание</span><span class="sxs-lookup"><span data-stu-id="cf522-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="cf522-140">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cf522-140">Authorization</span></span> | <span data-ttu-id="cf522-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cf522-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="cf522-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf522-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="cf522-144">CSV</span><span class="sxs-lookup"><span data-stu-id="cf522-144">CSV</span></span>

<span data-ttu-id="cf522-145">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="cf522-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="cf522-146">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="cf522-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="cf522-147">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="cf522-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="cf522-148">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="cf522-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="cf522-149">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="cf522-149">Report Refresh Date</span></span>
- <span data-ttu-id="cf522-150">"Windows";</span><span class="sxs-lookup"><span data-stu-id="cf522-150">Windows</span></span>
- <span data-ttu-id="cf522-151">"Windows Phone";</span><span class="sxs-lookup"><span data-stu-id="cf522-151">Windows Phone</span></span>
- <span data-ttu-id="cf522-152">"Android Phone" (Телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="cf522-152">Android Phone</span></span>
- <span data-ttu-id="cf522-153">iPhone</span><span class="sxs-lookup"><span data-stu-id="cf522-153">iPhone</span></span>
- <span data-ttu-id="cf522-154">iPad</span><span class="sxs-lookup"><span data-stu-id="cf522-154">iPad</span></span>
- <span data-ttu-id="cf522-155">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="cf522-155">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="cf522-156">JSON</span><span class="sxs-lookup"><span data-stu-id="cf522-156">JSON</span></span>

<span data-ttu-id="cf522-157">В случае успеха этот метод возвращает код отклика и `200 OK` **[объект SkypeForBusinessDeviceUsageDistributionUserCounts](../resources/skypeforbusinessdeviceusagedistributionusercounts.md)** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="cf522-157">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessDeviceUsageDistributionUserCounts](../resources/skypeforbusinessdeviceusagedistributionusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf522-158">Пример</span><span class="sxs-lookup"><span data-stu-id="cf522-158">Example</span></span>

### <a name="csv"></a><span data-ttu-id="cf522-159">CSV</span><span class="sxs-lookup"><span data-stu-id="cf522-159">CSV</span></span>

<span data-ttu-id="cf522-160">Ниже приводится пример, который выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="cf522-160">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="cf522-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="cf522-161">Request</span></span>

<span data-ttu-id="cf522-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cf522-162">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getskypeforbusinessdeviceusagedistributionusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="cf522-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf522-163">Response</span></span>

<span data-ttu-id="cf522-164">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cf522-164">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="cf522-165">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="cf522-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="cf522-166">JSON</span><span class="sxs-lookup"><span data-stu-id="cf522-166">JSON</span></span>

<span data-ttu-id="cf522-167">Ниже приводится пример, который возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="cf522-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="cf522-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="cf522-168">Request</span></span>

<span data-ttu-id="cf522-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cf522-169">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getskypeforbusinessdeviceusagedistributionusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="cf522-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf522-170">Response</span></span>

<span data-ttu-id="cf522-171">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="cf522-171">The following is an example of the response.</span></span>

> <span data-ttu-id="cf522-172">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="cf522-172">**Note:** The response object shown here might be shortened for readability.</span></span>

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


