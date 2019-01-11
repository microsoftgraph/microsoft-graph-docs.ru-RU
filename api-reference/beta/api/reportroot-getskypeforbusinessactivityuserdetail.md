---
title: 'reportRoot: getSkypeForBusinessActivityUserDetail'
description: Получите сведения о действиях пользователей в Skype для бизнеса.
localization_priority: Normal
ms.openlocfilehash: 43bf2d7f08bc9a0033bd04f98687c7d03be5f2ea
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872634"
---
# <a name="reportroot-getskypeforbusinessactivityuserdetail"></a><span data-ttu-id="bdbfc-103">reportRoot: getSkypeForBusinessActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="bdbfc-103">reportRoot: getSkypeForBusinessActivityUserDetail</span></span>

> <span data-ttu-id="bdbfc-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bdbfc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bdbfc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bdbfc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bdbfc-106">Получите сведения о действиях пользователей в Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="bdbfc-106">Get details about Skype for Business activity by user.</span></span>

> <span data-ttu-id="bdbfc-107">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span><span class="sxs-lookup"><span data-stu-id="bdbfc-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="bdbfc-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bdbfc-108">Permissions</span></span>

<span data-ttu-id="bdbfc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bdbfc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bdbfc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bdbfc-111">Permission type</span></span>                        | <span data-ttu-id="bdbfc-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bdbfc-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="bdbfc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bdbfc-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="bdbfc-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bdbfc-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="bdbfc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bdbfc-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bdbfc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bdbfc-116">Not supported.</span></span>                           |
| <span data-ttu-id="bdbfc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bdbfc-117">Application</span></span>                            | <span data-ttu-id="bdbfc-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bdbfc-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="bdbfc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bdbfc-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessActivityUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="bdbfc-120">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="bdbfc-120">Function parameters</span></span>

<span data-ttu-id="bdbfc-121">В URL-адресе запроса укажите один из следующих параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="bdbfc-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="bdbfc-122">Параметр</span><span class="sxs-lookup"><span data-stu-id="bdbfc-122">Parameter</span></span> | <span data-ttu-id="bdbfc-123">Тип</span><span class="sxs-lookup"><span data-stu-id="bdbfc-123">Type</span></span>   | <span data-ttu-id="bdbfc-124">Описание</span><span class="sxs-lookup"><span data-stu-id="bdbfc-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="bdbfc-125">period</span><span class="sxs-lookup"><span data-stu-id="bdbfc-125">period</span></span>    | <span data-ttu-id="bdbfc-126">строка</span><span class="sxs-lookup"><span data-stu-id="bdbfc-126">string</span></span> | <span data-ttu-id="bdbfc-127">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="bdbfc-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="bdbfc-128">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="bdbfc-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="bdbfc-129">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="bdbfc-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="bdbfc-130">date</span><span class="sxs-lookup"><span data-stu-id="bdbfc-130">date</span></span>      | <span data-ttu-id="bdbfc-131">Date</span><span class="sxs-lookup"><span data-stu-id="bdbfc-131">Date</span></span>   | <span data-ttu-id="bdbfc-132">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="bdbfc-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="bdbfc-133">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="bdbfc-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="bdbfc-134">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="bdbfc-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="bdbfc-135">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="bdbfc-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="bdbfc-136">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bdbfc-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="bdbfc-137">Выходной тип по умолчанию — текст и csv.</span><span class="sxs-lookup"><span data-stu-id="bdbfc-137">The default output type is text/csv.</span></span> <span data-ttu-id="bdbfc-138">Тем не менее если вы хотите указать тип выходных данных, можно использовать параметр $format запроса OData, задайте значение text/CSV-файла или приложение/json.</span><span class="sxs-lookup"><span data-stu-id="bdbfc-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bdbfc-139">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bdbfc-139">Request headers</span></span>

| <span data-ttu-id="bdbfc-140">Имя</span><span class="sxs-lookup"><span data-stu-id="bdbfc-140">Name</span></span>          | <span data-ttu-id="bdbfc-141">Описание</span><span class="sxs-lookup"><span data-stu-id="bdbfc-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="bdbfc-142">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bdbfc-142">Authorization</span></span> | <span data-ttu-id="bdbfc-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bdbfc-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="bdbfc-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="bdbfc-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="bdbfc-146">CSV</span><span class="sxs-lookup"><span data-stu-id="bdbfc-146">CSV</span></span>

