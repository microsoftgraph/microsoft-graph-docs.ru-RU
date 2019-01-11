---
title: 'reportRoot: getYammerDeviceUsageUserDetail function'
description: Получение сведений об использовании устройства с Yammer с разбивкой по пользователям.
localization_priority: Normal
ms.openlocfilehash: 3097d2aa384389e29c0419265d49cde663d763e6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880915"
---
# <a name="reportroot-getyammerdeviceusageuserdetail-function"></a><span data-ttu-id="6c1e6-103">reportRoot: getYammerDeviceUsageUserDetail function</span><span class="sxs-lookup"><span data-stu-id="6c1e6-103">reportRoot: getYammerDeviceUsageUserDetail function</span></span>

<span data-ttu-id="6c1e6-104">Получение сведений об использовании устройства с Yammer с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="6c1e6-104">Get details about Yammer device usage by user.</span></span>

> <span data-ttu-id="6c1e6-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: использование устройств с Yammer](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="6c1e6-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="6c1e6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6c1e6-106">Permissions</span></span>

<span data-ttu-id="6c1e6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c1e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6c1e6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6c1e6-109">Permission type</span></span>                        | <span data-ttu-id="6c1e6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6c1e6-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="6c1e6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6c1e6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6c1e6-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c1e6-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="6c1e6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6c1e6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c1e6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c1e6-114">Not supported.</span></span>                           |
| <span data-ttu-id="6c1e6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6c1e6-115">Application</span></span>                            | <span data-ttu-id="6c1e6-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c1e6-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="6c1e6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6c1e6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserDetail(period='{period_value}')
GET /reports/getYammerDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="6c1e6-118">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="6c1e6-118">Function parameters</span></span>

<span data-ttu-id="6c1e6-119">В URL-адресе запроса укажите параметр запроса и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="6c1e6-119">In the request URL, provide the query parameter with a valid value.</span></span>

| <span data-ttu-id="6c1e6-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="6c1e6-120">Parameter</span></span> | <span data-ttu-id="6c1e6-121">Тип</span><span class="sxs-lookup"><span data-stu-id="6c1e6-121">Type</span></span>   | <span data-ttu-id="6c1e6-122">Описание</span><span class="sxs-lookup"><span data-stu-id="6c1e6-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="6c1e6-123">period</span><span class="sxs-lookup"><span data-stu-id="6c1e6-123">period</span></span>    | <span data-ttu-id="6c1e6-124">строка</span><span class="sxs-lookup"><span data-stu-id="6c1e6-124">string</span></span> | <span data-ttu-id="6c1e6-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="6c1e6-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="6c1e6-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="6c1e6-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="6c1e6-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="6c1e6-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="6c1e6-128">date</span><span class="sxs-lookup"><span data-stu-id="6c1e6-128">date</span></span>      | <span data-ttu-id="6c1e6-129">Date</span><span class="sxs-lookup"><span data-stu-id="6c1e6-129">Date</span></span>   | <span data-ttu-id="6c1e6-130">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="6c1e6-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="6c1e6-131">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="6c1e6-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="6c1e6-132">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="6c1e6-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="6c1e6-133">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="6c1e6-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6c1e6-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6c1e6-134">Request headers</span></span>

| <span data-ttu-id="6c1e6-135">Имя</span><span class="sxs-lookup"><span data-stu-id="6c1e6-135">Name</span></span>          | <span data-ttu-id="6c1e6-136">Описание</span><span class="sxs-lookup"><span data-stu-id="6c1e6-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="6c1e6-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6c1e6-137">Authorization</span></span> | <span data-ttu-id="6c1e6-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6c1e6-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="6c1e6-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="6c1e6-140">If-None-Match</span></span> | <span data-ttu-id="6c1e6-141">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="6c1e6-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="6c1e6-142">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="6c1e6-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="6c1e6-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="6c1e6-143">Response</span></span>

<span data-ttu-id="6c1e6-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="6c1e6-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="6c1e6-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="6c1e6-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="6c1e6-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="6c1e6-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="6c1e6-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="6c1e6-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="6c1e6-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="6c1e6-148">Report Refresh Date</span></span>
- <span data-ttu-id="6c1e6-149">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="6c1e6-149">User Principal Name</span></span>
- <span data-ttu-id="6c1e6-150">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="6c1e6-150">Display Name</span></span>
- <span data-ttu-id="6c1e6-151">"User State" (Состояние пользователя);</span><span class="sxs-lookup"><span data-stu-id="6c1e6-151">User State</span></span>
- <span data-ttu-id="6c1e6-152">"State Change Date" (Дата изменения состояния);</span><span class="sxs-lookup"><span data-stu-id="6c1e6-152">State Change Date</span></span>
- <span data-ttu-id="6c1e6-153">"Last Activity Date" (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="6c1e6-153">Last Activity Date</span></span>
- <span data-ttu-id="6c1e6-154">"Used Web" (Используемое веб-приложение);</span><span class="sxs-lookup"><span data-stu-id="6c1e6-154">Used Web</span></span>
- <span data-ttu-id="6c1e6-155">"Used Windows Phone" (Используемое устройство Windows Phone);</span><span class="sxs-lookup"><span data-stu-id="6c1e6-155">Used Windows Phone</span></span>
- <span data-ttu-id="6c1e6-156">"Used Android Phone" (Используемый телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="6c1e6-156">Used Android Phone</span></span>
- <span data-ttu-id="6c1e6-157">"Used iPhone" (Используемый телефон iPhone);</span><span class="sxs-lookup"><span data-stu-id="6c1e6-157">Used iPhone</span></span>
- <span data-ttu-id="6c1e6-158">"Used iPad" (Используемое устройство iPad);</span><span class="sxs-lookup"><span data-stu-id="6c1e6-158">Used iPad</span></span>
- <span data-ttu-id="6c1e6-159">"Used Others" (Другое используемое);</span><span class="sxs-lookup"><span data-stu-id="6c1e6-159">Used Others</span></span>
- <span data-ttu-id="6c1e6-160">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="6c1e6-160">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="6c1e6-161">Пример</span><span class="sxs-lookup"><span data-stu-id="6c1e6-161">Example</span></span>

#### <a name="request"></a><span data-ttu-id="6c1e6-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="6c1e6-162">Request</span></span>

<span data-ttu-id="6c1e6-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6c1e6-163">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammerdeviceusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerDeviceUsageUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="6c1e6-164">Ответ</span><span class="sxs-lookup"><span data-stu-id="6c1e6-164">Response</span></span>

<span data-ttu-id="6c1e6-165">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6c1e6-165">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

#### <a name="request"></a><span data-ttu-id="6c1e6-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="6c1e6-166">Request</span></span>

<span data-ttu-id="6c1e6-167">При вызове с `date` пределах параметр отчета об использовании на данной даты.</span><span class="sxs-lookup"><span data-stu-id="6c1e6-167">If called with the `date` parameter, the report is scoped to usage on the given date.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammerdeviceusageuserdetail_date"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerDeviceUsageUserDetail(date='2018-03-05')
```

#### <a name="response"></a><span data-ttu-id="6c1e6-168">Ответ</span><span class="sxs-lookup"><span data-stu-id="6c1e6-168">Response</span></span>

<span data-ttu-id="6c1e6-169">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6c1e6-169">The following is an example of the response.</span></span>

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

<span data-ttu-id="6c1e6-170">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="6c1e6-170">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,User State,State Change Date,Last Activity Date,Used Web,Used Windows Phone,Used Android Phone,Used iPhone,Used iPad,Used Others,Report Period
```
