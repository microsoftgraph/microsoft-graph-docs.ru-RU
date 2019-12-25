---
title: 'reportRoot: getSkypeForBusinessActivityUserDetail'
description: Получите сведения о действиях пользователей в Skype для бизнеса.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 8ca56904638598085cb345acf5d93babc4226347
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865316"
---
# <a name="reportroot-getskypeforbusinessactivityuserdetail"></a><span data-ttu-id="064fa-103">reportRoot: getSkypeForBusinessActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="064fa-103">reportRoot: getSkypeForBusinessActivityUserDetail</span></span>

<span data-ttu-id="064fa-104">Получите сведения о действиях пользователей в Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="064fa-104">Get details about Skype for Business activity by user.</span></span>

> <span data-ttu-id="064fa-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span><span class="sxs-lookup"><span data-stu-id="064fa-105">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="064fa-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="064fa-106">Permissions</span></span>

<span data-ttu-id="064fa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="064fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="064fa-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="064fa-109">Permission type</span></span>                        | <span data-ttu-id="064fa-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="064fa-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="064fa-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="064fa-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="064fa-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="064fa-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="064fa-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="064fa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="064fa-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="064fa-114">Not supported.</span></span>                           |
| <span data-ttu-id="064fa-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="064fa-115">Application</span></span>                            | <span data-ttu-id="064fa-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="064fa-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="064fa-117">**Примечание**. для делегированных разрешений, чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя, администратору клиента необходимо назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="064fa-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="064fa-118">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Office 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="064fa-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="064fa-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="064fa-119">HTTP request</span></span>


<!-- { "blockType": "samples" } --> 

