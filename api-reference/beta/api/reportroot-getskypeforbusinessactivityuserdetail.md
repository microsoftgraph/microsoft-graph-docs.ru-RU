---
title: 'reportRoot: getSkypeForBusinessActivityUserDetail'
description: Получите сведения о действиях пользователей в Skype для бизнеса.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 8ac4f67c744a14b3240cdfcf365dc05b82ae2f4d
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36725049"
---
# <a name="reportroot-getskypeforbusinessactivityuserdetail"></a><span data-ttu-id="c4eff-103">reportRoot: getSkypeForBusinessActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="c4eff-103">reportRoot: getSkypeForBusinessActivityUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4eff-104">Получите сведения о действиях пользователей в Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="c4eff-104">Get details about Skype for Business activity by user.</span></span>

> <span data-ttu-id="c4eff-105">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span><span class="sxs-lookup"><span data-stu-id="c4eff-105">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="c4eff-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c4eff-106">Permissions</span></span>

<span data-ttu-id="c4eff-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4eff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c4eff-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c4eff-109">Permission type</span></span>                        | <span data-ttu-id="c4eff-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c4eff-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="c4eff-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c4eff-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c4eff-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c4eff-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="c4eff-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c4eff-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4eff-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4eff-114">Not supported.</span></span>                           |
| <span data-ttu-id="c4eff-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c4eff-115">Application</span></span>                            | <span data-ttu-id="c4eff-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c4eff-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="c4eff-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c4eff-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessActivityUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="c4eff-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="c4eff-118">Function parameters</span></span>

<span data-ttu-id="c4eff-119">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="c4eff-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="c4eff-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="c4eff-120">Parameter</span></span> | <span data-ttu-id="c4eff-121">Тип</span><span class="sxs-lookup"><span data-stu-id="c4eff-121">Type</span></span>   | <span data-ttu-id="c4eff-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c4eff-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="c4eff-123">period</span><span class="sxs-lookup"><span data-stu-id="c4eff-123">period</span></span>    | <span data-ttu-id="c4eff-124">string</span><span class="sxs-lookup"><span data-stu-id="c4eff-124">string</span></span> | <span data-ttu-id="c4eff-125">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="c4eff-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="c4eff-126">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="c4eff-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="c4eff-127">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="c4eff-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="c4eff-128">date</span><span class="sxs-lookup"><span data-stu-id="c4eff-128">date</span></span>      | <span data-ttu-id="c4eff-129">Date</span><span class="sxs-lookup"><span data-stu-id="c4eff-129">Date</span></span>   | <span data-ttu-id="c4eff-130">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="c4eff-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="c4eff-131">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="c4eff-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="c4eff-132">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="c4eff-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="c4eff-133">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="c4eff-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="c4eff-134">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c4eff-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="c4eff-135">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="c4eff-135">The default output type is text/csv.</span></span> <span data-ttu-id="c4eff-136">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="c4eff-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c4eff-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c4eff-137">Request headers</span></span>

| <span data-ttu-id="c4eff-138">Имя</span><span class="sxs-lookup"><span data-stu-id="c4eff-138">Name</span></span>          | <span data-ttu-id="c4eff-139">Описание</span><span class="sxs-lookup"><span data-stu-id="c4eff-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="c4eff-140">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c4eff-140">Authorization</span></span> | <span data-ttu-id="c4eff-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c4eff-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="c4eff-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4eff-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="c4eff-144">CSV</span><span class="sxs-lookup"><span data-stu-id="c4eff-144">CSV</span></span>

