---
title: 'reportRoot: getSkypeForBusinessActivityUserDetail'
description: Получите сведения о действиях пользователей в Skype для бизнеса.
ms.openlocfilehash: 39113039226b48bcefc2121acda5ff5e554d5cd0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075454"
---
# <a name="reportroot-getskypeforbusinessactivityuserdetail"></a><span data-ttu-id="9f43d-103">reportRoot: getSkypeForBusinessActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="9f43d-103">reportRoot: getSkypeForBusinessActivityUserDetail</span></span>

> <span data-ttu-id="9f43d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9f43d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9f43d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f43d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9f43d-106">Получите сведения о действиях пользователей в Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="9f43d-106">Get details about Skype for Business activity by user.</span></span>

> <span data-ttu-id="9f43d-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span><span class="sxs-lookup"><span data-stu-id="9f43d-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="9f43d-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9f43d-108">Permissions</span></span>

<span data-ttu-id="9f43d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f43d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9f43d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f43d-111">Permission type</span></span>                        | <span data-ttu-id="9f43d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f43d-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="9f43d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f43d-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="9f43d-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9f43d-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="9f43d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f43d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f43d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f43d-116">Not supported.</span></span>                           |
| <span data-ttu-id="9f43d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9f43d-117">Application</span></span>                            | <span data-ttu-id="9f43d-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9f43d-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="9f43d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f43d-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessActivityUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="9f43d-120">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="9f43d-120">Function parameters</span></span>

<span data-ttu-id="9f43d-121">В URL-адресе запроса укажите один из следующих параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="9f43d-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="9f43d-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="9f43d-122">Parameter</span></span> | <span data-ttu-id="9f43d-123">Тип</span><span class="sxs-lookup"><span data-stu-id="9f43d-123">Type</span></span>   | <span data-ttu-id="9f43d-124">Описание</span><span class="sxs-lookup"><span data-stu-id="9f43d-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="9f43d-125">period</span><span class="sxs-lookup"><span data-stu-id="9f43d-125">period</span></span>    | <span data-ttu-id="9f43d-126">строка</span><span class="sxs-lookup"><span data-stu-id="9f43d-126">string</span></span> | <span data-ttu-id="9f43d-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="9f43d-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="9f43d-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="9f43d-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="9f43d-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="9f43d-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="9f43d-130">date</span><span class="sxs-lookup"><span data-stu-id="9f43d-130">date</span></span>      | <span data-ttu-id="9f43d-131">Date</span><span class="sxs-lookup"><span data-stu-id="9f43d-131">Date</span></span>   | <span data-ttu-id="9f43d-132">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="9f43d-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="9f43d-133">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="9f43d-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="9f43d-134">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="9f43d-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="9f43d-135">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="9f43d-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="9f43d-136">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9f43d-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="9f43d-137">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="9f43d-137">The default output type is text/csv.</span></span> <span data-ttu-id="9f43d-138">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="9f43d-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9f43d-139">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9f43d-139">Request headers</span></span>

| <span data-ttu-id="9f43d-140">Имя</span><span class="sxs-lookup"><span data-stu-id="9f43d-140">Name</span></span>          | <span data-ttu-id="9f43d-141">Описание</span><span class="sxs-lookup"><span data-stu-id="9f43d-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="9f43d-142">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9f43d-142">Authorization</span></span> | <span data-ttu-id="9f43d-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f43d-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="9f43d-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="9f43d-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="9f43d-146">CSV</span><span class="sxs-lookup"><span data-stu-id="9f43d-146">CSV</span></span>

