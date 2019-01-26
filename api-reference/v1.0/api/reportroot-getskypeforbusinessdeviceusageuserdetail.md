---
title: 'reportRoot: getSkypeForBusinessDeviceUsageUserDetail'
description: Получите сведения об использовании устройств со Skype для бизнеса с разбивкой по пользователям.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: bf4fb6da750b54d220ca6d7319132ff62b3661f5
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577300"
---
# <a name="reportroot-getskypeforbusinessdeviceusageuserdetail"></a><span data-ttu-id="fb7c3-103">reportRoot: getSkypeForBusinessDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="fb7c3-103">reportRoot: getSkypeForBusinessDeviceUsageUserDetail</span></span>

<span data-ttu-id="fb7c3-104">Получите сведения об использовании устройств со Skype для бизнеса с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="fb7c3-104">Get details about Skype for Business device usage by user.</span></span>

> <span data-ttu-id="fb7c3-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: используемые клиенты Skype для бизнеса](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span><span class="sxs-lookup"><span data-stu-id="fb7c3-105">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="fb7c3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fb7c3-106">Permissions</span></span>

<span data-ttu-id="fb7c3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb7c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fb7c3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fb7c3-109">Permission type</span></span>                        | <span data-ttu-id="fb7c3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fb7c3-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="fb7c3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fb7c3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="fb7c3-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fb7c3-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="fb7c3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fb7c3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb7c3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb7c3-114">Not supported.</span></span>                           |
| <span data-ttu-id="fb7c3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fb7c3-115">Application</span></span>                            | <span data-ttu-id="fb7c3-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fb7c3-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="fb7c3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fb7c3-117">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="fb7c3-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="fb7c3-118">Function parameters</span></span>

<span data-ttu-id="fb7c3-119">В URL-адресе запроса укажите один из следующих параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="fb7c3-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="fb7c3-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="fb7c3-120">Parameter</span></span> | <span data-ttu-id="fb7c3-121">Тип</span><span class="sxs-lookup"><span data-stu-id="fb7c3-121">Type</span></span>   | <span data-ttu-id="fb7c3-122">Описание</span><span class="sxs-lookup"><span data-stu-id="fb7c3-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="fb7c3-123">period</span><span class="sxs-lookup"><span data-stu-id="fb7c3-123">period</span></span>    | <span data-ttu-id="fb7c3-124">строка</span><span class="sxs-lookup"><span data-stu-id="fb7c3-124">string</span></span> | <span data-ttu-id="fb7c3-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="fb7c3-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="fb7c3-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="fb7c3-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="fb7c3-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="fb7c3-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="fb7c3-128">date</span><span class="sxs-lookup"><span data-stu-id="fb7c3-128">date</span></span>      | <span data-ttu-id="fb7c3-129">Date</span><span class="sxs-lookup"><span data-stu-id="fb7c3-129">Date</span></span>   | <span data-ttu-id="fb7c3-130">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="fb7c3-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="fb7c3-131">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="fb7c3-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="fb7c3-132">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="fb7c3-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="fb7c3-133">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="fb7c3-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fb7c3-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fb7c3-134">Request headers</span></span>

| <span data-ttu-id="fb7c3-135">Имя</span><span class="sxs-lookup"><span data-stu-id="fb7c3-135">Name</span></span>          | <span data-ttu-id="fb7c3-136">Описание</span><span class="sxs-lookup"><span data-stu-id="fb7c3-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="fb7c3-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fb7c3-137">Authorization</span></span> | <span data-ttu-id="fb7c3-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fb7c3-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="fb7c3-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="fb7c3-140">If-None-Match</span></span> | <span data-ttu-id="fb7c3-141">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="fb7c3-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="fb7c3-142">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="fb7c3-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="fb7c3-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb7c3-143">Response</span></span>

<span data-ttu-id="fb7c3-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="fb7c3-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="fb7c3-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="fb7c3-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="fb7c3-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="fb7c3-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="fb7c3-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="fb7c3-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="fb7c3-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="fb7c3-148">Report Refresh Date</span></span>
- <span data-ttu-id="fb7c3-149">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="fb7c3-149">User Principal Name</span></span>
- <span data-ttu-id="fb7c3-150">"Last Activity Date" (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="fb7c3-150">Last Activity Date</span></span>
- <span data-ttu-id="fb7c3-151">"Used Windows" (Используемая ОС Windows);</span><span class="sxs-lookup"><span data-stu-id="fb7c3-151">Used Windows</span></span>
- <span data-ttu-id="fb7c3-152">"Used Windows Phone" (Используемое устройство Windows Phone);</span><span class="sxs-lookup"><span data-stu-id="fb7c3-152">Used Windows Phone</span></span>
- <span data-ttu-id="fb7c3-153">"Used Android Phone" (Используемый телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="fb7c3-153">Used Android Phone</span></span>
- <span data-ttu-id="fb7c3-154">"Used iPhone" (Используемый телефон iPhone);</span><span class="sxs-lookup"><span data-stu-id="fb7c3-154">Used iPhone</span></span>
- <span data-ttu-id="fb7c3-155">"Used iPad" (Используемое устройство iPad);</span><span class="sxs-lookup"><span data-stu-id="fb7c3-155">Used iPad</span></span>
- <span data-ttu-id="fb7c3-156">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="fb7c3-156">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="fb7c3-157">Пример</span><span class="sxs-lookup"><span data-stu-id="fb7c3-157">Example</span></span>

#### <a name="request"></a><span data-ttu-id="fb7c3-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="fb7c3-158">Request</span></span>

<span data-ttu-id="fb7c3-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fb7c3-159">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessdeviceusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessDeviceUsageUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="fb7c3-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb7c3-160">Response</span></span>

<span data-ttu-id="fb7c3-161">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fb7c3-161">The following is an example of the response.</span></span>

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

<span data-ttu-id="fb7c3-162">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="fb7c3-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Used Windows,Used Windows Phone,Used Android Phone,Used iPhone,Used iPad,Report Period
```
