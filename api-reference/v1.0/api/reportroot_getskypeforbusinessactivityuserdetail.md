# <a name="reportroot-getskypeforbusinessactivityuserdetail"></a><span data-ttu-id="1dae9-101">reportRoot: getSkypeForBusinessActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="1dae9-101">reportRoot: getSkypeForBusinessActivityUserDetail</span></span>

<span data-ttu-id="1dae9-102">Получите сведения о действиях пользователей в Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="1dae9-102">Get details about Skype for Business activity by user.</span></span>

> <span data-ttu-id="1dae9-103">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span><span class="sxs-lookup"><span data-stu-id="1dae9-103">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="1dae9-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1dae9-104">Permissions</span></span>

<span data-ttu-id="1dae9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1dae9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="1dae9-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1dae9-107">Permission type</span></span>                        | <span data-ttu-id="1dae9-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1dae9-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="1dae9-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1dae9-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="1dae9-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1dae9-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="1dae9-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1dae9-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1dae9-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1dae9-112">Not supported.</span></span>                           |
| <span data-ttu-id="1dae9-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1dae9-113">Application</span></span>                            | <span data-ttu-id="1dae9-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1dae9-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="1dae9-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1dae9-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessActivityUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessActivityUserDetail(date={date_value})
```

## <a name="request-parameters"></a><span data-ttu-id="1dae9-116">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="1dae9-116">Request parameters</span></span>

<span data-ttu-id="1dae9-117">В URL-адресе запроса укажите один из следующих параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="1dae9-117">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="1dae9-118">Параметр</span><span class="sxs-lookup"><span data-stu-id="1dae9-118">Parameter</span></span> | <span data-ttu-id="1dae9-119">Тип</span><span class="sxs-lookup"><span data-stu-id="1dae9-119">Type</span></span>   | <span data-ttu-id="1dae9-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1dae9-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="1dae9-121">period</span><span class="sxs-lookup"><span data-stu-id="1dae9-121">period</span></span>    | <span data-ttu-id="1dae9-122">string</span><span class="sxs-lookup"><span data-stu-id="1dae9-122">string</span></span> | <span data-ttu-id="1dae9-123">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="1dae9-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="1dae9-124">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="1dae9-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="1dae9-125">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="1dae9-125">These values follow the format D   where    represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="1dae9-126">date</span><span class="sxs-lookup"><span data-stu-id="1dae9-126">date</span></span>      | <span data-ttu-id="1dae9-127">Date</span><span class="sxs-lookup"><span data-stu-id="1dae9-127">Date</span></span>   | <span data-ttu-id="1dae9-128">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="1dae9-128">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="1dae9-129">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="1dae9-129">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="1dae9-130">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="1dae9-130">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="1dae9-131">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="1dae9-131">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1dae9-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1dae9-132">Request headers</span></span>

| <span data-ttu-id="1dae9-133">Имя</span><span class="sxs-lookup"><span data-stu-id="1dae9-133">Name</span></span>          | <span data-ttu-id="1dae9-134">Описание</span><span class="sxs-lookup"><span data-stu-id="1dae9-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="1dae9-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1dae9-135">Authorization</span></span> | <span data-ttu-id="1dae9-p104">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1dae9-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="1dae9-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="1dae9-138">If-None-Match</span></span> | <span data-ttu-id="1dae9-139">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="1dae9-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="1dae9-140">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="1dae9-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="1dae9-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="1dae9-141">Response</span></span>

<span data-ttu-id="1dae9-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="1dae9-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="1dae9-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="1dae9-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="1dae9-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="1dae9-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="1dae9-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="1dae9-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="1dae9-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="1dae9-146">Report Refresh Date</span></span>
- <span data-ttu-id="1dae9-147">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="1dae9-147">User Principal Name</span></span>
- <span data-ttu-id="1dae9-148">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="1dae9-148">Is Deleted</span></span>
- <span data-ttu-id="1dae9-149">"Deleted Date" (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="1dae9-149">Deleted Date</span></span>
- <span data-ttu-id="1dae9-150">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="1dae9-150">Last Activity Date</span></span>
- <span data-ttu-id="1dae9-151">Total Peer-to-peer Session Count (общее количество одноранговых сеансов)</span><span class="sxs-lookup"><span data-stu-id="1dae9-151">Total Peer-to-peer Session Count</span></span>
- <span data-ttu-id="1dae9-152">Total Organized Conference Count (общее количество организованных конференций)</span><span class="sxs-lookup"><span data-stu-id="1dae9-152">Total Organized Conference Count</span></span>
- <span data-ttu-id="1dae9-153">Total Participated Conference Count (общее количество конференций с участием пользователя)</span><span class="sxs-lookup"><span data-stu-id="1dae9-153">Total Participated Conference Count</span></span>
- <span data-ttu-id="1dae9-154">Peer-to-peer Last Activity Date (дата последнего действия в одноранговом сеансе)</span><span class="sxs-lookup"><span data-stu-id="1dae9-154">Peer-to-peer Last Activity Date</span></span>
- <span data-ttu-id="1dae9-155">Organized Conference Last Activity Date (дата последнего действия в организованной конференции)</span><span class="sxs-lookup"><span data-stu-id="1dae9-155">Organized Conference Last Activity Date</span></span>
- <span data-ttu-id="1dae9-156">Participated Conference Last Activity Date (дата последнего действия в конференции с участием пользователя)</span><span class="sxs-lookup"><span data-stu-id="1dae9-156">Participated Conference Last Activity Date</span></span>
- <span data-ttu-id="1dae9-157">Peer-to-peer IM Count (количество одноранговых сеансов с обменом мгновенными сообщениями)</span><span class="sxs-lookup"><span data-stu-id="1dae9-157">Peer-to-peer IM Count</span></span>
- <span data-ttu-id="1dae9-158">Peer-to-peer Audio Count (количество одноранговых сеансов с аудиосвязью)</span><span class="sxs-lookup"><span data-stu-id="1dae9-158">Peer-to-peer Audio Count</span></span>
- <span data-ttu-id="1dae9-159">Peer-to-peer Audio Minutes (продолжительность одноранговых сеансов с аудиосвязью, в минутах)</span><span class="sxs-lookup"><span data-stu-id="1dae9-159">Peer-to-peer Audio Minutes</span></span>
- <span data-ttu-id="1dae9-160">Peer-to-peer Video Count (количество одноранговых сеансов с видеосвязью)</span><span class="sxs-lookup"><span data-stu-id="1dae9-160">Peer-to-peer Video Count</span></span>
- <span data-ttu-id="1dae9-161">Peer-to-peer Video Minutes (продолжительность одноранговых сеансов с видеосвязью, в минутах)</span><span class="sxs-lookup"><span data-stu-id="1dae9-161">Peer-to-peer Video Minutes</span></span>
- <span data-ttu-id="1dae9-162">Peer-to-peer App Sharing Count (количество одноранговых сеансов с общим доступом к приложениям)</span><span class="sxs-lookup"><span data-stu-id="1dae9-162">Peer-to-peer App Sharing Count</span></span>
- <span data-ttu-id="1dae9-163">Peer-to-peer File Transfer Count (количество одноранговых сеансов с передачей файлов)</span><span class="sxs-lookup"><span data-stu-id="1dae9-163">Peer-to-peer File Transfer Count</span></span>
- <span data-ttu-id="1dae9-164">Organized Conference IM Count (количество организованных конференций с обменом мгновенными сообщениями)</span><span class="sxs-lookup"><span data-stu-id="1dae9-164">Organized Conference IM Count</span></span>
- <span data-ttu-id="1dae9-165">Organized Conference Audio/Video Count (количество организованных конференций с аудио- и видеосвязью)</span><span class="sxs-lookup"><span data-stu-id="1dae9-165">Organized Conference Audio/Video Count</span></span>
- <span data-ttu-id="1dae9-166">Organized Conference Audio/Video Minutes (продолжительность организованных конференций с аудио- и видеосвязью, в минутах)</span><span class="sxs-lookup"><span data-stu-id="1dae9-166">Organized Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="1dae9-167">Organized Conference App Sharing Count (количество организованных конференций с общим доступом к приложениям)</span><span class="sxs-lookup"><span data-stu-id="1dae9-167">Organized Conference App Sharing Count</span></span>
- <span data-ttu-id="1dae9-168">Organized Conference Web Count (количество организованных веб-конференций)</span><span class="sxs-lookup"><span data-stu-id="1dae9-168">Organized Conference Web Count</span></span>
- <span data-ttu-id="1dae9-169">Organized Conference Dial-in/out 3rd Party Count (количество организованных конференций с телефонным подключением или с присоединением обратным звонком, сторонняя служба)</span><span class="sxs-lookup"><span data-stu-id="1dae9-169">Organized Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="1dae9-170">Organized Conference Dial-in/out Microsoft Count (количество организованных конференций с телефонным подключением или с присоединением обратным звонком, Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1dae9-170">Organized Conference Dial-in/out Microsoft Count</span></span>
- <span data-ttu-id="1dae9-171">Organized Conference Dial-in Microsoft Minutes (продолжительность организованных конференций с телефонным подключением, Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1dae9-171">Organized Conference Dial-in Microsoft Minutes</span></span>
- <span data-ttu-id="1dae9-172">Organized Conference Dial-out Microsoft Minutes (продолжительность организованных конференций с присоединением обратным звонком, Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1dae9-172">Organized Conference Dial-out Microsoft Minutes</span></span>
- <span data-ttu-id="1dae9-173">Paricipated Conference IM Count (количество конференций с участием пользователя и обменом мгновенными сообщениями)</span><span class="sxs-lookup"><span data-stu-id="1dae9-173">Paricipated Conference IM Count</span></span>
- <span data-ttu-id="1dae9-174">Participated Conference Audio/Video Count (количество конференций с участием пользователя и аудио- и видеосвязью)</span><span class="sxs-lookup"><span data-stu-id="1dae9-174">Participated Conference Audio/Video Count</span></span>
- <span data-ttu-id="1dae9-175">Participated Conference Audio/Video Minutes (продолжительность конференций с участием пользователя и аудио- и видеосвязью)</span><span class="sxs-lookup"><span data-stu-id="1dae9-175">Participated Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="1dae9-176">Participated Conference App Sharing Count (количество конференций с участием пользователя и общим доступом к приложениям)</span><span class="sxs-lookup"><span data-stu-id="1dae9-176">Participated Conference App Sharing Count</span></span>
- <span data-ttu-id="1dae9-177">Participated Conference Web Count (количество веб-конференций с участием пользователя)</span><span class="sxs-lookup"><span data-stu-id="1dae9-177">Participated Conference Web Count</span></span>
- <span data-ttu-id="1dae9-178">Participated Conference Dial-in/out 3rd Party Count (количество конференций с участием пользователя и телефонным подключением или с присоединением обратным звонком, сторонняя служба)</span><span class="sxs-lookup"><span data-stu-id="1dae9-178">Participated Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="1dae9-179">Assigned Products (назначенные продукты)</span><span class="sxs-lookup"><span data-stu-id="1dae9-179">Assigned Products</span></span>
- <span data-ttu-id="1dae9-180">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="1dae9-180">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="1dae9-181">Пример</span><span class="sxs-lookup"><span data-stu-id="1dae9-181">Example</span></span>

#### <a name="request"></a><span data-ttu-id="1dae9-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="1dae9-182">Request</span></span>

<span data-ttu-id="1dae9-183">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1dae9-183">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessActivityUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="1dae9-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="1dae9-184">Response</span></span>

<span data-ttu-id="1dae9-185">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1dae9-185">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="1dae9-186">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="1dae9-186">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Total Peer-to-peer Session Count,Total Organized Conference Count,Total Participated Conference Count,Peer-to-peer Last Activity Date,Organized Conference Last Activity Date,Participated Conference Last Activity Date,Peer-to-peer IM Count,Peer-to-peer Audio Count,Peer-to-peer Audio Minutes,Peer-to-peer Video Count,Peer-to-peer Video Minutes,Peer-to-peer App Sharing Count,Peer-to-peer File Transfer Count,Organized Conference IM Count,Organized Conference Audio/Video Count,Organized Conference Audio/Video Minutes,Organized Conference App Sharing Count,Organized Conference Web Count,Organized Conference Dial-in/out 3rd Party Count,Organized Conference Dial-in/out Microsoft Count,Organized Conference Dial-in Microsoft Minutes,Organized Conference Dial-out Microsoft Minutes,Paricipated Conference IM Count,Participated Conference Audio/Video Count,Participated Conference Audio/Video Minutes,Participated Conference App Sharing Count,Participated Conference Web Count,Participated Conference Dial-in/out 3rd Party Count,Assigned Products,Report Period
```
