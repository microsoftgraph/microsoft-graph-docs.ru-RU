# <a name="reportroot-getyammerdeviceusageuserdetail-function"></a><span data-ttu-id="987fa-101">reportRoot: getYammerDeviceUsageUserDetail function</span><span class="sxs-lookup"><span data-stu-id="987fa-101">reportRoot: getYammerDeviceUsageUserDetail function</span></span>

<span data-ttu-id="987fa-102">Получение сведений об использовании устройства с Yammer с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="987fa-102">Get details about Yammer device usage by user.</span></span>

> <span data-ttu-id="987fa-103">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: использование устройств с Yammer](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="987fa-103">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="987fa-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="987fa-104">Permissions</span></span>

<span data-ttu-id="987fa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="987fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="987fa-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="987fa-107">Permission type</span></span>                        | <span data-ttu-id="987fa-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="987fa-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="987fa-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="987fa-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="987fa-110">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="987fa-110">Not supported.</span></span>                           |
| <span data-ttu-id="987fa-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="987fa-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="987fa-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="987fa-112">Not supported.</span></span>                           |
| <span data-ttu-id="987fa-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="987fa-113">Application</span></span>                            | <span data-ttu-id="987fa-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="987fa-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="987fa-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="987fa-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserDetail(period='{period_value}')
GET /reports/getYammerDeviceUsageUserDetail(date={date_value})
```

## <a name="request-parameters"></a><span data-ttu-id="987fa-116">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="987fa-116">Request parameters</span></span>

<span data-ttu-id="987fa-117">В URL-адресе запроса укажите выбранный параметр запроса и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="987fa-117">In the request URL, provide the chosen query parameter with a valid value.</span></span>

| <span data-ttu-id="987fa-118">Параметр</span><span class="sxs-lookup"><span data-stu-id="987fa-118">Parameter</span></span> | <span data-ttu-id="987fa-119">Тип</span><span class="sxs-lookup"><span data-stu-id="987fa-119">Type</span></span>   | <span data-ttu-id="987fa-120">Описание</span><span class="sxs-lookup"><span data-stu-id="987fa-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="987fa-121">period</span><span class="sxs-lookup"><span data-stu-id="987fa-121">period</span></span>    | <span data-ttu-id="987fa-122">string</span><span class="sxs-lookup"><span data-stu-id="987fa-122">string</span></span> | <span data-ttu-id="987fa-123">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="987fa-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="987fa-124">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="987fa-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="987fa-125">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="987fa-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="987fa-126">date</span><span class="sxs-lookup"><span data-stu-id="987fa-126">date</span></span>      | <span data-ttu-id="987fa-127">Date</span><span class="sxs-lookup"><span data-stu-id="987fa-127">Date</span></span>   | <span data-ttu-id="987fa-128">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="987fa-128">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="987fa-129">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="987fa-129">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="987fa-130">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="987fa-130">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="987fa-131">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="987fa-131">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="987fa-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="987fa-132">Request headers</span></span>

| <span data-ttu-id="987fa-133">Имя</span><span class="sxs-lookup"><span data-stu-id="987fa-133">Name</span></span>          | <span data-ttu-id="987fa-134">Описание</span><span class="sxs-lookup"><span data-stu-id="987fa-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="987fa-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="987fa-135">Authorization</span></span> | <span data-ttu-id="987fa-p104">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="987fa-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="987fa-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="987fa-138">if-none-match</span></span> | <span data-ttu-id="987fa-139">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="987fa-139">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `304 Not Modified` response is returned.</span></span> <span data-ttu-id="987fa-140">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="987fa-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="987fa-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="987fa-141">Response</span></span>

<span data-ttu-id="987fa-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="987fa-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="987fa-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="987fa-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="987fa-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="987fa-144">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<span data-ttu-id="987fa-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="987fa-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="987fa-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="987fa-146">Report Refresh Date</span></span>
- <span data-ttu-id="987fa-147">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="987fa-147">User Principal Name</span></span>
- <span data-ttu-id="987fa-148">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="987fa-148">Display Name</span></span>
- <span data-ttu-id="987fa-149">"User State" (Состояние пользователя);</span><span class="sxs-lookup"><span data-stu-id="987fa-149">Migrating User State</span></span>
- <span data-ttu-id="987fa-150">"State Change Date" (Дата изменения состояния);</span><span class="sxs-lookup"><span data-stu-id="987fa-150">State Change Date</span></span>
- <span data-ttu-id="987fa-151">"Last Activity Date" (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="987fa-151">Last Activity Date</span></span>
- <span data-ttu-id="987fa-152">"Used Web" (Используемое веб-приложение);</span><span class="sxs-lookup"><span data-stu-id="987fa-152">Used Web</span></span>
- <span data-ttu-id="987fa-153">"Used Windows Phone" (Используемое устройство Windows Phone);</span><span class="sxs-lookup"><span data-stu-id="987fa-153">Used Windows Phone</span></span>
- <span data-ttu-id="987fa-154">"Used Android Phone" (Используемый телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="987fa-154">Used Android Phone</span></span>
- <span data-ttu-id="987fa-155">"Used iPhone" (Используемый телефон iPhone);</span><span class="sxs-lookup"><span data-stu-id="987fa-155">Used iPhone</span></span>
- <span data-ttu-id="987fa-156">"Used iPad" (Используемое устройство iPad);</span><span class="sxs-lookup"><span data-stu-id="987fa-156">Used iPad</span></span>
- <span data-ttu-id="987fa-157">"Used Others" (Другое используемое);</span><span class="sxs-lookup"><span data-stu-id="987fa-157">Used Others</span></span>
- <span data-ttu-id="987fa-158">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="987fa-158">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="987fa-159">Пример</span><span class="sxs-lookup"><span data-stu-id="987fa-159">Example</span></span>

#### <a name="request"></a><span data-ttu-id="987fa-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="987fa-160">Request</span></span>

<span data-ttu-id="987fa-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="987fa-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerDeviceUsageUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="987fa-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="987fa-162">Response</span></span>

<span data-ttu-id="987fa-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="987fa-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="987fa-164">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="987fa-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,User State,State Change Date,Last Activity Date,Used Web,Used Windows Phone,Used Android Phone,Used iPhone,Used iPad,Used Others,Report Period
```