```http
GET /reports/getSkypeForBusinessActivityUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="064fa-120">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="064fa-120">Function parameters</span></span>

<span data-ttu-id="064fa-121">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="064fa-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="064fa-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="064fa-122">Parameter</span></span> | <span data-ttu-id="064fa-123">Тип</span><span class="sxs-lookup"><span data-stu-id="064fa-123">Type</span></span>   | <span data-ttu-id="064fa-124">Описание</span><span class="sxs-lookup"><span data-stu-id="064fa-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="064fa-125">period</span><span class="sxs-lookup"><span data-stu-id="064fa-125">period</span></span>    | <span data-ttu-id="064fa-126">string</span><span class="sxs-lookup"><span data-stu-id="064fa-126">string</span></span> | <span data-ttu-id="064fa-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="064fa-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="064fa-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="064fa-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="064fa-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="064fa-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="064fa-130">date</span><span class="sxs-lookup"><span data-stu-id="064fa-130">date</span></span>      | <span data-ttu-id="064fa-131">Date</span><span class="sxs-lookup"><span data-stu-id="064fa-131">Date</span></span>   | <span data-ttu-id="064fa-132">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="064fa-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="064fa-133">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="064fa-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="064fa-134">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="064fa-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="064fa-135">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="064fa-135">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="064fa-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="064fa-136">Request headers</span></span>

| <span data-ttu-id="064fa-137">Имя</span><span class="sxs-lookup"><span data-stu-id="064fa-137">Name</span></span>          | <span data-ttu-id="064fa-138">Описание</span><span class="sxs-lookup"><span data-stu-id="064fa-138">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="064fa-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="064fa-139">Authorization</span></span> | <span data-ttu-id="064fa-p105">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="064fa-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="064fa-142">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="064fa-142">If-None-Match</span></span> | <span data-ttu-id="064fa-143">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="064fa-143">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="064fa-144">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="064fa-144">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="064fa-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="064fa-145">Response</span></span>

<span data-ttu-id="064fa-146">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="064fa-146">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="064fa-147">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="064fa-147">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="064fa-148">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="064fa-148">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="064fa-149">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="064fa-149">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="064fa-150">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="064fa-150">Report Refresh Date</span></span>
- <span data-ttu-id="064fa-151">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="064fa-151">User Principal Name</span></span>
- <span data-ttu-id="064fa-152">Is Deleted (Удален);</span><span class="sxs-lookup"><span data-stu-id="064fa-152">Is Deleted</span></span>
- <span data-ttu-id="064fa-153">"Deleted Date" (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="064fa-153">Deleted Date</span></span>
- <span data-ttu-id="064fa-154">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="064fa-154">Last Activity Date</span></span>
- <span data-ttu-id="064fa-155">Total Peer-to-peer Session Count (общее количество одноранговых сеансов)</span><span class="sxs-lookup"><span data-stu-id="064fa-155">Total Peer-to-peer Session Count</span></span>
- <span data-ttu-id="064fa-156">Total Organized Conference Count (общее количество организованных конференций)</span><span class="sxs-lookup"><span data-stu-id="064fa-156">Total Organized Conference Count</span></span>
- <span data-ttu-id="064fa-157">Total Participated Conference Count (общее количество конференций с участием пользователя)</span><span class="sxs-lookup"><span data-stu-id="064fa-157">Total Participated Conference Count</span></span>
- <span data-ttu-id="064fa-158">Peer-to-peer Last Activity Date (дата последнего действия в одноранговом сеансе)</span><span class="sxs-lookup"><span data-stu-id="064fa-158">Peer-to-peer Last Activity Date</span></span>
- <span data-ttu-id="064fa-159">Organized Conference Last Activity Date (дата последнего действия в организованной конференции)</span><span class="sxs-lookup"><span data-stu-id="064fa-159">Organized Conference Last Activity Date</span></span>
- <span data-ttu-id="064fa-160">Participated Conference Last Activity Date (дата последнего действия в конференции с участием пользователя)</span><span class="sxs-lookup"><span data-stu-id="064fa-160">Participated Conference Last Activity Date</span></span>
- <span data-ttu-id="064fa-161">Peer-to-peer IM Count (количество одноранговых сеансов с обменом мгновенными сообщениями)</span><span class="sxs-lookup"><span data-stu-id="064fa-161">Peer-to-peer IM Count</span></span>
- <span data-ttu-id="064fa-162">Peer-to-peer Audio Count (количество одноранговых сеансов с аудиосвязью)</span><span class="sxs-lookup"><span data-stu-id="064fa-162">Peer-to-peer Audio Count</span></span>
- <span data-ttu-id="064fa-163">Peer-to-peer Audio Minutes (продолжительность одноранговых сеансов с аудиосвязью, в минутах)</span><span class="sxs-lookup"><span data-stu-id="064fa-163">Peer-to-peer Audio Minutes</span></span>
- <span data-ttu-id="064fa-164">Peer-to-peer Video Count (количество одноранговых сеансов с видеосвязью)</span><span class="sxs-lookup"><span data-stu-id="064fa-164">Peer-to-peer Video Count</span></span>
- <span data-ttu-id="064fa-165">Peer-to-peer Video Minutes (продолжительность одноранговых сеансов с видеосвязью, в минутах)</span><span class="sxs-lookup"><span data-stu-id="064fa-165">Peer-to-peer Video Minutes</span></span>
- <span data-ttu-id="064fa-166">Peer-to-peer App Sharing Count (количество одноранговых сеансов с общим доступом к приложениям)</span><span class="sxs-lookup"><span data-stu-id="064fa-166">Peer-to-peer App Sharing Count</span></span>
- <span data-ttu-id="064fa-167">Peer-to-peer File Transfer Count (количество одноранговых сеансов с передачей файлов)</span><span class="sxs-lookup"><span data-stu-id="064fa-167">Peer-to-peer File Transfer Count</span></span>
- <span data-ttu-id="064fa-168">Organized Conference IM Count (количество организованных конференций с обменом мгновенными сообщениями)</span><span class="sxs-lookup"><span data-stu-id="064fa-168">Organized Conference IM Count</span></span>
- <span data-ttu-id="064fa-169">Organized Conference Audio/Video Count (количество организованных конференций с аудио- и видеосвязью)</span><span class="sxs-lookup"><span data-stu-id="064fa-169">Organized Conference Audio/Video Count</span></span>
- <span data-ttu-id="064fa-170">Organized Conference Audio/Video Minutes (продолжительность организованных конференций с аудио- и видеосвязью, в минутах)</span><span class="sxs-lookup"><span data-stu-id="064fa-170">Organized Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="064fa-171">Organized Conference App Sharing Count (количество организованных конференций с общим доступом к приложениям)</span><span class="sxs-lookup"><span data-stu-id="064fa-171">Organized Conference App Sharing Count</span></span>
- <span data-ttu-id="064fa-172">Organized Conference Web Count (количество организованных веб-конференций)</span><span class="sxs-lookup"><span data-stu-id="064fa-172">Organized Conference Web Count</span></span>
- <span data-ttu-id="064fa-173">Organized Conference Dial-in/out 3rd Party Count (количество организованных конференций с телефонным подключением или с присоединением обратным звонком, сторонняя служба)</span><span class="sxs-lookup"><span data-stu-id="064fa-173">Organized Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="064fa-174">Organized Conference Dial-in/out Microsoft Count (количество организованных конференций с телефонным подключением или с присоединением обратным звонком, Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="064fa-174">Organized Conference Dial-in/out Microsoft Count</span></span>
- <span data-ttu-id="064fa-175">Organized Conference Dial-in Microsoft Minutes (продолжительность организованных конференций с телефонным подключением, Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="064fa-175">Organized Conference Dial-in Microsoft Minutes</span></span>
- <span data-ttu-id="064fa-176">Organized Conference Dial-out Microsoft Minutes (продолжительность организованных конференций с присоединением обратным звонком, Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="064fa-176">Organized Conference Dial-out Microsoft Minutes</span></span>
- <span data-ttu-id="064fa-177">Paricipated Conference IM Count (количество конференций с участием пользователя и обменом мгновенными сообщениями)</span><span class="sxs-lookup"><span data-stu-id="064fa-177">Paricipated Conference IM Count</span></span>
- <span data-ttu-id="064fa-178">Participated Conference Audio/Video Count (количество конференций с участием пользователя и аудио- и видеосвязью)</span><span class="sxs-lookup"><span data-stu-id="064fa-178">Participated Conference Audio/Video Count</span></span>
- <span data-ttu-id="064fa-179">Participated Conference Audio/Video Minutes (продолжительность конференций с участием пользователя и аудио- и видеосвязью)</span><span class="sxs-lookup"><span data-stu-id="064fa-179">Participated Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="064fa-180">Participated Conference App Sharing Count (количество конференций с участием пользователя и общим доступом к приложениям)</span><span class="sxs-lookup"><span data-stu-id="064fa-180">Participated Conference App Sharing Count</span></span>
- <span data-ttu-id="064fa-181">Participated Conference Web Count (количество веб-конференций с участием пользователя)</span><span class="sxs-lookup"><span data-stu-id="064fa-181">Participated Conference Web Count</span></span>
- <span data-ttu-id="064fa-182">Participated Conference Dial-in/out 3rd Party Count (количество конференций с участием пользователя и телефонным подключением или с присоединением обратным звонком, сторонняя служба)</span><span class="sxs-lookup"><span data-stu-id="064fa-182">Participated Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="064fa-183">Assigned Products (назначенные продукты)</span><span class="sxs-lookup"><span data-stu-id="064fa-183">Assigned Products</span></span>
- <span data-ttu-id="064fa-184">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="064fa-184">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="064fa-185">Пример</span><span class="sxs-lookup"><span data-stu-id="064fa-185">Example</span></span>

#### <a name="request"></a><span data-ttu-id="064fa-186">Запрос</span><span class="sxs-lookup"><span data-stu-id="064fa-186">Request</span></span>

<span data-ttu-id="064fa-187">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="064fa-187">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="064fa-188">HTTP</span><span class="sxs-lookup"><span data-stu-id="064fa-188">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessactivityuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessActivityUserDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="064fa-189">C#</span><span class="sxs-lookup"><span data-stu-id="064fa-189">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessactivityuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="064fa-190">JavaScript</span><span class="sxs-lookup"><span data-stu-id="064fa-190">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessactivityuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="064fa-191">Objective-C</span><span class="sxs-lookup"><span data-stu-id="064fa-191">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessactivityuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="064fa-192">Java</span><span class="sxs-lookup"><span data-stu-id="064fa-192">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getskypeforbusinessactivityuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="064fa-193">Ответ</span><span class="sxs-lookup"><span data-stu-id="064fa-193">Response</span></span>

<span data-ttu-id="064fa-194">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="064fa-194">The following is an example of the response.</span></span>

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

<span data-ttu-id="064fa-195">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="064fa-195">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
  ]
}-->
