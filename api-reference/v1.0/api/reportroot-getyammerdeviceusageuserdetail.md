---
title: 'reportRoot: getYammerDeviceUsageUserDetail function'
description: Получение сведений об использовании устройства с Yammer с разбивкой по пользователям.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: be3e699f8d023bdc6d331dc7e9d2c9d14f558a21
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865206"
---
# <a name="reportroot-getyammerdeviceusageuserdetail-function"></a><span data-ttu-id="ed6d0-103">reportRoot: getYammerDeviceUsageUserDetail function</span><span class="sxs-lookup"><span data-stu-id="ed6d0-103">reportRoot: getYammerDeviceUsageUserDetail function</span></span>

<span data-ttu-id="ed6d0-104">Получение сведений об использовании устройства с Yammer с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="ed6d0-104">Get details about Yammer device usage by user.</span></span>

> <span data-ttu-id="ed6d0-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: использование устройств с Yammer](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="ed6d0-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="ed6d0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ed6d0-106">Permissions</span></span>

<span data-ttu-id="ed6d0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed6d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ed6d0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ed6d0-109">Permission type</span></span>                        | <span data-ttu-id="ed6d0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ed6d0-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ed6d0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ed6d0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ed6d0-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ed6d0-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ed6d0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ed6d0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed6d0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed6d0-114">Not supported.</span></span>                           |
| <span data-ttu-id="ed6d0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ed6d0-115">Application</span></span>                            | <span data-ttu-id="ed6d0-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ed6d0-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="ed6d0-117">**Примечание**. для делегированных разрешений, чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя, администратору клиента необходимо назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ed6d0-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="ed6d0-118">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="ed6d0-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="ed6d0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ed6d0-119">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserDetail(period='{period_value}')
GET /reports/getYammerDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="ed6d0-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="ed6d0-120">Function parameters</span></span>

<span data-ttu-id="ed6d0-121">В URL-адресе запроса укажите параметр запроса и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="ed6d0-121">In the request URL, provide the query parameter with a valid value.</span></span>

| <span data-ttu-id="ed6d0-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="ed6d0-122">Parameter</span></span> | <span data-ttu-id="ed6d0-123">Тип</span><span class="sxs-lookup"><span data-stu-id="ed6d0-123">Type</span></span>   | <span data-ttu-id="ed6d0-124">Описание</span><span class="sxs-lookup"><span data-stu-id="ed6d0-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="ed6d0-125">period</span><span class="sxs-lookup"><span data-stu-id="ed6d0-125">period</span></span>    | <span data-ttu-id="ed6d0-126">string</span><span class="sxs-lookup"><span data-stu-id="ed6d0-126">string</span></span> | <span data-ttu-id="ed6d0-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="ed6d0-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="ed6d0-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="ed6d0-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="ed6d0-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="ed6d0-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="ed6d0-130">date</span><span class="sxs-lookup"><span data-stu-id="ed6d0-130">date</span></span>      | <span data-ttu-id="ed6d0-131">Date</span><span class="sxs-lookup"><span data-stu-id="ed6d0-131">Date</span></span>   | <span data-ttu-id="ed6d0-132">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="ed6d0-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="ed6d0-133">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="ed6d0-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="ed6d0-134">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="ed6d0-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="ed6d0-135">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="ed6d0-135">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ed6d0-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ed6d0-136">Request headers</span></span>

| <span data-ttu-id="ed6d0-137">Имя</span><span class="sxs-lookup"><span data-stu-id="ed6d0-137">Name</span></span>          | <span data-ttu-id="ed6d0-138">Описание</span><span class="sxs-lookup"><span data-stu-id="ed6d0-138">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="ed6d0-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ed6d0-139">Authorization</span></span> | <span data-ttu-id="ed6d0-p105">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ed6d0-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="ed6d0-142">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="ed6d0-142">If-None-Match</span></span> | <span data-ttu-id="ed6d0-143">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="ed6d0-143">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="ed6d0-144">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="ed6d0-144">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="ed6d0-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="ed6d0-145">Response</span></span>

