---
title: 'reportRoot: getSkypeForBusinessDeviceUsageUserDetail'
description: Получите сведения об использовании устройств со Skype для бизнеса с разбивкой по пользователям.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: e4075ae4679850b9f46ba75f0934baa4e5f53ba6
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36729534"
---
# <a name="reportroot-getskypeforbusinessdeviceusageuserdetail"></a><span data-ttu-id="c2491-103">reportRoot: getSkypeForBusinessDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="c2491-103">reportRoot: getSkypeForBusinessDeviceUsageUserDetail</span></span>

<span data-ttu-id="c2491-104">Получите сведения об использовании устройств со Skype для бизнеса с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="c2491-104">Get details about Skype for Business device usage by user.</span></span>

> <span data-ttu-id="c2491-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: используемые клиенты Skype для бизнеса](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span><span class="sxs-lookup"><span data-stu-id="c2491-105">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="c2491-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c2491-106">Permissions</span></span>

<span data-ttu-id="c2491-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2491-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c2491-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2491-109">Permission type</span></span>                        | <span data-ttu-id="c2491-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2491-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="c2491-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2491-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c2491-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2491-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="c2491-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2491-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2491-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2491-114">Not supported.</span></span>                           |
| <span data-ttu-id="c2491-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c2491-115">Application</span></span>                            | <span data-ttu-id="c2491-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2491-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="c2491-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2491-117">HTTP request</span></span>


<!-- { "blockType": "samples" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="c2491-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="c2491-118">Function parameters</span></span>

<span data-ttu-id="c2491-119">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="c2491-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="c2491-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="c2491-120">Parameter</span></span> | <span data-ttu-id="c2491-121">Тип</span><span class="sxs-lookup"><span data-stu-id="c2491-121">Type</span></span>   | <span data-ttu-id="c2491-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c2491-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="c2491-123">period</span><span class="sxs-lookup"><span data-stu-id="c2491-123">period</span></span>    | <span data-ttu-id="c2491-124">string</span><span class="sxs-lookup"><span data-stu-id="c2491-124">string</span></span> | <span data-ttu-id="c2491-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="c2491-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="c2491-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="c2491-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="c2491-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="c2491-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="c2491-128">date</span><span class="sxs-lookup"><span data-stu-id="c2491-128">date</span></span>      | <span data-ttu-id="c2491-129">Date</span><span class="sxs-lookup"><span data-stu-id="c2491-129">Date</span></span>   | <span data-ttu-id="c2491-130">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="c2491-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="c2491-131">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="c2491-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="c2491-132">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="c2491-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="c2491-133">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="c2491-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c2491-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c2491-134">Request headers</span></span>

| <span data-ttu-id="c2491-135">Имя</span><span class="sxs-lookup"><span data-stu-id="c2491-135">Name</span></span>          | <span data-ttu-id="c2491-136">Описание</span><span class="sxs-lookup"><span data-stu-id="c2491-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="c2491-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c2491-137">Authorization</span></span> | <span data-ttu-id="c2491-p104">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c2491-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="c2491-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="c2491-140">If-None-Match</span></span> | <span data-ttu-id="c2491-141">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="c2491-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="c2491-142">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="c2491-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="c2491-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2491-143">Response</span></span>

<span data-ttu-id="c2491-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="c2491-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="c2491-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="c2491-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="c2491-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="c2491-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="c2491-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="c2491-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="c2491-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="c2491-148">Report Refresh Date</span></span>
- <span data-ttu-id="c2491-149">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="c2491-149">User Principal Name</span></span>
- <span data-ttu-id="c2491-150">Last Activity Date (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="c2491-150">Last Activity Date</span></span>
- <span data-ttu-id="c2491-151">"Used Windows" (Используемая ОС Windows);</span><span class="sxs-lookup"><span data-stu-id="c2491-151">Used Windows</span></span>
- <span data-ttu-id="c2491-152">"Used Windows Phone" (Используемое устройство Windows Phone);</span><span class="sxs-lookup"><span data-stu-id="c2491-152">Used Windows Phone</span></span>
- <span data-ttu-id="c2491-153">"Used Android Phone" (Используемый телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="c2491-153">Used Android Phone</span></span>
- <span data-ttu-id="c2491-154">"Used iPhone" (Используемый телефон iPhone);</span><span class="sxs-lookup"><span data-stu-id="c2491-154">Used iPhone</span></span>
- <span data-ttu-id="c2491-155">"Used iPad" (Используемое устройство iPad);</span><span class="sxs-lookup"><span data-stu-id="c2491-155">Used iPad</span></span>
- <span data-ttu-id="c2491-156">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="c2491-156">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="c2491-157">Пример</span><span class="sxs-lookup"><span data-stu-id="c2491-157">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c2491-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2491-158">Request</span></span>

<span data-ttu-id="c2491-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2491-159">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c2491-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="c2491-160">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessdeviceusageuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessDeviceUsageUserDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c2491-161">C#</span><span class="sxs-lookup"><span data-stu-id="c2491-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessdeviceusageuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c2491-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c2491-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessdeviceusageuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c2491-163">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c2491-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessdeviceusageuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c2491-164">Java</span><span class="sxs-lookup"><span data-stu-id="c2491-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessdeviceusageuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c2491-165">Ответ</span><span class="sxs-lookup"><span data-stu-id="c2491-165">Response</span></span>

<span data-ttu-id="c2491-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c2491-166">The following is an example of the response.</span></span>

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

<span data-ttu-id="c2491-167">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="c2491-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
