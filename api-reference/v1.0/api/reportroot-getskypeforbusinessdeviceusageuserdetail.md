---
title: 'reportRoot: getSkypeForBusinessDeviceUsageUserDetail'
description: Получите сведения об использовании устройств со Skype для бизнеса с разбивкой по пользователям.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 78ee4819bbddcf0619a9f378ff12507bc69534f6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919416"
---
# <a name="reportroot-getskypeforbusinessdeviceusageuserdetail"></a><span data-ttu-id="41874-103">reportRoot: getSkypeForBusinessDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="41874-103">reportRoot: getSkypeForBusinessDeviceUsageUserDetail</span></span>

<span data-ttu-id="41874-104">Получите сведения об использовании устройств со Skype для бизнеса с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="41874-104">Get details about Skype for Business device usage by user.</span></span>

> <span data-ttu-id="41874-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: используемые клиенты Skype для бизнеса](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span><span class="sxs-lookup"><span data-stu-id="41874-105">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="41874-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="41874-106">Permissions</span></span>

<span data-ttu-id="41874-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41874-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="41874-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="41874-109">Permission type</span></span>                        | <span data-ttu-id="41874-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="41874-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="41874-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="41874-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="41874-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="41874-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="41874-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="41874-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41874-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41874-114">Not supported.</span></span>                           |
| <span data-ttu-id="41874-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="41874-115">Application</span></span>                            | <span data-ttu-id="41874-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="41874-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="41874-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="41874-117">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="41874-118">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="41874-118">Function parameters</span></span>

<span data-ttu-id="41874-119">В URL-адресе запроса укажите один из следующих параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="41874-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="41874-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="41874-120">Parameter</span></span> | <span data-ttu-id="41874-121">Тип</span><span class="sxs-lookup"><span data-stu-id="41874-121">Type</span></span>   | <span data-ttu-id="41874-122">Описание</span><span class="sxs-lookup"><span data-stu-id="41874-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="41874-123">period</span><span class="sxs-lookup"><span data-stu-id="41874-123">period</span></span>    | <span data-ttu-id="41874-124">строка</span><span class="sxs-lookup"><span data-stu-id="41874-124">string</span></span> | <span data-ttu-id="41874-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="41874-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="41874-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="41874-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="41874-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="41874-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="41874-128">date</span><span class="sxs-lookup"><span data-stu-id="41874-128">date</span></span>      | <span data-ttu-id="41874-129">Date</span><span class="sxs-lookup"><span data-stu-id="41874-129">Date</span></span>   | <span data-ttu-id="41874-130">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="41874-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="41874-131">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="41874-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="41874-132">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="41874-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="41874-133">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="41874-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="41874-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="41874-134">Request headers</span></span>

| <span data-ttu-id="41874-135">Имя</span><span class="sxs-lookup"><span data-stu-id="41874-135">Name</span></span>          | <span data-ttu-id="41874-136">Описание</span><span class="sxs-lookup"><span data-stu-id="41874-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="41874-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="41874-137">Authorization</span></span> | <span data-ttu-id="41874-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="41874-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="41874-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="41874-140">If-None-Match</span></span> | <span data-ttu-id="41874-141">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="41874-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="41874-142">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="41874-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="41874-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="41874-143">Response</span></span>

<span data-ttu-id="41874-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="41874-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="41874-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="41874-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="41874-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="41874-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="41874-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="41874-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="41874-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="41874-148">Report Refresh Date</span></span>
- <span data-ttu-id="41874-149">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="41874-149">User Principal Name</span></span>
- <span data-ttu-id="41874-150">"Last Activity Date" (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="41874-150">Last Activity Date</span></span>
- <span data-ttu-id="41874-151">"Used Windows" (Используемая ОС Windows);</span><span class="sxs-lookup"><span data-stu-id="41874-151">Used Windows</span></span>
- <span data-ttu-id="41874-152">"Used Windows Phone" (Используемое устройство Windows Phone);</span><span class="sxs-lookup"><span data-stu-id="41874-152">Used Windows Phone</span></span>
- <span data-ttu-id="41874-153">"Used Android Phone" (Используемый телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="41874-153">Used Android Phone</span></span>
- <span data-ttu-id="41874-154">"Used iPhone" (Используемый телефон iPhone);</span><span class="sxs-lookup"><span data-stu-id="41874-154">Used iPhone</span></span>
- <span data-ttu-id="41874-155">"Used iPad" (Используемое устройство iPad);</span><span class="sxs-lookup"><span data-stu-id="41874-155">Used iPad</span></span>
- <span data-ttu-id="41874-156">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="41874-156">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="41874-157">Пример</span><span class="sxs-lookup"><span data-stu-id="41874-157">Example</span></span>

#### <a name="request"></a><span data-ttu-id="41874-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="41874-158">Request</span></span>

<span data-ttu-id="41874-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="41874-159">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessdeviceusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessDeviceUsageUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="41874-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="41874-160">Response</span></span>

<span data-ttu-id="41874-161">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="41874-161">The following is an example of the response.</span></span>

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

<span data-ttu-id="41874-162">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="41874-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Used Windows,Used Windows Phone,Used Android Phone,Used iPhone,Used iPad,Report Period
```
