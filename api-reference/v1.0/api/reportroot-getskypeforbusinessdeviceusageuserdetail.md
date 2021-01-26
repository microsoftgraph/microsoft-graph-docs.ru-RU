---
title: 'reportRoot: getSkypeForBusinessDeviceUsageUserDetail'
description: Получите сведения об использовании устройств со Skype для бизнеса с разбивкой по пользователям.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 3314ea443fecc1a9fc93236ac93b8c137d6cf2bc
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981419"
---
# <a name="reportroot-getskypeforbusinessdeviceusageuserdetail"></a><span data-ttu-id="baca8-103">reportRoot: getSkypeForBusinessDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="baca8-103">reportRoot: getSkypeForBusinessDeviceUsageUserDetail</span></span>

<span data-ttu-id="baca8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="baca8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="baca8-105">Получите сведения об использовании устройств со Skype для бизнеса с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="baca8-105">Get details about Skype for Business device usage by user.</span></span>

> <span data-ttu-id="baca8-106">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [отчетах Microsoft 365 : используемые клиенты Skype для бизнеса.](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3)</span><span class="sxs-lookup"><span data-stu-id="baca8-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="baca8-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="baca8-107">Permissions</span></span>

<span data-ttu-id="baca8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="baca8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="baca8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="baca8-110">Permission type</span></span>                        | <span data-ttu-id="baca8-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="baca8-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="baca8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="baca8-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="baca8-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="baca8-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="baca8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="baca8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="baca8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="baca8-115">Not supported.</span></span>                           |
| <span data-ttu-id="baca8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="baca8-116">Application</span></span>                            | <span data-ttu-id="baca8-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="baca8-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="baca8-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="baca8-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="baca8-119">Дополнительные сведения см. в статье [Авторизация для API с целью чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="baca8-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="baca8-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="baca8-120">HTTP request</span></span>


<!-- { "blockType": "samples" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="baca8-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="baca8-121">Function parameters</span></span>

<span data-ttu-id="baca8-122">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="baca8-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="baca8-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="baca8-123">Parameter</span></span> | <span data-ttu-id="baca8-124">Тип</span><span class="sxs-lookup"><span data-stu-id="baca8-124">Type</span></span>   | <span data-ttu-id="baca8-125">Описание</span><span class="sxs-lookup"><span data-stu-id="baca8-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="baca8-126">period</span><span class="sxs-lookup"><span data-stu-id="baca8-126">period</span></span>    | <span data-ttu-id="baca8-127">string</span><span class="sxs-lookup"><span data-stu-id="baca8-127">string</span></span> | <span data-ttu-id="baca8-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="baca8-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="baca8-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="baca8-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="baca8-130">Эти значения указываются в формате D *n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="baca8-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="baca8-131">date</span><span class="sxs-lookup"><span data-stu-id="baca8-131">date</span></span>      | <span data-ttu-id="baca8-132">Date</span><span class="sxs-lookup"><span data-stu-id="baca8-132">Date</span></span>   | <span data-ttu-id="baca8-133">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="baca8-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="baca8-134">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="baca8-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="baca8-135">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="baca8-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="baca8-136">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="baca8-136">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="baca8-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="baca8-137">Request headers</span></span>

| <span data-ttu-id="baca8-138">Имя</span><span class="sxs-lookup"><span data-stu-id="baca8-138">Name</span></span>          | <span data-ttu-id="baca8-139">Описание</span><span class="sxs-lookup"><span data-stu-id="baca8-139">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="baca8-140">Авторизация</span><span class="sxs-lookup"><span data-stu-id="baca8-140">Authorization</span></span> | <span data-ttu-id="baca8-p105">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="baca8-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="baca8-143">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="baca8-143">If-None-Match</span></span> | <span data-ttu-id="baca8-144">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="baca8-144">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="baca8-145">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="baca8-145">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="baca8-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="baca8-146">Response</span></span>

<span data-ttu-id="baca8-147">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="baca8-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="baca8-148">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="baca8-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="baca8-149">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="baca8-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="baca8-150">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="baca8-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="baca8-151">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="baca8-151">Report Refresh Date</span></span>
- <span data-ttu-id="baca8-152">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="baca8-152">User Principal Name</span></span>
- <span data-ttu-id="baca8-153">Last Activity Date (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="baca8-153">Last Activity Date</span></span>
- <span data-ttu-id="baca8-154">"Used Windows" (Используемая ОС Windows);</span><span class="sxs-lookup"><span data-stu-id="baca8-154">Used Windows</span></span>
- <span data-ttu-id="baca8-155">"Used Windows Phone" (Используемое устройство Windows Phone);</span><span class="sxs-lookup"><span data-stu-id="baca8-155">Used Windows Phone</span></span>
- <span data-ttu-id="baca8-156">"Used Android Phone" (Используемый телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="baca8-156">Used Android Phone</span></span>
- <span data-ttu-id="baca8-157">"Used iPhone" (Используемый телефон iPhone);</span><span class="sxs-lookup"><span data-stu-id="baca8-157">Used iPhone</span></span>
- <span data-ttu-id="baca8-158">"Used iPad" (Используемое устройство iPad);</span><span class="sxs-lookup"><span data-stu-id="baca8-158">Used iPad</span></span>
- <span data-ttu-id="baca8-159">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="baca8-159">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="baca8-160">Пример</span><span class="sxs-lookup"><span data-stu-id="baca8-160">Example</span></span>

#### <a name="request"></a><span data-ttu-id="baca8-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="baca8-161">Request</span></span>

<span data-ttu-id="baca8-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="baca8-162">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessdeviceusageuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessDeviceUsageUserDetail(period='D7')
```


#### <a name="response"></a><span data-ttu-id="baca8-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="baca8-163">Response</span></span>

<span data-ttu-id="baca8-164">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="baca8-164">The following is an example of the response.</span></span>

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

<span data-ttu-id="baca8-165">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="baca8-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Used Windows,Used Windows Phone,Used Android Phone,Used iPhone,Used iPad,Report Period
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

