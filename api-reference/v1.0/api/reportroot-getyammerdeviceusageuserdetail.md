---
title: 'reportRoot: getYammerDeviceUsageUserDetail function'
description: Получение сведений об использовании устройства с Yammer с разбивкой по пользователям.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 9fd43175039608568dbf11f9ebef749b1239e527
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48038314"
---
# <a name="reportroot-getyammerdeviceusageuserdetail-function"></a><span data-ttu-id="653c0-103">reportRoot: getYammerDeviceUsageUserDetail function</span><span class="sxs-lookup"><span data-stu-id="653c0-103">reportRoot: getYammerDeviceUsageUserDetail function</span></span>

<span data-ttu-id="653c0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="653c0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="653c0-105">Получение сведений об использовании устройств с Yammer с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="653c0-105">Get details about Yammer device usage by user.</span></span>

> <span data-ttu-id="653c0-106">**Примечание:** Сведения о различных представлениях отчетов и их именах можно найти в [статье Microsoft 365 Reports-Device Device Usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="653c0-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="653c0-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="653c0-107">Permissions</span></span>

<span data-ttu-id="653c0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="653c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="653c0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="653c0-110">Permission type</span></span>                        | <span data-ttu-id="653c0-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="653c0-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="653c0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="653c0-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="653c0-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="653c0-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="653c0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="653c0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="653c0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="653c0-115">Not supported.</span></span>                           |
| <span data-ttu-id="653c0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="653c0-116">Application</span></span>                            | <span data-ttu-id="653c0-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="653c0-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="653c0-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="653c0-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="653c0-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="653c0-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="653c0-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="653c0-120">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserDetail(period='{period_value}')
GET /reports/getYammerDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="653c0-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="653c0-121">Function parameters</span></span>

<span data-ttu-id="653c0-122">В URL-адресе запроса укажите параметр запроса и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="653c0-122">In the request URL, provide the query parameter with a valid value.</span></span>

| <span data-ttu-id="653c0-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="653c0-123">Parameter</span></span> | <span data-ttu-id="653c0-124">Тип</span><span class="sxs-lookup"><span data-stu-id="653c0-124">Type</span></span>   | <span data-ttu-id="653c0-125">Описание</span><span class="sxs-lookup"><span data-stu-id="653c0-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="653c0-126">period</span><span class="sxs-lookup"><span data-stu-id="653c0-126">period</span></span>    | <span data-ttu-id="653c0-127">string</span><span class="sxs-lookup"><span data-stu-id="653c0-127">string</span></span> | <span data-ttu-id="653c0-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="653c0-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="653c0-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="653c0-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="653c0-130">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="653c0-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="653c0-131">date</span><span class="sxs-lookup"><span data-stu-id="653c0-131">date</span></span>      | <span data-ttu-id="653c0-132">Date</span><span class="sxs-lookup"><span data-stu-id="653c0-132">Date</span></span>   | <span data-ttu-id="653c0-133">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="653c0-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="653c0-134">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="653c0-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="653c0-135">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="653c0-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="653c0-136">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="653c0-136">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="653c0-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="653c0-137">Request headers</span></span>

| <span data-ttu-id="653c0-138">Имя</span><span class="sxs-lookup"><span data-stu-id="653c0-138">Name</span></span>          | <span data-ttu-id="653c0-139">Описание</span><span class="sxs-lookup"><span data-stu-id="653c0-139">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="653c0-140">Авторизация</span><span class="sxs-lookup"><span data-stu-id="653c0-140">Authorization</span></span> | <span data-ttu-id="653c0-p105">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="653c0-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="653c0-143">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="653c0-143">If-None-Match</span></span> | <span data-ttu-id="653c0-144">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="653c0-144">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="653c0-145">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="653c0-145">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="653c0-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="653c0-146">Response</span></span>

<span data-ttu-id="653c0-147">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="653c0-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="653c0-148">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="653c0-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="653c0-149">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="653c0-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="653c0-150">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="653c0-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="653c0-151">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="653c0-151">Report Refresh Date</span></span>
- <span data-ttu-id="653c0-152">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="653c0-152">User Principal Name</span></span>
- <span data-ttu-id="653c0-153">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="653c0-153">Display Name</span></span>
- <span data-ttu-id="653c0-154">"User State" (Состояние пользователя);</span><span class="sxs-lookup"><span data-stu-id="653c0-154">User State</span></span>
- <span data-ttu-id="653c0-155">"State Change Date" (Дата изменения состояния);</span><span class="sxs-lookup"><span data-stu-id="653c0-155">State Change Date</span></span>
- <span data-ttu-id="653c0-156">"Last Activity Date" (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="653c0-156">Last Activity Date</span></span>
- <span data-ttu-id="653c0-157">"Used Web" (Используемое веб-приложение);</span><span class="sxs-lookup"><span data-stu-id="653c0-157">Used Web</span></span>
- <span data-ttu-id="653c0-158">"Used Windows Phone" (Используемое устройство Windows Phone);</span><span class="sxs-lookup"><span data-stu-id="653c0-158">Used Windows Phone</span></span>
- <span data-ttu-id="653c0-159">"Used Android Phone" (Используемый телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="653c0-159">Used Android Phone</span></span>
- <span data-ttu-id="653c0-160">"Used iPhone" (Используемый телефон iPhone);</span><span class="sxs-lookup"><span data-stu-id="653c0-160">Used iPhone</span></span>
- <span data-ttu-id="653c0-161">"Used iPad" (Используемое устройство iPad);</span><span class="sxs-lookup"><span data-stu-id="653c0-161">Used iPad</span></span>
- <span data-ttu-id="653c0-162">"Used Others" (Другое используемое);</span><span class="sxs-lookup"><span data-stu-id="653c0-162">Used Others</span></span>
- <span data-ttu-id="653c0-163">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="653c0-163">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="653c0-164">Пример</span><span class="sxs-lookup"><span data-stu-id="653c0-164">Example</span></span>

#### <a name="request"></a><span data-ttu-id="653c0-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="653c0-165">Request</span></span>

<span data-ttu-id="653c0-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="653c0-166">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getyammerdeviceusageuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getYammerDeviceUsageUserDetail(period='D7')
```


#### <a name="response"></a><span data-ttu-id="653c0-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="653c0-167">Response</span></span>

<span data-ttu-id="653c0-168">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="653c0-168">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

#### <a name="request"></a><span data-ttu-id="653c0-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="653c0-169">Request</span></span>

<span data-ttu-id="653c0-170">При вызове с `date` параметром область применения отчета определяется на заданную дату.</span><span class="sxs-lookup"><span data-stu-id="653c0-170">If called with the `date` parameter, the report is scoped to usage on the given date.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammerdeviceusageuserdetail_date"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerDeviceUsageUserDetail(date='2018-03-05')
```

#### <a name="response"></a><span data-ttu-id="653c0-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="653c0-171">Response</span></span>

<span data-ttu-id="653c0-172">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="653c0-172">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.report"
} -->

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="653c0-173">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="653c0-173">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,User State,State Change Date,Last Activity Date,Used Web,Used Windows Phone,Used Android Phone,Used iPhone,Used iPad,Used Others,Report Period
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