<span data-ttu-id="ed6d0-146">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="ed6d0-146">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ed6d0-147">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="ed6d0-147">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ed6d0-148">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="ed6d0-148">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ed6d0-149">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="ed6d0-149">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="ed6d0-150">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="ed6d0-150">Report Refresh Date</span></span>
- <span data-ttu-id="ed6d0-151">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="ed6d0-151">User Principal Name</span></span>
- <span data-ttu-id="ed6d0-152">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="ed6d0-152">Display Name</span></span>
- <span data-ttu-id="ed6d0-153">"User State" (Состояние пользователя);</span><span class="sxs-lookup"><span data-stu-id="ed6d0-153">User State</span></span>
- <span data-ttu-id="ed6d0-154">"State Change Date" (Дата изменения состояния);</span><span class="sxs-lookup"><span data-stu-id="ed6d0-154">State Change Date</span></span>
- <span data-ttu-id="ed6d0-155">"Last Activity Date" (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="ed6d0-155">Last Activity Date</span></span>
- <span data-ttu-id="ed6d0-156">"Used Web" (Используемое веб-приложение);</span><span class="sxs-lookup"><span data-stu-id="ed6d0-156">Used Web</span></span>
- <span data-ttu-id="ed6d0-157">"Used Windows Phone" (Используемое устройство Windows Phone);</span><span class="sxs-lookup"><span data-stu-id="ed6d0-157">Used Windows Phone</span></span>
- <span data-ttu-id="ed6d0-158">"Used Android Phone" (Используемый телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="ed6d0-158">Used Android Phone</span></span>
- <span data-ttu-id="ed6d0-159">"Used iPhone" (Используемый телефон iPhone);</span><span class="sxs-lookup"><span data-stu-id="ed6d0-159">Used iPhone</span></span>
- <span data-ttu-id="ed6d0-160">"Used iPad" (Используемое устройство iPad);</span><span class="sxs-lookup"><span data-stu-id="ed6d0-160">Used iPad</span></span>
- <span data-ttu-id="ed6d0-161">"Used Others" (Другое используемое);</span><span class="sxs-lookup"><span data-stu-id="ed6d0-161">Used Others</span></span>
- <span data-ttu-id="ed6d0-162">Report Period (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="ed6d0-162">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="ed6d0-163">Пример</span><span class="sxs-lookup"><span data-stu-id="ed6d0-163">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ed6d0-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="ed6d0-164">Request</span></span>

<span data-ttu-id="ed6d0-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ed6d0-165">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ed6d0-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="ed6d0-166">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammerdeviceusageuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getYammerDeviceUsageUserDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ed6d0-167">C#</span><span class="sxs-lookup"><span data-stu-id="ed6d0-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammerdeviceusageuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ed6d0-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ed6d0-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammerdeviceusageuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ed6d0-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ed6d0-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammerdeviceusageuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ed6d0-170">Java</span><span class="sxs-lookup"><span data-stu-id="ed6d0-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getyammerdeviceusageuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ed6d0-171">Ответ</span><span class="sxs-lookup"><span data-stu-id="ed6d0-171">Response</span></span>

<span data-ttu-id="ed6d0-172">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ed6d0-172">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

#### <a name="request"></a><span data-ttu-id="ed6d0-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="ed6d0-173">Request</span></span>

<span data-ttu-id="ed6d0-174">При вызове с `date` параметром область применения отчета определяется на заданную дату.</span><span class="sxs-lookup"><span data-stu-id="ed6d0-174">If called with the `date` parameter, the report is scoped to usage on the given date.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammerdeviceusageuserdetail_date"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerDeviceUsageUserDetail(date='2018-03-05')
```

#### <a name="response"></a><span data-ttu-id="ed6d0-175">Ответ</span><span class="sxs-lookup"><span data-stu-id="ed6d0-175">Response</span></span>

<span data-ttu-id="ed6d0-176">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ed6d0-176">The following is an example of the response.</span></span>

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

<span data-ttu-id="ed6d0-177">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="ed6d0-177">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