<span data-ttu-id="bdbfc-147">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="bdbfc-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="bdbfc-148">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="bdbfc-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="bdbfc-149">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="bdbfc-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="bdbfc-150">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="bdbfc-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="bdbfc-151">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="bdbfc-151">Report Refresh Date</span></span>
- <span data-ttu-id="bdbfc-152">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="bdbfc-152">User Principal Name</span></span>
- <span data-ttu-id="bdbfc-153">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="bdbfc-153">Is Deleted</span></span>
- <span data-ttu-id="bdbfc-154">"Deleted Date" (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="bdbfc-154">Deleted Date</span></span>
- <span data-ttu-id="bdbfc-155">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="bdbfc-155">Last Activity Date</span></span>
- <span data-ttu-id="bdbfc-156">Total Peer-to-peer Session Count (общее количество одноранговых сеансов)</span><span class="sxs-lookup"><span data-stu-id="bdbfc-156">Total Peer-to-peer Session Count</span></span>
- <span data-ttu-id="bdbfc-157">Total Organized Conference Count (общее количество организованных конференций)</span><span class="sxs-lookup"><span data-stu-id="bdbfc-157">Total Organized Conference Count</span></span>
- <span data-ttu-id="bdbfc-158">Total Participated Conference Count (общее количество конференций с участием пользователя)</span><span class="sxs-lookup"><span data-stu-id="bdbfc-158">Total Participated Conference Count</span></span>
- <span data-ttu-id="bdbfc-159">Peer-to-peer Last Activity Date (дата последнего действия в одноранговом сеансе)</span><span class="sxs-lookup"><span data-stu-id="bdbfc-159">Peer-to-peer Last Activity Date</span></span>
- <span data-ttu-id="bdbfc-160">Organized Conference Last Activity Date (дата последнего действия в организованной конференции)</span><span class="sxs-lookup"><span data-stu-id="bdbfc-160">Organized Conference Last Activity Date</span></span>
- <span data-ttu-id="bdbfc-161">Participated Conference Last Activity Date (дата последнего действия в конференции с участием пользователя)</span><span class="sxs-lookup"><span data-stu-id="bdbfc-161">Participated Conference Last Activity Date</span></span>
- <span data-ttu-id="bdbfc-162">Peer-to-peer IM Count (количество одноранговых сеансов с обменом мгновенными сообщениями)</span><span class="sxs-lookup"><span data-stu-id="bdbfc-162">Peer-to-peer IM Count</span></span>
- <span data-ttu-id="bdbfc-163">Peer-to-peer Audio Count (количество одноранговых сеансов с аудиосвязью)</span><span class="sxs-lookup"><span data-stu-id="bdbfc-163">Peer-to-peer Audio Count</span></span>
- <span data-ttu-id="bdbfc-164">Peer-to-peer Audio Minutes (продолжительность одноранговых сеансов с аудиосвязью, в минутах)</span><span class="sxs-lookup"><span data-stu-id="bdbfc-164">Peer-to-peer Audio Minutes</span></span>
- <span data-ttu-id="bdbfc-165">Peer-to-peer Video Count (количество одноранговых сеансов с видеосвязью)</span><span class="sxs-lookup"><span data-stu-id="bdbfc-165">Peer-to-peer Video Count</span></span>
- <span data-ttu-id="bdbfc-166">Peer-to-peer Video Minutes (продолжительность одноранговых сеансов с видеосвязью, в минутах)</span><span class="sxs-lookup"><span data-stu-id="bdbfc-166">Peer-to-peer Video Minutes</span></span>
- <span data-ttu-id="bdbfc-167">Peer-to-peer App Sharing Count (количество одноранговых сеансов с общим доступом к приложениям)</span><span class="sxs-lookup"><span data-stu-id="bdbfc-167">Peer-to-peer App Sharing Count</span></span>
- <span data-ttu-id="bdbfc-168">Peer-to-peer File Transfer Count (количество одноранговых сеансов с передачей файлов)</span><span class="sxs-lookup"><span data-stu-id="bdbfc-168">Peer-to-peer File Transfer Count</span></span>
- <span data-ttu-id="bdbfc-169">Organized Conference IM Count (количество организованных конференций с обменом мгновенными сообщениями)</span><span class="sxs-lookup"><span data-stu-id="bdbfc-169">Organized Conference IM Count</span></span>
- <span data-ttu-id="bdbfc-170">Organized Conference Audio/Video Count (количество организованных конференций с аудио- и видеосвязью)</span><span class="sxs-lookup"><span data-stu-id="bdbfc-170">Organized Conference Audio/Video Count</span></span>
- <span data-ttu-id="bdbfc-171">Organized Conference Audio/Video Minutes (продолжительность организованных конференций с аудио- и видеосвязью, в минутах)</span><span class="sxs-lookup"><span data-stu-id="bdbfc-171">Organized Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="bdbfc-172">Organized Conference App Sharing Count (количество организованных конференций с общим доступом к приложениям)</span><span class="sxs-lookup"><span data-stu-id="bdbfc-172">Organized Conference App Sharing Count</span></span>
- <span data-ttu-id="bdbfc-173">Organized Conference Web Count (количество организованных веб-конференций)</span><span class="sxs-lookup"><span data-stu-id="bdbfc-173">Organized Conference Web Count</span></span>
- <span data-ttu-id="bdbfc-174">Organized Conference Dial-in/out 3rd Party Count (количество организованных конференций с телефонным подключением или с присоединением обратным звонком, сторонняя служба)</span><span class="sxs-lookup"><span data-stu-id="bdbfc-174">Organized Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="bdbfc-175">Organized Conference Dial-in/out Microsoft Count (количество организованных конференций с телефонным подключением или с присоединением обратным звонком, Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bdbfc-175">Organized Conference Dial-in/out Microsoft Count</span></span>
- <span data-ttu-id="bdbfc-176">Organized Conference Dial-in Microsoft Minutes (продолжительность организованных конференций с телефонным подключением, Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bdbfc-176">Organized Conference Dial-in Microsoft Minutes</span></span>
- <span data-ttu-id="bdbfc-177">Organized Conference Dial-out Microsoft Minutes (продолжительность организованных конференций с присоединением обратным звонком, Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bdbfc-177">Organized Conference Dial-out Microsoft Minutes</span></span>
- <span data-ttu-id="bdbfc-178">Число конференций являлся обмена мгновенными Сообщениями</span><span class="sxs-lookup"><span data-stu-id="bdbfc-178">Participated Conference IM Count</span></span>
- <span data-ttu-id="bdbfc-179">Participated Conference Audio/Video Count (количество конференций с участием пользователя и аудио- и видеосвязью)</span><span class="sxs-lookup"><span data-stu-id="bdbfc-179">Participated Conference Audio/Video Count</span></span>
- <span data-ttu-id="bdbfc-180">Participated Conference Audio/Video Minutes (продолжительность конференций с участием пользователя и аудио- и видеосвязью)</span><span class="sxs-lookup"><span data-stu-id="bdbfc-180">Participated Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="bdbfc-181">Participated Conference App Sharing Count (количество конференций с участием пользователя и общим доступом к приложениям)</span><span class="sxs-lookup"><span data-stu-id="bdbfc-181">Participated Conference App Sharing Count</span></span>
- <span data-ttu-id="bdbfc-182">Participated Conference Web Count (количество веб-конференций с участием пользователя)</span><span class="sxs-lookup"><span data-stu-id="bdbfc-182">Participated Conference Web Count</span></span>
- <span data-ttu-id="bdbfc-183">Participated Conference Dial-in/out 3rd Party Count (количество конференций с участием пользователя и телефонным подключением или с присоединением обратным звонком, сторонняя служба)</span><span class="sxs-lookup"><span data-stu-id="bdbfc-183">Participated Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="bdbfc-184">Assigned Products (назначенные продукты)</span><span class="sxs-lookup"><span data-stu-id="bdbfc-184">Assigned Products</span></span>
- <span data-ttu-id="bdbfc-185">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="bdbfc-185">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="bdbfc-186">JSON</span><span class="sxs-lookup"><span data-stu-id="bdbfc-186">JSON</span></span>

<span data-ttu-id="bdbfc-187">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект **[skypeForBusinessActivityUserDetail](../resources/skypeforbusinessactivityuserdetail.md)** в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="bdbfc-187">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessActivityUserDetail](../resources/skypeforbusinessactivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="bdbfc-188">Размер страницы по умолчанию для этого запроса — 200 элементов.</span><span class="sxs-lookup"><span data-stu-id="bdbfc-188">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="bdbfc-189">Пример</span><span class="sxs-lookup"><span data-stu-id="bdbfc-189">Example</span></span>

### <a name="csv"></a><span data-ttu-id="bdbfc-190">CSV</span><span class="sxs-lookup"><span data-stu-id="bdbfc-190">CSV</span></span>

<span data-ttu-id="bdbfc-191">Ниже приведен пример выводит CSV.</span><span class="sxs-lookup"><span data-stu-id="bdbfc-191">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="bdbfc-192">Запрос</span><span class="sxs-lookup"><span data-stu-id="bdbfc-192">Request</span></span>

<span data-ttu-id="bdbfc-193">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bdbfc-193">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivityuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="bdbfc-194">Ответ</span><span class="sxs-lookup"><span data-stu-id="bdbfc-194">Response</span></span>

<span data-ttu-id="bdbfc-195">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="bdbfc-195">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="bdbfc-196">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="bdbfc-196">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="bdbfc-197">JSON</span><span class="sxs-lookup"><span data-stu-id="bdbfc-197">JSON</span></span>

<span data-ttu-id="bdbfc-198">Ниже приведен пример, в котором возвращает JSON.</span><span class="sxs-lookup"><span data-stu-id="bdbfc-198">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="bdbfc-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="bdbfc-199">Request</span></span>

<span data-ttu-id="bdbfc-200">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bdbfc-200">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivityuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="bdbfc-201">Ответ</span><span class="sxs-lookup"><span data-stu-id="bdbfc-201">Response</span></span>

<span data-ttu-id="bdbfc-202">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bdbfc-202">The following is an example of the response.</span></span>

> <span data-ttu-id="bdbfc-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bdbfc-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
