---
title: 'reportRoot: getSkypeForBusinessDeviceUsageUserCounts'
description: Отследите динамику использования по количеству пользователей в организации, подключавшихся с помощью приложения Skype для бизнеса. Кроме того, вы получите статистические данные с разбивкой по типу устройства (устройство с Windows, телефон с Windows, телефон с Android, iPhone или iPad), на котором установлено клиентское приложение Skype для бизнеса, используемое в организации.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: aace5af72229b022ee6b03c114388a1c99a59269
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48053274"
---
# <a name="reportroot-getskypeforbusinessdeviceusageusercounts"></a><span data-ttu-id="ac9fc-104">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="ac9fc-104">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span></span>

<span data-ttu-id="ac9fc-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac9fc-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac9fc-106">Отследите динамику использования по количеству пользователей в организации, подключавшихся с помощью приложения Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-106">Get the usage trends on how many users in your organization have connected using the Skype for Business app.</span></span> <span data-ttu-id="ac9fc-107">Кроме того, вы получите статистические данные с разбивкой по типу устройства (устройство с Windows, телефон с Windows, телефон с Android, iPhone или iPad), на котором установлено клиентское приложение Skype для бизнеса, используемое в организации.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-107">You will also get a breakdown by the type of device (Windows, Windows phone, Android phone, iPhone, or iPad) on which the Skype for Business client app is installed and used across your organization.</span></span>

> <span data-ttu-id="ac9fc-108">**Примечание:** Сведения о различных представлениях отчетов и их именах можно найти в [статье Microsoft 365 Reports-клиенты Skype для бизнеса](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span><span class="sxs-lookup"><span data-stu-id="ac9fc-108">**Note:** For details about different report views and names, see [Microsoft 365 reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="ac9fc-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ac9fc-109">Permissions</span></span>

<span data-ttu-id="ac9fc-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac9fc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ac9fc-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ac9fc-112">Permission type</span></span>                        | <span data-ttu-id="ac9fc-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ac9fc-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ac9fc-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ac9fc-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="ac9fc-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ac9fc-115">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ac9fc-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ac9fc-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac9fc-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-117">Not supported.</span></span>                           |
| <span data-ttu-id="ac9fc-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ac9fc-118">Application</span></span>                            | <span data-ttu-id="ac9fc-119">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ac9fc-119">Reports.Read.All</span></span>                         |

<span data-ttu-id="ac9fc-120">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-120">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="ac9fc-121">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="ac9fc-121">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="ac9fc-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ac9fc-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="ac9fc-123">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="ac9fc-123">Function parameters</span></span>

<span data-ttu-id="ac9fc-124">В URL-адресе запроса укажите приведенный ниже параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-124">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="ac9fc-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="ac9fc-125">Parameter</span></span> | <span data-ttu-id="ac9fc-126">Тип</span><span class="sxs-lookup"><span data-stu-id="ac9fc-126">Type</span></span>   | <span data-ttu-id="ac9fc-127">Описание</span><span class="sxs-lookup"><span data-stu-id="ac9fc-127">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="ac9fc-128">period</span><span class="sxs-lookup"><span data-stu-id="ac9fc-128">period</span></span>    | <span data-ttu-id="ac9fc-129">string</span><span class="sxs-lookup"><span data-stu-id="ac9fc-129">string</span></span> | <span data-ttu-id="ac9fc-130">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-130">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="ac9fc-131">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-131">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="ac9fc-132">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-132">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="ac9fc-133">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-133">Required.</span></span> |

<span data-ttu-id="ac9fc-134">Этот метод поддерживает [параметр запросов OData](/graph/query-parameters) `$format` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-134">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="ac9fc-135">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-135">The default output type is text/csv.</span></span> <span data-ttu-id="ac9fc-136">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ac9fc-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ac9fc-137">Request headers</span></span>

| <span data-ttu-id="ac9fc-138">Имя</span><span class="sxs-lookup"><span data-stu-id="ac9fc-138">Name</span></span>          | <span data-ttu-id="ac9fc-139">Описание</span><span class="sxs-lookup"><span data-stu-id="ac9fc-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="ac9fc-140">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ac9fc-140">Authorization</span></span> | <span data-ttu-id="ac9fc-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="ac9fc-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac9fc-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="ac9fc-144">CSV</span><span class="sxs-lookup"><span data-stu-id="ac9fc-144">CSV</span></span>

<span data-ttu-id="ac9fc-145">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ac9fc-146">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ac9fc-147">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ac9fc-148">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="ac9fc-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="ac9fc-149">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="ac9fc-149">Report Refresh Date</span></span>
- <span data-ttu-id="ac9fc-150">"Windows";</span><span class="sxs-lookup"><span data-stu-id="ac9fc-150">Windows</span></span>
- <span data-ttu-id="ac9fc-151">"Windows Phone";</span><span class="sxs-lookup"><span data-stu-id="ac9fc-151">Windows Phone</span></span>
- <span data-ttu-id="ac9fc-152">"Android Phone" (Телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="ac9fc-152">Android Phone</span></span>
- <span data-ttu-id="ac9fc-153">iPhone</span><span class="sxs-lookup"><span data-stu-id="ac9fc-153">iPhone</span></span>
- <span data-ttu-id="ac9fc-154">iPad</span><span class="sxs-lookup"><span data-stu-id="ac9fc-154">iPad</span></span>
- <span data-ttu-id="ac9fc-155">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="ac9fc-155">Report Date</span></span>
- <span data-ttu-id="ac9fc-156">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="ac9fc-156">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="ac9fc-157">JSON</span><span class="sxs-lookup"><span data-stu-id="ac9fc-157">JSON</span></span>

<span data-ttu-id="ac9fc-158">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[скипефорбусинессдевицеусажеусеркаунтс](../resources/skypeforbusinessdeviceusageusercounts.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-158">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessDeviceUsageUserCounts](../resources/skypeforbusinessdeviceusageusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac9fc-159">Пример</span><span class="sxs-lookup"><span data-stu-id="ac9fc-159">Example</span></span>

### <a name="csv"></a><span data-ttu-id="ac9fc-160">CSV</span><span class="sxs-lookup"><span data-stu-id="ac9fc-160">CSV</span></span>

<span data-ttu-id="ac9fc-161">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-161">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="ac9fc-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="ac9fc-162">Request</span></span>

<span data-ttu-id="ac9fc-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-163">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getskypeforbusinessdeviceusageusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageUserCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="ac9fc-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac9fc-164">Response</span></span>

<span data-ttu-id="ac9fc-165">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-165">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="ac9fc-166">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Windows,Windows Phone,Android Phone,iPhone,iPad,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="ac9fc-167">JSON</span><span class="sxs-lookup"><span data-stu-id="ac9fc-167">JSON</span></span>

<span data-ttu-id="ac9fc-168">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-168">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="ac9fc-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="ac9fc-169">Request</span></span>

<span data-ttu-id="ac9fc-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-170">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getskypeforbusinessdeviceusageusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageUserCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="ac9fc-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac9fc-171">Response</span></span>

<span data-ttu-id="ac9fc-172">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-172">The following is an example of the response.</span></span>

> <span data-ttu-id="ac9fc-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ac9fc-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 289

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessDeviceUsageUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "windows": 403, 
      "windowsPhone": 2, 
      "androidPhone": 13, 
      "iPhone": 26, 
      "iPad": 0, 
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


