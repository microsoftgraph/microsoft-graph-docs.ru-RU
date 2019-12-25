---
title: 'reportRoot: getSkypeForBusinessDeviceUsageUserDetail'
description: Получите сведения об использовании устройств со Skype для бизнеса с разбивкой по пользователям.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: b422e5683f124d6a457402f0a554708d3e80fcbf
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40864266"
---
# <a name="reportroot-getskypeforbusinessdeviceusageuserdetail"></a><span data-ttu-id="4c55d-103">reportRoot: getSkypeForBusinessDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="4c55d-103">reportRoot: getSkypeForBusinessDeviceUsageUserDetail</span></span>

<span data-ttu-id="4c55d-104">Получите сведения об использовании устройств со Skype для бизнеса с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="4c55d-104">Get details about Skype for Business device usage by user.</span></span>

> <span data-ttu-id="4c55d-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: используемые клиенты Skype для бизнеса](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span><span class="sxs-lookup"><span data-stu-id="4c55d-105">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="4c55d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4c55d-106">Permissions</span></span>

<span data-ttu-id="4c55d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c55d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4c55d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c55d-109">Permission type</span></span>                        | <span data-ttu-id="4c55d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c55d-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="4c55d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c55d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4c55d-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4c55d-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="4c55d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c55d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c55d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c55d-114">Not supported.</span></span>                           |
| <span data-ttu-id="4c55d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4c55d-115">Application</span></span>                            | <span data-ttu-id="4c55d-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4c55d-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="4c55d-117">**Примечание**. для делегированных разрешений, чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя, администратору клиента необходимо назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4c55d-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="4c55d-118">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="4c55d-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="4c55d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c55d-119">HTTP request</span></span>


<!-- { "blockType": "samples" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="4c55d-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="4c55d-120">Function parameters</span></span>

<span data-ttu-id="4c55d-121">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="4c55d-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="4c55d-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="4c55d-122">Parameter</span></span> | <span data-ttu-id="4c55d-123">Тип</span><span class="sxs-lookup"><span data-stu-id="4c55d-123">Type</span></span>   | <span data-ttu-id="4c55d-124">Описание</span><span class="sxs-lookup"><span data-stu-id="4c55d-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="4c55d-125">period</span><span class="sxs-lookup"><span data-stu-id="4c55d-125">period</span></span>    | <span data-ttu-id="4c55d-126">string</span><span class="sxs-lookup"><span data-stu-id="4c55d-126">string</span></span> | <span data-ttu-id="4c55d-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="4c55d-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="4c55d-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="4c55d-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="4c55d-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="4c55d-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="4c55d-130">date</span><span class="sxs-lookup"><span data-stu-id="4c55d-130">date</span></span>      | <span data-ttu-id="4c55d-131">Date</span><span class="sxs-lookup"><span data-stu-id="4c55d-131">Date</span></span>   | <span data-ttu-id="4c55d-132">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="4c55d-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="4c55d-133">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="4c55d-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="4c55d-134">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="4c55d-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="4c55d-135">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="4c55d-135">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4c55d-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4c55d-136">Request headers</span></span>

| <span data-ttu-id="4c55d-137">Имя</span><span class="sxs-lookup"><span data-stu-id="4c55d-137">Name</span></span>          | <span data-ttu-id="4c55d-138">Описание</span><span class="sxs-lookup"><span data-stu-id="4c55d-138">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="4c55d-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4c55d-139">Authorization</span></span> | <span data-ttu-id="4c55d-p105">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c55d-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="4c55d-142">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="4c55d-142">If-None-Match</span></span> | <span data-ttu-id="4c55d-143">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="4c55d-143">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="4c55d-144">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="4c55d-144">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="4c55d-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c55d-145">Response</span></span>

<span data-ttu-id="4c55d-146">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="4c55d-146">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="4c55d-147">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="4c55d-147">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="4c55d-148">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="4c55d-148">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="4c55d-149">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="4c55d-149">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="4c55d-150">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="4c55d-150">Report Refresh Date</span></span>
- <span data-ttu-id="4c55d-151">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="4c55d-151">User Principal Name</span></span>
- <span data-ttu-id="4c55d-152">Last Activity Date (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="4c55d-152">Last Activity Date</span></span>
- <span data-ttu-id="4c55d-153">"Used Windows" (Используемая ОС Windows);</span><span class="sxs-lookup"><span data-stu-id="4c55d-153">Used Windows</span></span>
- <span data-ttu-id="4c55d-154">"Used Windows Phone" (Используемое устройство Windows Phone);</span><span class="sxs-lookup"><span data-stu-id="4c55d-154">Used Windows Phone</span></span>
- <span data-ttu-id="4c55d-155">"Used Android Phone" (Используемый телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="4c55d-155">Used Android Phone</span></span>
- <span data-ttu-id="4c55d-156">"Used iPhone" (Используемый телефон iPhone);</span><span class="sxs-lookup"><span data-stu-id="4c55d-156">Used iPhone</span></span>
- <span data-ttu-id="4c55d-157">"Used iPad" (Используемое устройство iPad);</span><span class="sxs-lookup"><span data-stu-id="4c55d-157">Used iPad</span></span>
- <span data-ttu-id="4c55d-158">Report Period (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="4c55d-158">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="4c55d-159">Пример</span><span class="sxs-lookup"><span data-stu-id="4c55d-159">Example</span></span>

#### <a name="request"></a><span data-ttu-id="4c55d-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c55d-160">Request</span></span>

<span data-ttu-id="4c55d-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c55d-161">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="4c55d-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="4c55d-162">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessdeviceusageuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessDeviceUsageUserDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4c55d-163">C#</span><span class="sxs-lookup"><span data-stu-id="4c55d-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessdeviceusageuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4c55d-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4c55d-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessdeviceusageuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4c55d-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4c55d-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessdeviceusageuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4c55d-166">Java</span><span class="sxs-lookup"><span data-stu-id="4c55d-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessdeviceusageuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4c55d-167">Ответ</span><span class="sxs-lookup"><span data-stu-id="4c55d-167">Response</span></span>

<span data-ttu-id="4c55d-168">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4c55d-168">The following is an example of the response.</span></span>

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

<span data-ttu-id="4c55d-169">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="4c55d-169">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
