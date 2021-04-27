---
title: 'reportRoot: getSkypeForBusinessDeviceUsageUserDetail'
description: Получите сведения об использовании устройств со Skype для бизнеса с разбивкой по пользователям.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: fe7fdfa1a1d041522ea88037b3e0ca954be4646f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052819"
---
# <a name="reportroot-getskypeforbusinessdeviceusageuserdetail"></a><span data-ttu-id="009a6-103">reportRoot: getSkypeForBusinessDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="009a6-103">reportRoot: getSkypeForBusinessDeviceUsageUserDetail</span></span>

<span data-ttu-id="009a6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="009a6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="009a6-105">Получите сведения об использовании устройств со Skype для бизнеса с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="009a6-105">Get details about Skype for Business device usage by user.</span></span>

> <span data-ttu-id="009a6-106">**Примечание:** Подробные сведения о различных представлениях отчетов и [именах см. в Microsoft 365 отчетов — Skype для бизнеса используемых клиентов.](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3)</span><span class="sxs-lookup"><span data-stu-id="009a6-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="009a6-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="009a6-107">Permissions</span></span>

<span data-ttu-id="009a6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="009a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="009a6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="009a6-110">Permission type</span></span>                        | <span data-ttu-id="009a6-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="009a6-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="009a6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="009a6-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="009a6-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="009a6-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="009a6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="009a6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="009a6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="009a6-115">Not supported.</span></span>                           |
| <span data-ttu-id="009a6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="009a6-116">Application</span></span>                            | <span data-ttu-id="009a6-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="009a6-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="009a6-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="009a6-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="009a6-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="009a6-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="009a6-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="009a6-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="009a6-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="009a6-121">Function parameters</span></span>

<span data-ttu-id="009a6-122">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="009a6-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="009a6-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="009a6-123">Parameter</span></span> | <span data-ttu-id="009a6-124">Тип</span><span class="sxs-lookup"><span data-stu-id="009a6-124">Type</span></span>   | <span data-ttu-id="009a6-125">Описание</span><span class="sxs-lookup"><span data-stu-id="009a6-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="009a6-126">period</span><span class="sxs-lookup"><span data-stu-id="009a6-126">period</span></span>    | <span data-ttu-id="009a6-127">string</span><span class="sxs-lookup"><span data-stu-id="009a6-127">string</span></span> | <span data-ttu-id="009a6-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="009a6-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="009a6-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="009a6-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="009a6-130">Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="009a6-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="009a6-131">date</span><span class="sxs-lookup"><span data-stu-id="009a6-131">date</span></span>      | <span data-ttu-id="009a6-132">Date</span><span class="sxs-lookup"><span data-stu-id="009a6-132">Date</span></span>   | <span data-ttu-id="009a6-133">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="009a6-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="009a6-134">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="009a6-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="009a6-135">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="009a6-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="009a6-136">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="009a6-136">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="009a6-137">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="009a6-137">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="009a6-138">Тип вывода по умолчанию — текст/csv.</span><span class="sxs-lookup"><span data-stu-id="009a6-138">The default output type is text/csv.</span></span> <span data-ttu-id="009a6-139">Однако, если требуется указать тип вывода, можно использовать параметр OData $format для параметра text/csv или application/json.</span><span class="sxs-lookup"><span data-stu-id="009a6-139">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="009a6-140">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="009a6-140">Request headers</span></span>

| <span data-ttu-id="009a6-141">Имя</span><span class="sxs-lookup"><span data-stu-id="009a6-141">Name</span></span>          | <span data-ttu-id="009a6-142">Описание</span><span class="sxs-lookup"><span data-stu-id="009a6-142">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="009a6-143">Авторизация</span><span class="sxs-lookup"><span data-stu-id="009a6-143">Authorization</span></span> | <span data-ttu-id="009a6-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="009a6-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="009a6-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="009a6-146">Response</span></span>