<span data-ttu-id="9f43d-147">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="9f43d-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="9f43d-148">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="9f43d-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="9f43d-149">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="9f43d-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="9f43d-150">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="9f43d-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="9f43d-151">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="9f43d-151">Report Refresh Date</span></span>
- <span data-ttu-id="9f43d-152">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="9f43d-152">User Principal Name</span></span>
- <span data-ttu-id="9f43d-153">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="9f43d-153">Is Deleted</span></span>
- <span data-ttu-id="9f43d-154">"Deleted Date" (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="9f43d-154">Deleted Date</span></span>
- <span data-ttu-id="9f43d-155">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="9f43d-155">Last Activity Date</span></span>
- <span data-ttu-id="9f43d-156">Total Peer-to-peer Session Count (общее количество одноранговых сеансов)</span><span class="sxs-lookup"><span data-stu-id="9f43d-156">Total Peer-to-peer Session Count</span></span>
- <span data-ttu-id="9f43d-157">Total Organized Conference Count (общее количество организованных конференций)</span><span class="sxs-lookup"><span data-stu-id="9f43d-157">Total Organized Conference Count</span></span>
- <span data-ttu-id="9f43d-158">Total Participated Conference Count (общее количество конференций с участием пользователя)</span><span class="sxs-lookup"><span data-stu-id="9f43d-158">Total Participated Conference Count</span></span>
- <span data-ttu-id="9f43d-159">Peer-to-peer Last Activity Date (дата последнего действия в одноранговом сеансе)</span><span class="sxs-lookup"><span data-stu-id="9f43d-159">Peer-to-peer Last Activity Date</span></span>
- <span data-ttu-id="9f43d-160">Organized Conference Last Activity Date (дата последнего действия в организованной конференции)</span><span class="sxs-lookup"><span data-stu-id="9f43d-160">Organized Conference Last Activity Date</span></span>
- <span data-ttu-id="9f43d-161">Participated Conference Last Activity Date (дата последнего действия в конференции с участием пользователя)</span><span class="sxs-lookup"><span data-stu-id="9f43d-161">Participated Conference Last Activity Date</span></span>
- <span data-ttu-id="9f43d-162">Peer-to-peer IM Count (количество одноранговых сеансов с обменом мгновенными сообщениями)</span><span class="sxs-lookup"><span data-stu-id="9f43d-162">Peer-to-peer IM Count</span></span>
- <span data-ttu-id="9f43d-163">Peer-to-peer Audio Count (количество одноранговых сеансов с аудиосвязью)</span><span class="sxs-lookup"><span data-stu-id="9f43d-163">Peer-to-peer Audio Count</span></span>
- <span data-ttu-id="9f43d-164">Peer-to-peer Audio Minutes (продолжительность одноранговых сеансов с аудиосвязью, в минутах)</span><span class="sxs-lookup"><span data-stu-id="9f43d-164">Peer-to-peer Audio Minutes</span></span>
- <span data-ttu-id="9f43d-165">Peer-to-peer Video Count (количество одноранговых сеансов с видеосвязью)</span><span class="sxs-lookup"><span data-stu-id="9f43d-165">Peer-to-peer Video Count</span></span>
- <span data-ttu-id="9f43d-166">Peer-to-peer Video Minutes (продолжительность одноранговых сеансов с видеосвязью, в минутах)</span><span class="sxs-lookup"><span data-stu-id="9f43d-166">Peer-to-peer Video Minutes</span></span>
- <span data-ttu-id="9f43d-167">Peer-to-peer App Sharing Count (количество одноранговых сеансов с общим доступом к приложениям)</span><span class="sxs-lookup"><span data-stu-id="9f43d-167">Peer-to-peer App Sharing Count</span></span>
- <span data-ttu-id="9f43d-168">Peer-to-peer File Transfer Count (количество одноранговых сеансов с передачей файлов)</span><span class="sxs-lookup"><span data-stu-id="9f43d-168">Peer-to-peer File Transfer Count</span></span>
- <span data-ttu-id="9f43d-169">Organized Conference IM Count (количество организованных конференций с обменом мгновенными сообщениями)</span><span class="sxs-lookup"><span data-stu-id="9f43d-169">Organized Conference IM Count</span></span>
- <span data-ttu-id="9f43d-170">Organized Conference Audio/Video Count (количество организованных конференций с аудио- и видеосвязью)</span><span class="sxs-lookup"><span data-stu-id="9f43d-170">Organized Conference Audio/Video Count</span></span>
- <span data-ttu-id="9f43d-171">Organized Conference Audio/Video Minutes (продолжительность организованных конференций с аудио- и видеосвязью, в минутах)</span><span class="sxs-lookup"><span data-stu-id="9f43d-171">Organized Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="9f43d-172">Organized Conference App Sharing Count (количество организованных конференций с общим доступом к приложениям)</span><span class="sxs-lookup"><span data-stu-id="9f43d-172">Organized Conference App Sharing Count</span></span>
- <span data-ttu-id="9f43d-173">Organized Conference Web Count (количество организованных веб-конференций)</span><span class="sxs-lookup"><span data-stu-id="9f43d-173">Organized Conference Web Count</span></span>
- <span data-ttu-id="9f43d-174">Organized Conference Dial-in/out 3rd Party Count (количество организованных конференций с телефонным подключением или с присоединением обратным звонком, сторонняя служба)</span><span class="sxs-lookup"><span data-stu-id="9f43d-174">Organized Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="9f43d-175">Organized Conference Dial-in/out Microsoft Count (количество организованных конференций с телефонным подключением или с присоединением обратным звонком, Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f43d-175">Organized Conference Dial-in/out Microsoft Count</span></span>
- <span data-ttu-id="9f43d-176">Organized Conference Dial-in Microsoft Minutes (продолжительность организованных конференций с телефонным подключением, Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f43d-176">Organized Conference Dial-in Microsoft Minutes</span></span>
- <span data-ttu-id="9f43d-177">Organized Conference Dial-out Microsoft Minutes (продолжительность организованных конференций с присоединением обратным звонком, Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f43d-177">Organized Conference Dial-out Microsoft Minutes</span></span>
- <span data-ttu-id="9f43d-178">Число конференций являлся обмена мгновенными Сообщениями</span><span class="sxs-lookup"><span data-stu-id="9f43d-178">Participated Conference IM Count</span></span>
- <span data-ttu-id="9f43d-179">Participated Conference Audio/Video Count (количество конференций с участием пользователя и аудио- и видеосвязью)</span><span class="sxs-lookup"><span data-stu-id="9f43d-179">Participated Conference Audio/Video Count</span></span>
- <span data-ttu-id="9f43d-180">Participated Conference Audio/Video Minutes (продолжительность конференций с участием пользователя и аудио- и видеосвязью)</span><span class="sxs-lookup"><span data-stu-id="9f43d-180">Participated Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="9f43d-181">Participated Conference App Sharing Count (количество конференций с участием пользователя и общим доступом к приложениям)</span><span class="sxs-lookup"><span data-stu-id="9f43d-181">Participated Conference App Sharing Count</span></span>
- <span data-ttu-id="9f43d-182">Participated Conference Web Count (количество веб-конференций с участием пользователя)</span><span class="sxs-lookup"><span data-stu-id="9f43d-182">Participated Conference Web Count</span></span>
- <span data-ttu-id="9f43d-183">Participated Conference Dial-in/out 3rd Party Count (количество конференций с участием пользователя и телефонным подключением или с присоединением обратным звонком, сторонняя служба)</span><span class="sxs-lookup"><span data-stu-id="9f43d-183">Participated Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="9f43d-184">Assigned Products (назначенные продукты)</span><span class="sxs-lookup"><span data-stu-id="9f43d-184">Assigned Products</span></span>
- <span data-ttu-id="9f43d-185">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="9f43d-185">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="9f43d-186">JSON</span><span class="sxs-lookup"><span data-stu-id="9f43d-186">JSON</span></span>

<span data-ttu-id="9f43d-187">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[skypeForBusinessActivityUserDetail](../resources/skypeforbusinessactivityuserdetail.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="9f43d-187">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessActivityUserDetail](../resources/skypeforbusinessactivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="9f43d-188">Размер страницы по умолчанию для этого запроса — 200 элементов.</span><span class="sxs-lookup"><span data-stu-id="9f43d-188">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="9f43d-189">Пример</span><span class="sxs-lookup"><span data-stu-id="9f43d-189">Example</span></span>

### <a name="csv"></a><span data-ttu-id="9f43d-190">CSV</span><span class="sxs-lookup"><span data-stu-id="9f43d-190">CSV</span></span>

<span data-ttu-id="9f43d-191">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="9f43d-191">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="9f43d-192">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f43d-192">Request</span></span>

<span data-ttu-id="9f43d-193">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f43d-193">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivityuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="9f43d-194">Ответ</span><span class="sxs-lookup"><span data-stu-id="9f43d-194">Response</span></span>

<span data-ttu-id="9f43d-195">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9f43d-195">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="9f43d-196">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="9f43d-196">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="9f43d-197">JSON</span><span class="sxs-lookup"><span data-stu-id="9f43d-197">JSON</span></span>

<span data-ttu-id="9f43d-198">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="9f43d-198">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="9f43d-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f43d-199">Request</span></span>

<span data-ttu-id="9f43d-200">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f43d-200">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivityuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="9f43d-201">Ответ</span><span class="sxs-lookup"><span data-stu-id="9f43d-201">Response</span></span>

<span data-ttu-id="9f43d-202">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9f43d-202">The following is an example of the response.</span></span>

> <span data-ttu-id="9f43d-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9f43d-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
