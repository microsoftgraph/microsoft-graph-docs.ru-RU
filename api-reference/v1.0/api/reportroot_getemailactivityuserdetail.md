# <a name="reportroot-getemailactivityuserdetail"></a><span data-ttu-id="fe00d-101">reportRoot: getEmailActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="fe00d-101">reportRoot: getEmailActivityUserDetail</span></span>

<span data-ttu-id="fe00d-102">Узнайте, какие действия пользователи выполняли с электронной почтой.</span><span class="sxs-lookup"><span data-stu-id="fe00d-102">Get details about email activity users have performed.</span></span>

> <span data-ttu-id="fe00d-103">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span><span class="sxs-lookup"><span data-stu-id="fe00d-103">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="permissions"></a><span data-ttu-id="fe00d-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fe00d-104">Permissions</span></span>

<span data-ttu-id="fe00d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fe00d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="fe00d-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fe00d-107">Permission type</span></span>                        | <span data-ttu-id="fe00d-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fe00d-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="fe00d-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fe00d-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="fe00d-110">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe00d-110">Not supported.</span></span>                           |
| <span data-ttu-id="fe00d-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fe00d-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe00d-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe00d-112">Not supported.</span></span>                           |
| <span data-ttu-id="fe00d-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fe00d-113">Application</span></span>                            | <span data-ttu-id="fe00d-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fe00d-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="fe00d-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fe00d-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailActivityUserDetail(period='{period_value}')
GET /reports/getEmailActivityUserDetail(date={date_value})
```

## <a name="request-parameters"></a><span data-ttu-id="fe00d-116">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="fe00d-116">Request parameters</span></span>

<span data-ttu-id="fe00d-117">В URL-адресе запроса укажите один из следующих параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="fe00d-117">In the request URL, provide the following query parameter with a valid value.</span></span>

| <span data-ttu-id="fe00d-118">Параметр</span><span class="sxs-lookup"><span data-stu-id="fe00d-118">Parameter</span></span> | <span data-ttu-id="fe00d-119">Тип</span><span class="sxs-lookup"><span data-stu-id="fe00d-119">Type</span></span>   | <span data-ttu-id="fe00d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="fe00d-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="fe00d-121">period</span><span class="sxs-lookup"><span data-stu-id="fe00d-121">period</span></span>    | <span data-ttu-id="fe00d-122">string</span><span class="sxs-lookup"><span data-stu-id="fe00d-122">string</span></span> | <span data-ttu-id="fe00d-123">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="fe00d-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="fe00d-124">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="fe00d-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="fe00d-125">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="fe00d-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="fe00d-126">date</span><span class="sxs-lookup"><span data-stu-id="fe00d-126">date</span></span>      | <span data-ttu-id="fe00d-127">Date</span><span class="sxs-lookup"><span data-stu-id="fe00d-127">Date</span></span>   | <span data-ttu-id="fe00d-128">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="fe00d-128">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="fe00d-129">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="fe00d-129">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="fe00d-130">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="fe00d-130">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="fe00d-131">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="fe00d-131">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fe00d-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fe00d-132">Request headers</span></span>

| <span data-ttu-id="fe00d-133">Имя</span><span class="sxs-lookup"><span data-stu-id="fe00d-133">Name</span></span>          | <span data-ttu-id="fe00d-134">Описание</span><span class="sxs-lookup"><span data-stu-id="fe00d-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="fe00d-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fe00d-135">Authorization</span></span> | <span data-ttu-id="fe00d-p104">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fe00d-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="fe00d-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="fe00d-138">If-None-Match</span></span> | <span data-ttu-id="fe00d-139">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="fe00d-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="fe00d-140">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="fe00d-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="fe00d-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe00d-141">Response</span></span>

<span data-ttu-id="fe00d-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="fe00d-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="fe00d-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="fe00d-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="fe00d-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="fe00d-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="fe00d-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="fe00d-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="fe00d-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="fe00d-146">Report Refresh Date</span></span>
- <span data-ttu-id="fe00d-147">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="fe00d-147">User Principal Name</span></span>
- <span data-ttu-id="fe00d-148">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="fe00d-148">Display Name</span></span>
- <span data-ttu-id="fe00d-149">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="fe00d-149">Is Deleted</span></span>
- <span data-ttu-id="fe00d-150">"Deleted Date" (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="fe00d-150">Deleted Date</span></span>
- <span data-ttu-id="fe00d-151">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="fe00d-151">Last Activity Date</span></span>
- <span data-ttu-id="fe00d-152">Send Count (количество отправленных писем)</span><span class="sxs-lookup"><span data-stu-id="fe00d-152">Send Count</span></span>
- <span data-ttu-id="fe00d-153">Receive Count (количество полученных писем)</span><span class="sxs-lookup"><span data-stu-id="fe00d-153">Receive Count</span></span>
- <span data-ttu-id="fe00d-154">Read Count (количество прочитанных сообщений)</span><span class="sxs-lookup"><span data-stu-id="fe00d-154">Read Count</span></span>
- <span data-ttu-id="fe00d-155">Assigned Products (назначенные продукты)</span><span class="sxs-lookup"><span data-stu-id="fe00d-155">Assigned Products</span></span>
- <span data-ttu-id="fe00d-156">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="fe00d-156">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="fe00d-157">Пример</span><span class="sxs-lookup"><span data-stu-id="fe00d-157">Example</span></span>

#### <a name="request"></a><span data-ttu-id="fe00d-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="fe00d-158">Request</span></span>

<span data-ttu-id="fe00d-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fe00d-159">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getEmailActivityUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="fe00d-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe00d-160">Response</span></span>

<span data-ttu-id="fe00d-161">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fe00d-161">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="fe00d-162">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="fe00d-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Last Activity Date,Send Count,Receive Count,Read Count,Assigned Products,Report Period
```