### <a name="csv"></a><span data-ttu-id="009a6-147">CSV</span><span class="sxs-lookup"><span data-stu-id="009a6-147">CSV</span></span>

<span data-ttu-id="009a6-148">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="009a6-148">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="009a6-149">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="009a6-149">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="009a6-150">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="009a6-150">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="009a6-151">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="009a6-151">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="009a6-152">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="009a6-152">Report Refresh Date</span></span>
- <span data-ttu-id="009a6-153">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="009a6-153">User Principal Name</span></span>
- <span data-ttu-id="009a6-154">Last Activity Date (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="009a6-154">Last Activity Date</span></span>
- <span data-ttu-id="009a6-155">"Used Windows" (Используемая ОС Windows);</span><span class="sxs-lookup"><span data-stu-id="009a6-155">Used Windows</span></span>
- <span data-ttu-id="009a6-156">"Used Windows Phone" (Используемое устройство Windows Phone);</span><span class="sxs-lookup"><span data-stu-id="009a6-156">Used Windows Phone</span></span>
- <span data-ttu-id="009a6-157">"Used Android Phone" (Используемый телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="009a6-157">Used Android Phone</span></span>
- <span data-ttu-id="009a6-158">"Used iPhone" (Используемый телефон iPhone);</span><span class="sxs-lookup"><span data-stu-id="009a6-158">Used iPhone</span></span>
- <span data-ttu-id="009a6-159">"Used iPad" (Используемое устройство iPad);</span><span class="sxs-lookup"><span data-stu-id="009a6-159">Used iPad</span></span>
- <span data-ttu-id="009a6-160">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="009a6-160">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="009a6-161">JSON</span><span class="sxs-lookup"><span data-stu-id="009a6-161">JSON</span></span>

<span data-ttu-id="009a6-162">В случае успешной работы этот метод возвращает код отклика и `200 OK` **[объект SkypeForBusinessDeviceUsageUserDetail](../resources/skypeforbusinessdeviceusageuserdetail.md)** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="009a6-162">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessDeviceUsageUserDetail](../resources/skypeforbusinessdeviceusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="009a6-163">Размер страницы по умолчанию для этого запроса составляет 200 элементов.</span><span class="sxs-lookup"><span data-stu-id="009a6-163">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="009a6-164">Пример</span><span class="sxs-lookup"><span data-stu-id="009a6-164">Example</span></span>

### <a name="csv"></a><span data-ttu-id="009a6-165">CSV</span><span class="sxs-lookup"><span data-stu-id="009a6-165">CSV</span></span>

<span data-ttu-id="009a6-166">Ниже приводится пример, который выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="009a6-166">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="009a6-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="009a6-167">Request</span></span>

<span data-ttu-id="009a6-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="009a6-168">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getskypeforbusinessdeviceusageuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageUserDetail(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="009a6-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="009a6-169">Response</span></span>

<span data-ttu-id="009a6-170">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="009a6-170">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="009a6-171">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="009a6-171">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Used Windows,Used Windows Phone,Used Android Phone,Used iPhone,Used iPad,Report Period
```

### <a name="json"></a><span data-ttu-id="009a6-172">JSON</span><span class="sxs-lookup"><span data-stu-id="009a6-172">JSON</span></span>

<span data-ttu-id="009a6-173">Ниже приводится пример, который возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="009a6-173">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="009a6-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="009a6-174">Request</span></span>

<span data-ttu-id="009a6-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="009a6-175">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getskypeforbusinessdeviceusageuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageUserDetail(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="009a6-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="009a6-176">Response</span></span>

<span data-ttu-id="009a6-177">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="009a6-177">The following is an example of the response.</span></span>

> <span data-ttu-id="009a6-178">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="009a6-178">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 356

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessDeviceUsageUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "lastActivityDate": "2017-09-01", 
      "usedWindows": true, 
      "usedWindowsPhone": false, 
      "usedAndroidPhone": false, 
      "usediPhone": false, 
      "usediPad": false, 
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