<span data-ttu-id="c4eff-145">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="c4eff-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="c4eff-146">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="c4eff-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="c4eff-147">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="c4eff-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="c4eff-148">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="c4eff-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="c4eff-149">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="c4eff-149">Report Refresh Date</span></span>
- <span data-ttu-id="c4eff-150">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="c4eff-150">User Principal Name</span></span>
- <span data-ttu-id="c4eff-151">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="c4eff-151">Is Deleted</span></span>
- <span data-ttu-id="c4eff-152">"Deleted Date" (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="c4eff-152">Deleted Date</span></span>
- <span data-ttu-id="c4eff-153">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="c4eff-153">Last Activity Date</span></span>
- <span data-ttu-id="c4eff-154">Total Peer-to-peer Session Count (общее количество одноранговых сеансов)</span><span class="sxs-lookup"><span data-stu-id="c4eff-154">Total Peer-to-peer Session Count</span></span>
- <span data-ttu-id="c4eff-155">Total Organized Conference Count (общее количество организованных конференций)</span><span class="sxs-lookup"><span data-stu-id="c4eff-155">Total Organized Conference Count</span></span>
- <span data-ttu-id="c4eff-156">Total Participated Conference Count (общее количество конференций с участием пользователя)</span><span class="sxs-lookup"><span data-stu-id="c4eff-156">Total Participated Conference Count</span></span>
- <span data-ttu-id="c4eff-157">Peer-to-peer Last Activity Date (дата последнего действия в одноранговом сеансе)</span><span class="sxs-lookup"><span data-stu-id="c4eff-157">Peer-to-peer Last Activity Date</span></span>
- <span data-ttu-id="c4eff-158">Organized Conference Last Activity Date (дата последнего действия в организованной конференции)</span><span class="sxs-lookup"><span data-stu-id="c4eff-158">Organized Conference Last Activity Date</span></span>
- <span data-ttu-id="c4eff-159">Participated Conference Last Activity Date (дата последнего действия в конференции с участием пользователя)</span><span class="sxs-lookup"><span data-stu-id="c4eff-159">Participated Conference Last Activity Date</span></span>
- <span data-ttu-id="c4eff-160">Peer-to-peer IM Count (количество одноранговых сеансов с обменом мгновенными сообщениями)</span><span class="sxs-lookup"><span data-stu-id="c4eff-160">Peer-to-peer IM Count</span></span>
- <span data-ttu-id="c4eff-161">Peer-to-peer Audio Count (количество одноранговых сеансов с аудиосвязью)</span><span class="sxs-lookup"><span data-stu-id="c4eff-161">Peer-to-peer Audio Count</span></span>
- <span data-ttu-id="c4eff-162">Peer-to-peer Audio Minutes (продолжительность одноранговых сеансов с аудиосвязью, в минутах)</span><span class="sxs-lookup"><span data-stu-id="c4eff-162">Peer-to-peer Audio Minutes</span></span>
- <span data-ttu-id="c4eff-163">Peer-to-peer Video Count (количество одноранговых сеансов с видеосвязью)</span><span class="sxs-lookup"><span data-stu-id="c4eff-163">Peer-to-peer Video Count</span></span>
- <span data-ttu-id="c4eff-164">Peer-to-peer Video Minutes (продолжительность одноранговых сеансов с видеосвязью, в минутах)</span><span class="sxs-lookup"><span data-stu-id="c4eff-164">Peer-to-peer Video Minutes</span></span>
- <span data-ttu-id="c4eff-165">Peer-to-peer App Sharing Count (количество одноранговых сеансов с общим доступом к приложениям)</span><span class="sxs-lookup"><span data-stu-id="c4eff-165">Peer-to-peer App Sharing Count</span></span>
- <span data-ttu-id="c4eff-166">Peer-to-peer File Transfer Count (количество одноранговых сеансов с передачей файлов)</span><span class="sxs-lookup"><span data-stu-id="c4eff-166">Peer-to-peer File Transfer Count</span></span>
- <span data-ttu-id="c4eff-167">Organized Conference IM Count (количество организованных конференций с обменом мгновенными сообщениями)</span><span class="sxs-lookup"><span data-stu-id="c4eff-167">Organized Conference IM Count</span></span>
- <span data-ttu-id="c4eff-168">Organized Conference Audio/Video Count (количество организованных конференций с аудио- и видеосвязью)</span><span class="sxs-lookup"><span data-stu-id="c4eff-168">Organized Conference Audio/Video Count</span></span>
- <span data-ttu-id="c4eff-169">Organized Conference Audio/Video Minutes (продолжительность организованных конференций с аудио- и видеосвязью, в минутах)</span><span class="sxs-lookup"><span data-stu-id="c4eff-169">Organized Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="c4eff-170">Organized Conference App Sharing Count (количество организованных конференций с общим доступом к приложениям)</span><span class="sxs-lookup"><span data-stu-id="c4eff-170">Organized Conference App Sharing Count</span></span>
- <span data-ttu-id="c4eff-171">Organized Conference Web Count (количество организованных веб-конференций)</span><span class="sxs-lookup"><span data-stu-id="c4eff-171">Organized Conference Web Count</span></span>
- <span data-ttu-id="c4eff-172">Organized Conference Dial-in/out 3rd Party Count (количество организованных конференций с телефонным подключением или с присоединением обратным звонком, сторонняя служба)</span><span class="sxs-lookup"><span data-stu-id="c4eff-172">Organized Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="c4eff-173">Organized Conference Dial-in/out Microsoft Count (количество организованных конференций с телефонным подключением или с присоединением обратным звонком, Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c4eff-173">Organized Conference Dial-in/out Microsoft Count</span></span>
- <span data-ttu-id="c4eff-174">Organized Conference Dial-in Microsoft Minutes (продолжительность организованных конференций с телефонным подключением, Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c4eff-174">Organized Conference Dial-in Microsoft Minutes</span></span>
- <span data-ttu-id="c4eff-175">Organized Conference Dial-out Microsoft Minutes (продолжительность организованных конференций с присоединением обратным звонком, Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c4eff-175">Organized Conference Dial-out Microsoft Minutes</span></span>
- <span data-ttu-id="c4eff-176">Количество мгновенных сообщений для конференций с участием</span><span class="sxs-lookup"><span data-stu-id="c4eff-176">Participated Conference IM Count</span></span>
- <span data-ttu-id="c4eff-177">Participated Conference Audio/Video Count (количество конференций с участием пользователя и аудио- и видеосвязью)</span><span class="sxs-lookup"><span data-stu-id="c4eff-177">Participated Conference Audio/Video Count</span></span>
- <span data-ttu-id="c4eff-178">Participated Conference Audio/Video Minutes (продолжительность конференций с участием пользователя и аудио- и видеосвязью)</span><span class="sxs-lookup"><span data-stu-id="c4eff-178">Participated Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="c4eff-179">Participated Conference App Sharing Count (количество конференций с участием пользователя и общим доступом к приложениям)</span><span class="sxs-lookup"><span data-stu-id="c4eff-179">Participated Conference App Sharing Count</span></span>
- <span data-ttu-id="c4eff-180">Participated Conference Web Count (количество веб-конференций с участием пользователя)</span><span class="sxs-lookup"><span data-stu-id="c4eff-180">Participated Conference Web Count</span></span>
- <span data-ttu-id="c4eff-181">Participated Conference Dial-in/out 3rd Party Count (количество конференций с участием пользователя и телефонным подключением или с присоединением обратным звонком, сторонняя служба)</span><span class="sxs-lookup"><span data-stu-id="c4eff-181">Participated Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="c4eff-182">Assigned Products (назначенные продукты)</span><span class="sxs-lookup"><span data-stu-id="c4eff-182">Assigned Products</span></span>
- <span data-ttu-id="c4eff-183">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="c4eff-183">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="c4eff-184">JSON</span><span class="sxs-lookup"><span data-stu-id="c4eff-184">JSON</span></span>

<span data-ttu-id="c4eff-185">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[скипефорбусинессактивитюсердетаил](../resources/skypeforbusinessactivityuserdetail.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c4eff-185">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessActivityUserDetail](../resources/skypeforbusinessactivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="c4eff-186">Размер страницы по умолчанию для этого запроса составляет 200 элементов.</span><span class="sxs-lookup"><span data-stu-id="c4eff-186">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="c4eff-187">Пример</span><span class="sxs-lookup"><span data-stu-id="c4eff-187">Example</span></span>

### <a name="csv"></a><span data-ttu-id="c4eff-188">CSV</span><span class="sxs-lookup"><span data-stu-id="c4eff-188">CSV</span></span>

<span data-ttu-id="c4eff-189">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="c4eff-189">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="c4eff-190">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4eff-190">Request</span></span>

<span data-ttu-id="c4eff-191">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c4eff-191">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c4eff-192">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4eff-192">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivityuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityUserDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c4eff-193">C#</span><span class="sxs-lookup"><span data-stu-id="c4eff-193">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessactivityuserdetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c4eff-194">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4eff-194">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessactivityuserdetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c4eff-195">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c4eff-195">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessactivityuserdetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c4eff-196">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4eff-196">Response</span></span>

<span data-ttu-id="c4eff-197">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c4eff-197">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="c4eff-198">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="c4eff-198">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Total Peer-to-peer Session Count,Total Organized Conference Count,Total Participated Conference Count,Peer-to-peer Last Activity Date,Organized Conference Last Activity Date,Participated Conference Last Activity Date,Peer-to-peer IM Count,Peer-to-peer Audio Count,Peer-to-peer Audio Minutes,Peer-to-peer Video Count,Peer-to-peer Video Minutes,Peer-to-peer App Sharing Count,Peer-to-peer File Transfer Count,Organized Conference IM Count,Organized Conference Audio/Video Count,Organized Conference Audio/Video Minutes,Organized Conference App Sharing Count,Organized Conference Web Count,Organized Conference Dial-in/out 3rd Party Count,Organized Conference Dial-in/out Microsoft Count,Organized Conference Dial-in Microsoft Minutes,Organized Conference Dial-out Microsoft Minutes,Participated Conference IM Count,Participated Conference Audio/Video Count,Participated Conference Audio/Video Minutes,Participated Conference App Sharing Count,Participated Conference Web Count,Participated Conference Dial-in/out 3rd Party Count,Assigned Products,Report Period
```

### <a name="json"></a><span data-ttu-id="c4eff-199">JSON</span><span class="sxs-lookup"><span data-stu-id="c4eff-199">JSON</span></span>

<span data-ttu-id="c4eff-200">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="c4eff-200">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="c4eff-201">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4eff-201">Request</span></span>

<span data-ttu-id="c4eff-202">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c4eff-202">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c4eff-203">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4eff-203">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivityuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityUserDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c4eff-204">C#</span><span class="sxs-lookup"><span data-stu-id="c4eff-204">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessactivityuserdetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c4eff-205">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4eff-205">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessactivityuserdetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c4eff-206">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c4eff-206">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessactivityuserdetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c4eff-207">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4eff-207">Response</span></span>

<span data-ttu-id="c4eff-208">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c4eff-208">The following is an example of the response.</span></span>

> <span data-ttu-id="c4eff-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c4eff-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessActivityUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1419

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessActivityUserDetail)", 
  "value": [
    {
      "totalPeerToPeerSessionCount": 12, 
      "totalOrganizedConferenceCount": 0, 
      "totalParticipatedConferenceCount": 1, 
      "peerToPeerLastActivityDate": "2017-09-01", 
      "organizedConferenceLastActivityDate": null, 
      "participatedConferenceLastActivityDate": "2017-08-31", 
      "peerToPeerIMCount": 12, 
      "peerToPeerAudioCount": 0, 
      "peerToPeerAudioMinutes": 0, 
      "peerToPeerVideoCount": 0, 
      "peerToPeerVideoMinutes": 0, 
      "peerToPeerAppSharingCount": 0, 
      "peerToPeerFileTransferCount": 0, 
      "organizedConferenceIMCount": 0, 
      "organizedConferenceAudioVideoCount": 0, 
      "organizedConferenceAudioVideoMinutes": 0, 
      "organizedConferenceAppSharingCount": 0, 
      "organizedConferenceWebCount": 0, 
      "organizedConferenceDialInOut3rdPartyCount": 0, 
      "organizedConferenceCloudDialInOutMicrosoftCount": 0, 
      "organizedConferenceCloudDialInMicrosoftMinutes": 0, 
      "organizedConferenceCloudDialOutMicrosoftMinutes": 0, 
      "participatedConferenceIMCount": 0, 
      "participatedConferenceAudioVideoCount": 1, 
      "participatedConferenceAudioVideoMinutes": 69, 
      "participatedConferenceAppSharingCount": 0, 
      "participatedConferenceWebCount": 0, 
      "participatedConferenceDialInOut3rdPartyCount": 0, 
      "reportRefreshDate": "2017-09-06", 
      "userPrincipalName": "userPrincipalName-value", 
      "isDeleted": false, 
      "deletedDate": null, 
      "lastActivityDate": "2017-09-01", 
      "assignedProducts": [
        "OFFICE 365 ENTERPRISE E5", 
      ], 
      "reportPeriod": "7"
    }
  ]
}
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
