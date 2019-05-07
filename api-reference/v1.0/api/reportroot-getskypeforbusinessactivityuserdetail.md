---
title: 'reportRoot: getSkypeForBusinessActivityUserDetail'
description: Получите сведения о действиях пользователей в Skype для бизнеса.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: c9d166d2fb3ebd02c237864c6e7950bfd09ccc2f
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33604214"
---
# <a name="reportroot-getskypeforbusinessactivityuserdetail"></a><span data-ttu-id="c862e-103">reportRoot: getSkypeForBusinessActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="c862e-103">reportRoot: getSkypeForBusinessActivityUserDetail</span></span>

<span data-ttu-id="c862e-104">Получите сведения о действиях пользователей в Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="c862e-104">Get details about Skype for Business activity by user.</span></span>

> <span data-ttu-id="c862e-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span><span class="sxs-lookup"><span data-stu-id="c862e-105">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="c862e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c862e-106">Permissions</span></span>

<span data-ttu-id="c862e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c862e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c862e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c862e-109">Permission type</span></span>                        | <span data-ttu-id="c862e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c862e-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="c862e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c862e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c862e-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c862e-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="c862e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c862e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c862e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c862e-114">Not supported.</span></span>                           |
| <span data-ttu-id="c862e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c862e-115">Application</span></span>                            | <span data-ttu-id="c862e-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c862e-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="c862e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c862e-117">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getSkypeForBusinessActivityUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="c862e-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="c862e-118">Function parameters</span></span>

<span data-ttu-id="c862e-119">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="c862e-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="c862e-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="c862e-120">Parameter</span></span> | <span data-ttu-id="c862e-121">Тип</span><span class="sxs-lookup"><span data-stu-id="c862e-121">Type</span></span>   | <span data-ttu-id="c862e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c862e-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="c862e-123">period</span><span class="sxs-lookup"><span data-stu-id="c862e-123">period</span></span>    | <span data-ttu-id="c862e-124">string</span><span class="sxs-lookup"><span data-stu-id="c862e-124">string</span></span> | <span data-ttu-id="c862e-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="c862e-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="c862e-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="c862e-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="c862e-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="c862e-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="c862e-128">date</span><span class="sxs-lookup"><span data-stu-id="c862e-128">date</span></span>      | <span data-ttu-id="c862e-129">Date</span><span class="sxs-lookup"><span data-stu-id="c862e-129">Date</span></span>   | <span data-ttu-id="c862e-130">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="c862e-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="c862e-131">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="c862e-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="c862e-132">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="c862e-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="c862e-133">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="c862e-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c862e-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c862e-134">Request headers</span></span>

| <span data-ttu-id="c862e-135">Имя</span><span class="sxs-lookup"><span data-stu-id="c862e-135">Name</span></span>          | <span data-ttu-id="c862e-136">Описание</span><span class="sxs-lookup"><span data-stu-id="c862e-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="c862e-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c862e-137">Authorization</span></span> | <span data-ttu-id="c862e-p104">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c862e-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="c862e-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="c862e-140">If-None-Match</span></span> | <span data-ttu-id="c862e-141">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="c862e-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="c862e-142">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="c862e-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="c862e-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="c862e-143">Response</span></span>

