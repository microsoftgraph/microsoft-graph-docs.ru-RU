---
title: 'reportRoot: getYammerDeviceUsageUserDetail function'
description: Получение сведений об использовании устройства с Yammer с разбивкой по пользователям.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: a338d005535263d68530bfb63ddfd2baebdbe925
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33603871"
---
# <a name="reportroot-getyammerdeviceusageuserdetail-function"></a><span data-ttu-id="7895a-103">reportRoot: getYammerDeviceUsageUserDetail function</span><span class="sxs-lookup"><span data-stu-id="7895a-103">reportRoot: getYammerDeviceUsageUserDetail function</span></span>

<span data-ttu-id="7895a-104">Получение сведений об использовании устройства с Yammer с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="7895a-104">Get details about Yammer device usage by user.</span></span>

> <span data-ttu-id="7895a-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: использование устройств с Yammer](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="7895a-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="7895a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7895a-106">Permissions</span></span>

<span data-ttu-id="7895a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7895a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7895a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7895a-109">Permission type</span></span>                        | <span data-ttu-id="7895a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7895a-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="7895a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7895a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7895a-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7895a-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="7895a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7895a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7895a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7895a-114">Not supported.</span></span>                           |
| <span data-ttu-id="7895a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7895a-115">Application</span></span>                            | <span data-ttu-id="7895a-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7895a-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="7895a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7895a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserDetail(period='{period_value}')
GET /reports/getYammerDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="7895a-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="7895a-118">Function parameters</span></span>

<span data-ttu-id="7895a-119">В URL-адресе запроса укажите параметр запроса и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="7895a-119">In the request URL, provide the query parameter with a valid value.</span></span>

| <span data-ttu-id="7895a-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="7895a-120">Parameter</span></span> | <span data-ttu-id="7895a-121">Тип</span><span class="sxs-lookup"><span data-stu-id="7895a-121">Type</span></span>   | <span data-ttu-id="7895a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="7895a-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="7895a-123">period</span><span class="sxs-lookup"><span data-stu-id="7895a-123">period</span></span>    | <span data-ttu-id="7895a-124">string</span><span class="sxs-lookup"><span data-stu-id="7895a-124">string</span></span> | <span data-ttu-id="7895a-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="7895a-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="7895a-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="7895a-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="7895a-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="7895a-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="7895a-128">date</span><span class="sxs-lookup"><span data-stu-id="7895a-128">date</span></span>      | <span data-ttu-id="7895a-129">Date</span><span class="sxs-lookup"><span data-stu-id="7895a-129">Date</span></span>   | <span data-ttu-id="7895a-130">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="7895a-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="7895a-131">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="7895a-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="7895a-132">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="7895a-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="7895a-133">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="7895a-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7895a-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7895a-134">Request headers</span></span>

| <span data-ttu-id="7895a-135">Имя</span><span class="sxs-lookup"><span data-stu-id="7895a-135">Name</span></span>          | <span data-ttu-id="7895a-136">Описание</span><span class="sxs-lookup"><span data-stu-id="7895a-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="7895a-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7895a-137">Authorization</span></span> | <span data-ttu-id="7895a-p104">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7895a-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="7895a-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="7895a-140">If-None-Match</span></span> | <span data-ttu-id="7895a-141">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="7895a-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="7895a-142">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="7895a-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="7895a-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="7895a-143">Response</span></span>

<span data-ttu-id="7895a-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="7895a-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="7895a-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="7895a-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="7895a-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="7895a-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="7895a-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="7895a-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="7895a-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="7895a-148">Report Refresh Date</span></span>
- <span data-ttu-id="7895a-149">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="7895a-149">User Principal Name</span></span>
- <span data-ttu-id="7895a-150">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="7895a-150">Display Name</span></span>
- <span data-ttu-id="7895a-151">"User State" (Состояние пользователя);</span><span class="sxs-lookup"><span data-stu-id="7895a-151">User State</span></span>
- <span data-ttu-id="7895a-152">"State Change Date" (Дата изменения состояния);</span><span class="sxs-lookup"><span data-stu-id="7895a-152">State Change Date</span></span>
- <span data-ttu-id="7895a-153">"Last Activity Date" (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="7895a-153">Last Activity Date</span></span>
- <span data-ttu-id="7895a-154">"Used Web" (Используемое веб-приложение);</span><span class="sxs-lookup"><span data-stu-id="7895a-154">Used Web</span></span>
- <span data-ttu-id="7895a-155">"Used Windows Phone" (Используемое устройство Windows Phone);</span><span class="sxs-lookup"><span data-stu-id="7895a-155">Used Windows Phone</span></span>
- <span data-ttu-id="7895a-156">"Used Android Phone" (Используемый телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="7895a-156">Used Android Phone</span></span>
- <span data-ttu-id="7895a-157">"Used iPhone" (Используемый телефон iPhone);</span><span class="sxs-lookup"><span data-stu-id="7895a-157">Used iPhone</span></span>
- <span data-ttu-id="7895a-158">"Used iPad" (Используемое устройство iPad);</span><span class="sxs-lookup"><span data-stu-id="7895a-158">Used iPad</span></span>
- <span data-ttu-id="7895a-159">"Used Others" (Другое используемое);</span><span class="sxs-lookup"><span data-stu-id="7895a-159">Used Others</span></span>
- <span data-ttu-id="7895a-160">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="7895a-160">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="7895a-161">Пример</span><span class="sxs-lookup"><span data-stu-id="7895a-161">Example</span></span>

#### <a name="request"></a><span data-ttu-id="7895a-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="7895a-162">Request</span></span>

<span data-ttu-id="7895a-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7895a-163">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammerdeviceusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerDeviceUsageUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="7895a-164">Ответ</span><span class="sxs-lookup"><span data-stu-id="7895a-164">Response</span></span>

<span data-ttu-id="7895a-165">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7895a-165">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="7895a-166">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="7895a-166">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7895a-167">Языках</span><span class="sxs-lookup"><span data-stu-id="7895a-167">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getyammerdeviceusageuserdetail-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7895a-168">Язык</span><span class="sxs-lookup"><span data-stu-id="7895a-168">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getyammerdeviceusageuserdetail-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

#### <a name="request"></a><span data-ttu-id="7895a-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="7895a-169">Request</span></span>

<span data-ttu-id="7895a-170">При вызове с `date` параметром область применения отчета определяется на заданную дату.</span><span class="sxs-lookup"><span data-stu-id="7895a-170">If called with the `date` parameter, the report is scoped to usage on the given date.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammerdeviceusageuserdetail_date"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerDeviceUsageUserDetail(date='2018-03-05')
```

#### <a name="response"></a><span data-ttu-id="7895a-171">Ответ</span><span class="sxs-lookup"><span data-stu-id="7895a-171">Response</span></span>

<span data-ttu-id="7895a-172">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7895a-172">The following is an example of the response.</span></span>

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

<span data-ttu-id="7895a-173">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="7895a-173">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
    "Error: /api-reference/v1.0/api/reportroot-getyammerdeviceusageuserdetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getyammerdeviceusageuserdetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
