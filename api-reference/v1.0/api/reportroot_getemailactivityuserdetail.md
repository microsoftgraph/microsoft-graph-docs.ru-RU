# <a name="reportroot-getemailactivityuserdetail"></a><span data-ttu-id="50989-101">reportRoot: getEmailActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="50989-101">reportRoot: getEmailActivityUserDetail</span></span>

<span data-ttu-id="50989-102">Узнайте, какие действия пользователи выполняли с электронной почтой.</span><span class="sxs-lookup"><span data-stu-id="50989-102">Get details about email activity users have performed.</span></span>

> <span data-ttu-id="50989-103">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span><span class="sxs-lookup"><span data-stu-id="50989-103">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="permissions"></a><span data-ttu-id="50989-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="50989-104">Permissions</span></span>

<span data-ttu-id="50989-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="50989-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="50989-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="50989-107">Permission type</span></span>                        | <span data-ttu-id="50989-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="50989-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="50989-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="50989-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="50989-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="50989-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="50989-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="50989-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50989-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50989-112">Not supported.</span></span>                           |
| <span data-ttu-id="50989-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="50989-113">Application</span></span>                            | <span data-ttu-id="50989-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="50989-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="50989-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="50989-115">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getEmailActivityUserDetail(period='{period_value}')
GET /reports/getEmailActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="50989-116">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="50989-116">Function parameters</span></span>

<span data-ttu-id="50989-117">В URL-адресе запроса укажите один из следующих параметров с действительным значением.</span><span class="sxs-lookup"><span data-stu-id="50989-117">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="50989-118">Параметр</span><span class="sxs-lookup"><span data-stu-id="50989-118">Parameter</span></span> | <span data-ttu-id="50989-119">Тип</span><span class="sxs-lookup"><span data-stu-id="50989-119">Type</span></span>   | <span data-ttu-id="50989-120">Описание</span><span class="sxs-lookup"><span data-stu-id="50989-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="50989-121">period</span><span class="sxs-lookup"><span data-stu-id="50989-121">period</span></span>    | <span data-ttu-id="50989-122">строка</span><span class="sxs-lookup"><span data-stu-id="50989-122">string</span></span> | <span data-ttu-id="50989-123">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="50989-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="50989-124">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="50989-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="50989-125">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="50989-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="50989-126">date</span><span class="sxs-lookup"><span data-stu-id="50989-126">date</span></span>      | <span data-ttu-id="50989-127">Дата</span><span class="sxs-lookup"><span data-stu-id="50989-127">Date</span></span>   | <span data-ttu-id="50989-128">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="50989-128">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="50989-129">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="50989-129">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="50989-130">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="50989-130">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="50989-131">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="50989-131">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="50989-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="50989-132">Request headers</span></span>

| <span data-ttu-id="50989-133">Имя</span><span class="sxs-lookup"><span data-stu-id="50989-133">Name</span></span>          | <span data-ttu-id="50989-134">Описание</span><span class="sxs-lookup"><span data-stu-id="50989-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="50989-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="50989-135">Authorization</span></span> | <span data-ttu-id="50989-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="50989-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="50989-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="50989-138">If-None-Match</span></span> | <span data-ttu-id="50989-139">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="50989-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="50989-140">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="50989-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="50989-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="50989-141">Response</span></span>

<span data-ttu-id="50989-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="50989-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="50989-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="50989-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="50989-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="50989-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="50989-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="50989-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="50989-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="50989-146">Report Refresh Date</span></span>
- <span data-ttu-id="50989-147">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="50989-147">User Principal Name</span></span>
- <span data-ttu-id="50989-148">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="50989-148">Display Name</span></span>
- <span data-ttu-id="50989-149">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="50989-149">Is Deleted</span></span>
- <span data-ttu-id="50989-150">"Deleted Date" (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="50989-150">Deleted Date</span></span>
- <span data-ttu-id="50989-151">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="50989-151">Last Activity Date</span></span>
- <span data-ttu-id="50989-152">Send Count (количество отправленных писем)</span><span class="sxs-lookup"><span data-stu-id="50989-152">Send Count</span></span>
- <span data-ttu-id="50989-153">Receive Count (количество полученных писем)</span><span class="sxs-lookup"><span data-stu-id="50989-153">Receive Count</span></span>
- <span data-ttu-id="50989-154">Read Count (количество прочитанных сообщений)</span><span class="sxs-lookup"><span data-stu-id="50989-154">Read Count</span></span>
- <span data-ttu-id="50989-155">Assigned Products (назначенные продукты)</span><span class="sxs-lookup"><span data-stu-id="50989-155">Assigned Products</span></span>
- <span data-ttu-id="50989-156">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="50989-156">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="50989-157">Пример</span><span class="sxs-lookup"><span data-stu-id="50989-157">Example</span></span>

#### <a name="request"></a><span data-ttu-id="50989-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="50989-158">Request</span></span>

<span data-ttu-id="50989-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="50989-159">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getemailactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getEmailActivityUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="50989-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="50989-160">Response</span></span>

<span data-ttu-id="50989-161">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="50989-161">The following is an example of the response.</span></span>

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

<span data-ttu-id="50989-162">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="50989-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Last Activity Date,Send Count,Receive Count,Read Count,Assigned Products,Report Period
```
