# <a name="reportroot-getemailappusageuserdetail"></a><span data-ttu-id="dfa30-101">reportRoot: getEmailAppUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="dfa30-101">reportRoot: getEmailAppUsageUserDetail</span></span>

<span data-ttu-id="dfa30-102">Узнайте, какие действия пользователи выполняли в различных почтовых приложениях.</span><span class="sxs-lookup"><span data-stu-id="dfa30-102">Get details about which activities users performed on the various email apps.</span></span>

> <span data-ttu-id="dfa30-103">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: использование почтовых приложений](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span><span class="sxs-lookup"><span data-stu-id="dfa30-103">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="dfa30-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dfa30-104">Permissions</span></span>

<span data-ttu-id="dfa30-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="dfa30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="dfa30-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dfa30-107">Permission type</span></span>                        | <span data-ttu-id="dfa30-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dfa30-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="dfa30-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dfa30-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="dfa30-110">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dfa30-110">Not supported.</span></span>                           |
| <span data-ttu-id="dfa30-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dfa30-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dfa30-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dfa30-112">Not supported.</span></span>                           |
| <span data-ttu-id="dfa30-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dfa30-113">Application</span></span>                            | <span data-ttu-id="dfa30-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="dfa30-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="dfa30-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dfa30-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageUserDetail(period='{period_value}')
GET /reports/getEmailAppUsageUserDetail(date={date_value})
```

## <a name="request-parameters"></a><span data-ttu-id="dfa30-116">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="dfa30-116">Request parameters</span></span>

<span data-ttu-id="dfa30-117">В URL-адресе запроса укажите выбранный параметр запроса и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="dfa30-117">In the request URL, provide the chosen query parameter with a valid value.</span></span>

| <span data-ttu-id="dfa30-118">Параметр</span><span class="sxs-lookup"><span data-stu-id="dfa30-118">Parameter</span></span> | <span data-ttu-id="dfa30-119">Тип</span><span class="sxs-lookup"><span data-stu-id="dfa30-119">Type</span></span>   | <span data-ttu-id="dfa30-120">Описание</span><span class="sxs-lookup"><span data-stu-id="dfa30-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="dfa30-121">period</span><span class="sxs-lookup"><span data-stu-id="dfa30-121">period</span></span>    | <span data-ttu-id="dfa30-122">string</span><span class="sxs-lookup"><span data-stu-id="dfa30-122">string</span></span> | <span data-ttu-id="dfa30-123">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="dfa30-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="dfa30-124">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="dfa30-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="dfa30-125">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="dfa30-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="dfa30-126">date</span><span class="sxs-lookup"><span data-stu-id="dfa30-126">date</span></span>      | <span data-ttu-id="dfa30-127">Date</span><span class="sxs-lookup"><span data-stu-id="dfa30-127">Date</span></span>   | <span data-ttu-id="dfa30-128">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="dfa30-128">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="dfa30-129">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="dfa30-129">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="dfa30-130">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="dfa30-130">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="dfa30-131">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="dfa30-131">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dfa30-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dfa30-132">Request headers</span></span>

| <span data-ttu-id="dfa30-133">Имя</span><span class="sxs-lookup"><span data-stu-id="dfa30-133">Name</span></span>          | <span data-ttu-id="dfa30-134">Описание</span><span class="sxs-lookup"><span data-stu-id="dfa30-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="dfa30-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dfa30-135">Authorization</span></span> | <span data-ttu-id="dfa30-p104">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dfa30-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="dfa30-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="dfa30-138">if-none-match</span></span> | <span data-ttu-id="dfa30-139">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="dfa30-139">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `304 Not Modified` response is returned.</span></span> <span data-ttu-id="dfa30-140">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="dfa30-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="dfa30-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="dfa30-141">Response</span></span>

<span data-ttu-id="dfa30-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="dfa30-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="dfa30-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="dfa30-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="dfa30-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="dfa30-144">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<span data-ttu-id="dfa30-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="dfa30-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="dfa30-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="dfa30-146">Report Refresh Date</span></span>
- <span data-ttu-id="dfa30-147">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="dfa30-147">User Principal Name</span></span>
- <span data-ttu-id="dfa30-148">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="dfa30-148">Display Name</span></span>
- <span data-ttu-id="dfa30-149">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="dfa30-149">Is Deleted</span></span>
- <span data-ttu-id="dfa30-150">"Deleted Date" (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="dfa30-150">Deleted Date</span></span>
- <span data-ttu-id="dfa30-151">"Last Activity Date" (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="dfa30-151">Last Activity Date</span></span>
- <span data-ttu-id="dfa30-152">"Mail For Mac" (Почта для Mac);</span><span class="sxs-lookup"><span data-stu-id="dfa30-152">Mail For Mac</span></span>
- <span data-ttu-id="dfa30-153">"Outlook For Mac" (Outlook для Mac);</span><span class="sxs-lookup"><span data-stu-id="dfa30-153">Outlook for Mac</span></span>
- <span data-ttu-id="dfa30-154">"Outlook For Windows" (Outlook для Windows);</span><span class="sxs-lookup"><span data-stu-id="dfa30-154">Outlook for Windows</span></span>
- <span data-ttu-id="dfa30-155">"Outlook For Mobile" (Outlook для мобильных устройств);</span><span class="sxs-lookup"><span data-stu-id="dfa30-155">Outlook For Mobile</span></span>
- <span data-ttu-id="dfa30-156">"Other For Mobile" (Другое для мобильных устройств);</span><span class="sxs-lookup"><span data-stu-id="dfa30-156">Other For Mobile</span></span>
- <span data-ttu-id="dfa30-157">"Outlook For Web" (Outlook для браузера);</span><span class="sxs-lookup"><span data-stu-id="dfa30-157">Outlook for web</span></span>
- <span data-ttu-id="dfa30-158">"POP3 App" (Приложение с поддержкой POP3);</span><span class="sxs-lookup"><span data-stu-id="dfa30-158">POP3 App</span></span>
- <span data-ttu-id="dfa30-159">"IMAP4 App" (Приложение с поддержкой IMAP4);</span><span class="sxs-lookup"><span data-stu-id="dfa30-159">IMAP4 App</span></span>
- <span data-ttu-id="dfa30-160">"SMTP App" (Приложение с поддержкой SMTP);</span><span class="sxs-lookup"><span data-stu-id="dfa30-160">SMTP App</span></span>
- <span data-ttu-id="dfa30-161">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="dfa30-161">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="dfa30-162">Пример</span><span class="sxs-lookup"><span data-stu-id="dfa30-162">Example</span></span>

#### <a name="request"></a><span data-ttu-id="dfa30-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="dfa30-163">Request</span></span>

<span data-ttu-id="dfa30-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dfa30-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getEmailAppUsageUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="dfa30-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="dfa30-165">Response</span></span>

<span data-ttu-id="dfa30-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dfa30-166">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="dfa30-167">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="dfa30-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Last Activity Date,Mail For Mac,Outlook For Mac,Outlook For Windows,Outlook For Mobile,Other For Mobile,Outlook For Web,POP3 App,IMAP4 App,SMTP App,Report Period
```
