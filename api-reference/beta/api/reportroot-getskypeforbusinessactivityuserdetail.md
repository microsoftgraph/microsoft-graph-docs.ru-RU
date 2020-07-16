---
title: 'reportRoot: getSkypeForBusinessActivityUserDetail'
description: Получите сведения о действиях пользователей в Skype для бизнеса.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: a9356841cb71180cebf0f79053c62c2f8d025f87
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896205"
---
# <a name="reportroot-getskypeforbusinessactivityuserdetail"></a><span data-ttu-id="ec92c-103">reportRoot: getSkypeForBusinessActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="ec92c-103">reportRoot: getSkypeForBusinessActivityUserDetail</span></span>

<span data-ttu-id="ec92c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec92c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec92c-105">Получите сведения о действиях пользователей в Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="ec92c-105">Get details about Skype for Business activity by user.</span></span>

> <span data-ttu-id="ec92c-106">**Примечание:** Сведения о различных представлениях отчетов и их именах можно найти в [статье Microsoft 365 Reports-Activity for Skype для бизнеса](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span><span class="sxs-lookup"><span data-stu-id="ec92c-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="ec92c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ec92c-107">Permissions</span></span>

<span data-ttu-id="ec92c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec92c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ec92c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ec92c-110">Permission type</span></span>                        | <span data-ttu-id="ec92c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ec92c-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ec92c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ec92c-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="ec92c-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ec92c-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ec92c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ec92c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec92c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec92c-115">Not supported.</span></span>                           |
| <span data-ttu-id="ec92c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ec92c-116">Application</span></span>                            | <span data-ttu-id="ec92c-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ec92c-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="ec92c-118">**Примечание**. Чтобы разрешить приложениям читать отчеты об использовании служб от имени пользователя с помощью делегированных разрешений, администратор клиента должен назначить пользователю соответствующую роль ограниченного администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ec92c-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="ec92c-119">Более подробную информацию [можно узнать в статье авторизация для API для чтения отчетов об использовании Microsoft 365](/graph/reportroot-authorization).</span><span class="sxs-lookup"><span data-stu-id="ec92c-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="ec92c-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ec92c-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessActivityUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="ec92c-121">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="ec92c-121">Function parameters</span></span>

<span data-ttu-id="ec92c-122">В URL-адресе запроса укажите один из приведенных ниже параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="ec92c-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="ec92c-123">Параметр</span><span class="sxs-lookup"><span data-stu-id="ec92c-123">Parameter</span></span> | <span data-ttu-id="ec92c-124">Тип</span><span class="sxs-lookup"><span data-stu-id="ec92c-124">Type</span></span>   | <span data-ttu-id="ec92c-125">Описание</span><span class="sxs-lookup"><span data-stu-id="ec92c-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="ec92c-126">period</span><span class="sxs-lookup"><span data-stu-id="ec92c-126">period</span></span>    | <span data-ttu-id="ec92c-127">string</span><span class="sxs-lookup"><span data-stu-id="ec92c-127">string</span></span> | <span data-ttu-id="ec92c-128">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="ec92c-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="ec92c-129">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="ec92c-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="ec92c-130">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="ec92c-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="ec92c-131">date</span><span class="sxs-lookup"><span data-stu-id="ec92c-131">date</span></span>      | <span data-ttu-id="ec92c-132">Date</span><span class="sxs-lookup"><span data-stu-id="ec92c-132">Date</span></span>   | <span data-ttu-id="ec92c-133">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="ec92c-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="ec92c-134">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="ec92c-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="ec92c-135">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="ec92c-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="ec92c-136">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="ec92c-136">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="ec92c-137">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$format`, `$top` и `$skipToken` для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ec92c-137">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="ec92c-138">Тип выходных данных по умолчанию — Text/CSV.</span><span class="sxs-lookup"><span data-stu-id="ec92c-138">The default output type is text/csv.</span></span> <span data-ttu-id="ec92c-139">Тем не менее, если вы хотите указать тип выходных данных, можно использовать параметр запроса OData $format, для которого задано значение Text/CSV или Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="ec92c-139">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ec92c-140">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ec92c-140">Request headers</span></span>

| <span data-ttu-id="ec92c-141">Имя</span><span class="sxs-lookup"><span data-stu-id="ec92c-141">Name</span></span>          | <span data-ttu-id="ec92c-142">Описание</span><span class="sxs-lookup"><span data-stu-id="ec92c-142">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="ec92c-143">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ec92c-143">Authorization</span></span> | <span data-ttu-id="ec92c-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ec92c-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="ec92c-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec92c-146">Response</span></span>

### <a name="csv"></a><span data-ttu-id="ec92c-147">CSV</span><span class="sxs-lookup"><span data-stu-id="ec92c-147">CSV</span></span>

<span data-ttu-id="ec92c-148">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="ec92c-148">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ec92c-149">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="ec92c-149">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ec92c-150">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="ec92c-150">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ec92c-151">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="ec92c-151">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="ec92c-152">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="ec92c-152">Report Refresh Date</span></span>
- <span data-ttu-id="ec92c-153">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="ec92c-153">User Principal Name</span></span>
- <span data-ttu-id="ec92c-154">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="ec92c-154">Is Deleted</span></span>
- <span data-ttu-id="ec92c-155">"Deleted Date" (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="ec92c-155">Deleted Date</span></span>
- <span data-ttu-id="ec92c-156">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="ec92c-156">Last Activity Date</span></span>
- <span data-ttu-id="ec92c-157">Total Peer-to-peer Session Count (общее количество одноранговых сеансов)</span><span class="sxs-lookup"><span data-stu-id="ec92c-157">Total Peer-to-peer Session Count</span></span>
- <span data-ttu-id="ec92c-158">Total Organized Conference Count (общее количество организованных конференций)</span><span class="sxs-lookup"><span data-stu-id="ec92c-158">Total Organized Conference Count</span></span>
- <span data-ttu-id="ec92c-159">Total Participated Conference Count (общее количество конференций с участием пользователя)</span><span class="sxs-lookup"><span data-stu-id="ec92c-159">Total Participated Conference Count</span></span>
- <span data-ttu-id="ec92c-160">Peer-to-peer Last Activity Date (дата последнего действия в одноранговом сеансе)</span><span class="sxs-lookup"><span data-stu-id="ec92c-160">Peer-to-peer Last Activity Date</span></span>
- <span data-ttu-id="ec92c-161">Organized Conference Last Activity Date (дата последнего действия в организованной конференции)</span><span class="sxs-lookup"><span data-stu-id="ec92c-161">Organized Conference Last Activity Date</span></span>
- <span data-ttu-id="ec92c-162">Participated Conference Last Activity Date (дата последнего действия в конференции с участием пользователя)</span><span class="sxs-lookup"><span data-stu-id="ec92c-162">Participated Conference Last Activity Date</span></span>
- <span data-ttu-id="ec92c-163">Peer-to-peer IM Count (количество одноранговых сеансов с обменом мгновенными сообщениями)</span><span class="sxs-lookup"><span data-stu-id="ec92c-163">Peer-to-peer IM Count</span></span>
- <span data-ttu-id="ec92c-164">Peer-to-peer Audio Count (количество одноранговых сеансов с аудиосвязью)</span><span class="sxs-lookup"><span data-stu-id="ec92c-164">Peer-to-peer Audio Count</span></span>
- <span data-ttu-id="ec92c-165">Peer-to-peer Audio Minutes (продолжительность одноранговых сеансов с аудиосвязью, в минутах)</span><span class="sxs-lookup"><span data-stu-id="ec92c-165">Peer-to-peer Audio Minutes</span></span>
- <span data-ttu-id="ec92c-166">Peer-to-peer Video Count (количество одноранговых сеансов с видеосвязью)</span><span class="sxs-lookup"><span data-stu-id="ec92c-166">Peer-to-peer Video Count</span></span>
- <span data-ttu-id="ec92c-167">Peer-to-peer Video Minutes (продолжительность одноранговых сеансов с видеосвязью, в минутах)</span><span class="sxs-lookup"><span data-stu-id="ec92c-167">Peer-to-peer Video Minutes</span></span>
- <span data-ttu-id="ec92c-168">Peer-to-peer App Sharing Count (количество одноранговых сеансов с общим доступом к приложениям)</span><span class="sxs-lookup"><span data-stu-id="ec92c-168">Peer-to-peer App Sharing Count</span></span>
- <span data-ttu-id="ec92c-169">Peer-to-peer File Transfer Count (количество одноранговых сеансов с передачей файлов)</span><span class="sxs-lookup"><span data-stu-id="ec92c-169">Peer-to-peer File Transfer Count</span></span>
- <span data-ttu-id="ec92c-170">Organized Conference IM Count (количество организованных конференций с обменом мгновенными сообщениями)</span><span class="sxs-lookup"><span data-stu-id="ec92c-170">Organized Conference IM Count</span></span>
- <span data-ttu-id="ec92c-171">Organized Conference Audio/Video Count (количество организованных конференций с аудио- и видеосвязью)</span><span class="sxs-lookup"><span data-stu-id="ec92c-171">Organized Conference Audio/Video Count</span></span>
- <span data-ttu-id="ec92c-172">Organized Conference Audio/Video Minutes (продолжительность организованных конференций с аудио- и видеосвязью, в минутах)</span><span class="sxs-lookup"><span data-stu-id="ec92c-172">Organized Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="ec92c-173">Organized Conference App Sharing Count (количество организованных конференций с общим доступом к приложениям)</span><span class="sxs-lookup"><span data-stu-id="ec92c-173">Organized Conference App Sharing Count</span></span>
- <span data-ttu-id="ec92c-174">Organized Conference Web Count (количество организованных веб-конференций)</span><span class="sxs-lookup"><span data-stu-id="ec92c-174">Organized Conference Web Count</span></span>
- <span data-ttu-id="ec92c-175">Organized Conference Dial-in/out 3rd Party Count (количество организованных конференций с телефонным подключением или с присоединением обратным звонком, сторонняя служба)</span><span class="sxs-lookup"><span data-stu-id="ec92c-175">Organized Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="ec92c-176">Organized Conference Dial-in/out Microsoft Count (количество организованных конференций с телефонным подключением или с присоединением обратным звонком, Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ec92c-176">Organized Conference Dial-in/out Microsoft Count</span></span>
- <span data-ttu-id="ec92c-177">Organized Conference Dial-in Microsoft Minutes (продолжительность организованных конференций с телефонным подключением, Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ec92c-177">Organized Conference Dial-in Microsoft Minutes</span></span>
- <span data-ttu-id="ec92c-178">Organized Conference Dial-out Microsoft Minutes (продолжительность организованных конференций с присоединением обратным звонком, Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ec92c-178">Organized Conference Dial-out Microsoft Minutes</span></span>
- <span data-ttu-id="ec92c-179">Количество мгновенных сообщений для конференций с участием</span><span class="sxs-lookup"><span data-stu-id="ec92c-179">Participated Conference IM Count</span></span>
- <span data-ttu-id="ec92c-180">Participated Conference Audio/Video Count (количество конференций с участием пользователя и аудио- и видеосвязью)</span><span class="sxs-lookup"><span data-stu-id="ec92c-180">Participated Conference Audio/Video Count</span></span>
- <span data-ttu-id="ec92c-181">Participated Conference Audio/Video Minutes (продолжительность конференций с участием пользователя и аудио- и видеосвязью)</span><span class="sxs-lookup"><span data-stu-id="ec92c-181">Participated Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="ec92c-182">Participated Conference App Sharing Count (количество конференций с участием пользователя и общим доступом к приложениям)</span><span class="sxs-lookup"><span data-stu-id="ec92c-182">Participated Conference App Sharing Count</span></span>
- <span data-ttu-id="ec92c-183">Participated Conference Web Count (количество веб-конференций с участием пользователя)</span><span class="sxs-lookup"><span data-stu-id="ec92c-183">Participated Conference Web Count</span></span>
- <span data-ttu-id="ec92c-184">Participated Conference Dial-in/out 3rd Party Count (количество конференций с участием пользователя и телефонным подключением или с присоединением обратным звонком, сторонняя служба)</span><span class="sxs-lookup"><span data-stu-id="ec92c-184">Participated Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="ec92c-185">Assigned Products (назначенные продукты)</span><span class="sxs-lookup"><span data-stu-id="ec92c-185">Assigned Products</span></span>
- <span data-ttu-id="ec92c-186">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="ec92c-186">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="ec92c-187">JSON</span><span class="sxs-lookup"><span data-stu-id="ec92c-187">JSON</span></span>

<span data-ttu-id="ec92c-188">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **[скипефорбусинессактивитюсердетаил](../resources/skypeforbusinessactivityuserdetail.md)** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ec92c-188">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessActivityUserDetail](../resources/skypeforbusinessactivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="ec92c-189">Размер страницы по умолчанию для этого запроса составляет 200 элементов.</span><span class="sxs-lookup"><span data-stu-id="ec92c-189">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="ec92c-190">Пример</span><span class="sxs-lookup"><span data-stu-id="ec92c-190">Example</span></span>

### <a name="csv"></a><span data-ttu-id="ec92c-191">CSV</span><span class="sxs-lookup"><span data-stu-id="ec92c-191">CSV</span></span>

<span data-ttu-id="ec92c-192">Ниже приведен пример выходных данных CSV.</span><span class="sxs-lookup"><span data-stu-id="ec92c-192">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="ec92c-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="ec92c-193">Request</span></span>

<span data-ttu-id="ec92c-194">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ec92c-194">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getskypeforbusinessactivityuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityUserDetail(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="ec92c-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec92c-195">Response</span></span>

<span data-ttu-id="ec92c-196">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ec92c-196">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="ec92c-197">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="ec92c-197">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="ec92c-198">JSON</span><span class="sxs-lookup"><span data-stu-id="ec92c-198">JSON</span></span>

<span data-ttu-id="ec92c-199">Ниже приведен пример, в котором возвращается JSON.</span><span class="sxs-lookup"><span data-stu-id="ec92c-199">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="ec92c-200">Запрос</span><span class="sxs-lookup"><span data-stu-id="ec92c-200">Request</span></span>

<span data-ttu-id="ec92c-201">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ec92c-201">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getskypeforbusinessactivityuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityUserDetail(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="ec92c-202">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec92c-202">Response</span></span>

<span data-ttu-id="ec92c-203">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ec92c-203">The following is an example of the response.</span></span>

> <span data-ttu-id="ec92c-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ec92c-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
        "Microsoft 365 ENTERPRISE E5", 
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