<span data-ttu-id="c862e-144">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="c862e-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="c862e-145">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="c862e-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="c862e-146">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="c862e-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="c862e-147">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="c862e-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="c862e-148">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="c862e-148">Report Refresh Date</span></span>
- <span data-ttu-id="c862e-149">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="c862e-149">User Principal Name</span></span>
- <span data-ttu-id="c862e-150">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="c862e-150">Is Deleted</span></span>
- <span data-ttu-id="c862e-151">"Deleted Date" (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="c862e-151">Deleted Date</span></span>
- <span data-ttu-id="c862e-152">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="c862e-152">Last Activity Date</span></span>
- <span data-ttu-id="c862e-153">Total Peer-to-peer Session Count (общее количество одноранговых сеансов)</span><span class="sxs-lookup"><span data-stu-id="c862e-153">Total Peer-to-peer Session Count</span></span>
- <span data-ttu-id="c862e-154">Total Organized Conference Count (общее количество организованных конференций)</span><span class="sxs-lookup"><span data-stu-id="c862e-154">Total Organized Conference Count</span></span>
- <span data-ttu-id="c862e-155">Total Participated Conference Count (общее количество конференций с участием пользователя)</span><span class="sxs-lookup"><span data-stu-id="c862e-155">Total Participated Conference Count</span></span>
- <span data-ttu-id="c862e-156">Peer-to-peer Last Activity Date (дата последнего действия в одноранговом сеансе)</span><span class="sxs-lookup"><span data-stu-id="c862e-156">Peer-to-peer Last Activity Date</span></span>
- <span data-ttu-id="c862e-157">Organized Conference Last Activity Date (дата последнего действия в организованной конференции)</span><span class="sxs-lookup"><span data-stu-id="c862e-157">Organized Conference Last Activity Date</span></span>
- <span data-ttu-id="c862e-158">Participated Conference Last Activity Date (дата последнего действия в конференции с участием пользователя)</span><span class="sxs-lookup"><span data-stu-id="c862e-158">Participated Conference Last Activity Date</span></span>
- <span data-ttu-id="c862e-159">Peer-to-peer IM Count (количество одноранговых сеансов с обменом мгновенными сообщениями)</span><span class="sxs-lookup"><span data-stu-id="c862e-159">Peer-to-peer IM Count</span></span>
- <span data-ttu-id="c862e-160">Peer-to-peer Audio Count (количество одноранговых сеансов с аудиосвязью)</span><span class="sxs-lookup"><span data-stu-id="c862e-160">Peer-to-peer Audio Count</span></span>
- <span data-ttu-id="c862e-161">Peer-to-peer Audio Minutes (продолжительность одноранговых сеансов с аудиосвязью, в минутах)</span><span class="sxs-lookup"><span data-stu-id="c862e-161">Peer-to-peer Audio Minutes</span></span>
- <span data-ttu-id="c862e-162">Peer-to-peer Video Count (количество одноранговых сеансов с видеосвязью)</span><span class="sxs-lookup"><span data-stu-id="c862e-162">Peer-to-peer Video Count</span></span>
- <span data-ttu-id="c862e-163">Peer-to-peer Video Minutes (продолжительность одноранговых сеансов с видеосвязью, в минутах)</span><span class="sxs-lookup"><span data-stu-id="c862e-163">Peer-to-peer Video Minutes</span></span>
- <span data-ttu-id="c862e-164">Peer-to-peer App Sharing Count (количество одноранговых сеансов с общим доступом к приложениям)</span><span class="sxs-lookup"><span data-stu-id="c862e-164">Peer-to-peer App Sharing Count</span></span>
- <span data-ttu-id="c862e-165">Peer-to-peer File Transfer Count (количество одноранговых сеансов с передачей файлов)</span><span class="sxs-lookup"><span data-stu-id="c862e-165">Peer-to-peer File Transfer Count</span></span>
- <span data-ttu-id="c862e-166">Organized Conference IM Count (количество организованных конференций с обменом мгновенными сообщениями)</span><span class="sxs-lookup"><span data-stu-id="c862e-166">Organized Conference IM Count</span></span>
- <span data-ttu-id="c862e-167">Organized Conference Audio/Video Count (количество организованных конференций с аудио- и видеосвязью)</span><span class="sxs-lookup"><span data-stu-id="c862e-167">Organized Conference Audio/Video Count</span></span>
- <span data-ttu-id="c862e-168">Organized Conference Audio/Video Minutes (продолжительность организованных конференций с аудио- и видеосвязью, в минутах)</span><span class="sxs-lookup"><span data-stu-id="c862e-168">Organized Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="c862e-169">Organized Conference App Sharing Count (количество организованных конференций с общим доступом к приложениям)</span><span class="sxs-lookup"><span data-stu-id="c862e-169">Organized Conference App Sharing Count</span></span>
- <span data-ttu-id="c862e-170">Organized Conference Web Count (количество организованных веб-конференций)</span><span class="sxs-lookup"><span data-stu-id="c862e-170">Organized Conference Web Count</span></span>
- <span data-ttu-id="c862e-171">Organized Conference Dial-in/out 3rd Party Count (количество организованных конференций с телефонным подключением или с присоединением обратным звонком, сторонняя служба)</span><span class="sxs-lookup"><span data-stu-id="c862e-171">Organized Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="c862e-172">Organized Conference Dial-in/out Microsoft Count (количество организованных конференций с телефонным подключением или с присоединением обратным звонком, Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c862e-172">Organized Conference Dial-in/out Microsoft Count</span></span>
- <span data-ttu-id="c862e-173">Organized Conference Dial-in Microsoft Minutes (продолжительность организованных конференций с телефонным подключением, Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c862e-173">Organized Conference Dial-in Microsoft Minutes</span></span>
- <span data-ttu-id="c862e-174">Organized Conference Dial-out Microsoft Minutes (продолжительность организованных конференций с присоединением обратным звонком, Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c862e-174">Organized Conference Dial-out Microsoft Minutes</span></span>
- <span data-ttu-id="c862e-175">Paricipated Conference IM Count (количество конференций с участием пользователя и обменом мгновенными сообщениями)</span><span class="sxs-lookup"><span data-stu-id="c862e-175">Paricipated Conference IM Count</span></span>
- <span data-ttu-id="c862e-176">Participated Conference Audio/Video Count (количество конференций с участием пользователя и аудио- и видеосвязью)</span><span class="sxs-lookup"><span data-stu-id="c862e-176">Participated Conference Audio/Video Count</span></span>
- <span data-ttu-id="c862e-177">Participated Conference Audio/Video Minutes (продолжительность конференций с участием пользователя и аудио- и видеосвязью)</span><span class="sxs-lookup"><span data-stu-id="c862e-177">Participated Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="c862e-178">Participated Conference App Sharing Count (количество конференций с участием пользователя и общим доступом к приложениям)</span><span class="sxs-lookup"><span data-stu-id="c862e-178">Participated Conference App Sharing Count</span></span>
- <span data-ttu-id="c862e-179">Participated Conference Web Count (количество веб-конференций с участием пользователя)</span><span class="sxs-lookup"><span data-stu-id="c862e-179">Participated Conference Web Count</span></span>
- <span data-ttu-id="c862e-180">Participated Conference Dial-in/out 3rd Party Count (количество конференций с участием пользователя и телефонным подключением или с присоединением обратным звонком, сторонняя служба)</span><span class="sxs-lookup"><span data-stu-id="c862e-180">Participated Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="c862e-181">Assigned Products (назначенные продукты)</span><span class="sxs-lookup"><span data-stu-id="c862e-181">Assigned Products</span></span>
- <span data-ttu-id="c862e-182">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="c862e-182">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="c862e-183">Пример</span><span class="sxs-lookup"><span data-stu-id="c862e-183">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c862e-184">Запрос</span><span class="sxs-lookup"><span data-stu-id="c862e-184">Request</span></span>

<span data-ttu-id="c862e-185">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c862e-185">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessActivityUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="c862e-186">Ответ</span><span class="sxs-lookup"><span data-stu-id="c862e-186">Response</span></span>

<span data-ttu-id="c862e-187">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c862e-187">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="c862e-188">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="c862e-188">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c862e-189">Языках</span><span class="sxs-lookup"><span data-stu-id="c862e-189">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessactivityuserdetail-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c862e-190">Язык</span><span class="sxs-lookup"><span data-stu-id="c862e-190">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessactivityuserdetail-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="c862e-191">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="c862e-191">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Total Peer-to-peer Session Count,Total Organized Conference Count,Total Participated Conference Count,Peer-to-peer Last Activity Date,Organized Conference Last Activity Date,Participated Conference Last Activity Date,Peer-to-peer IM Count,Peer-to-peer Audio Count,Peer-to-peer Audio Minutes,Peer-to-peer Video Count,Peer-to-peer Video Minutes,Peer-to-peer App Sharing Count,Peer-to-peer File Transfer Count,Organized Conference IM Count,Organized Conference Audio/Video Count,Organized Conference Audio/Video Minutes,Organized Conference App Sharing Count,Organized Conference Web Count,Organized Conference Dial-in/out 3rd Party Count,Organized Conference Dial-in/out Microsoft Count,Organized Conference Dial-in Microsoft Minutes,Organized Conference Dial-out Microsoft Minutes,Paricipated Conference IM Count,Participated Conference Audio/Video Count,Participated Conference Audio/Video Minutes,Participated Conference App Sharing Count,Participated Conference Web Count,Participated Conference Dial-in/out 3rd Party Count,Assigned Products,Report Period
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
    "Error: /api-reference/v1.0/api/reportroot-getskypeforbusinessactivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getskypeforbusinessactivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
