# <a name="reportroot-getoffice365groupsactivitydetail"></a><span data-ttu-id="b4c7e-101">reportRoot: getOffice365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="b4c7e-101">reportRoot: getOffice365GroupsActivityDetail</span></span>

<span data-ttu-id="b4c7e-102">Получите сведения об активности в группах Office 365.</span><span class="sxs-lookup"><span data-stu-id="b4c7e-102">Get details about Office 365 Groups activity by group.</span></span>

> <span data-ttu-id="b4c7e-103">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="b4c7e-103">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="b4c7e-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b4c7e-104">Permissions</span></span>

<span data-ttu-id="b4c7e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b4c7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="b4c7e-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b4c7e-107">Permission type</span></span>                        | <span data-ttu-id="b4c7e-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b4c7e-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b4c7e-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b4c7e-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="b4c7e-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b4c7e-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b4c7e-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b4c7e-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4c7e-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4c7e-112">Not supported.</span></span>                           |
| <span data-ttu-id="b4c7e-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b4c7e-113">Application</span></span>                            | <span data-ttu-id="b4c7e-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b4c7e-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="b4c7e-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b4c7e-115">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOffice365GroupsActivityDetail(period='{period_value}')
GET /reports/getOffice365GroupsActivityDetail(date={date_value})
```

## <a name="request-parameters"></a><span data-ttu-id="b4c7e-116">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="b4c7e-116">Request parameters</span></span>

<span data-ttu-id="b4c7e-117">В URL-адресе запроса укажите один из следующих параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="b4c7e-117">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="b4c7e-118">Параметр</span><span class="sxs-lookup"><span data-stu-id="b4c7e-118">Parameter</span></span> | <span data-ttu-id="b4c7e-119">Тип</span><span class="sxs-lookup"><span data-stu-id="b4c7e-119">Type</span></span>   | <span data-ttu-id="b4c7e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b4c7e-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b4c7e-121">period</span><span class="sxs-lookup"><span data-stu-id="b4c7e-121">period</span></span>    | <span data-ttu-id="b4c7e-122">строка</span><span class="sxs-lookup"><span data-stu-id="b4c7e-122">string</span></span> | <span data-ttu-id="b4c7e-123">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="b4c7e-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b4c7e-124">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="b4c7e-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b4c7e-125">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="b4c7e-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="b4c7e-126">date</span><span class="sxs-lookup"><span data-stu-id="b4c7e-126">date</span></span>      | <span data-ttu-id="b4c7e-127">Date</span><span class="sxs-lookup"><span data-stu-id="b4c7e-127">Date</span></span>   | <span data-ttu-id="b4c7e-128">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="b4c7e-128">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="b4c7e-129">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="b4c7e-129">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="b4c7e-130">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="b4c7e-130">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="b4c7e-131">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="b4c7e-131">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b4c7e-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b4c7e-132">Request headers</span></span>

| <span data-ttu-id="b4c7e-133">Имя</span><span class="sxs-lookup"><span data-stu-id="b4c7e-133">Name</span></span>          | <span data-ttu-id="b4c7e-134">Описание</span><span class="sxs-lookup"><span data-stu-id="b4c7e-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="b4c7e-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b4c7e-135">Authorization</span></span> | <span data-ttu-id="b4c7e-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b4c7e-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="b4c7e-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="b4c7e-138">If-None-Match</span></span> | <span data-ttu-id="b4c7e-139">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="b4c7e-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="b4c7e-140">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="b4c7e-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="b4c7e-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="b4c7e-141">Response</span></span>

<span data-ttu-id="b4c7e-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="b4c7e-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b4c7e-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="b4c7e-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b4c7e-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="b4c7e-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b4c7e-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="b4c7e-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b4c7e-146">Report Refresh Date (дата обновления отчета)</span><span class="sxs-lookup"><span data-stu-id="b4c7e-146">Report Refresh Date</span></span>
- <span data-ttu-id="b4c7e-147">Group Display Name (отображаемое имя группы)</span><span class="sxs-lookup"><span data-stu-id="b4c7e-147">Group Display Name</span></span>
- <span data-ttu-id="b4c7e-148">Is Deleted (удален)</span><span class="sxs-lookup"><span data-stu-id="b4c7e-148">Is Deleted</span></span>
- <span data-ttu-id="b4c7e-149">Owner Principal Name (имя участника-владельца)</span><span class="sxs-lookup"><span data-stu-id="b4c7e-149">Owner Principal Name</span></span>
- <span data-ttu-id="b4c7e-150">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="b4c7e-150">Last Activity Date</span></span>
- <span data-ttu-id="b4c7e-151">Group Type (тип группы)</span><span class="sxs-lookup"><span data-stu-id="b4c7e-151">Group Type</span></span>
- <span data-ttu-id="b4c7e-152">Member Count (количество участников)</span><span class="sxs-lookup"><span data-stu-id="b4c7e-152">Member Count</span></span>
- <span data-ttu-id="b4c7e-153">External Member Count (количество внешних участников)</span><span class="sxs-lookup"><span data-stu-id="b4c7e-153">External Member Count</span></span>
- <span data-ttu-id="b4c7e-154">Exchange Received Email Count (количество полученных сообщений Exchange)</span><span class="sxs-lookup"><span data-stu-id="b4c7e-154">Exchange Received Email Count</span></span>
- <span data-ttu-id="b4c7e-155">SharePoint Active File Count (количество активных файлов SharePoint)</span><span class="sxs-lookup"><span data-stu-id="b4c7e-155">SharePoint Active File Count</span></span>
- <span data-ttu-id="b4c7e-156">Yammer Posted Message Count (количество опубликованных сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="b4c7e-156">Yammer Posted Message Count</span></span>
- <span data-ttu-id="b4c7e-157">Yammer Read Message Count (количество прочитанных сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="b4c7e-157">Yammer Read Message Count</span></span>
- <span data-ttu-id="b4c7e-158">Yammer Liked Message Count (количество понравившихся сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="b4c7e-158">Yammer Liked Message Count</span></span>
- <span data-ttu-id="b4c7e-159">Exchange Mailbox Total Item Count (общее количество элементов в почтовых ящиках Exchange)</span><span class="sxs-lookup"><span data-stu-id="b4c7e-159">Exchange Mailbox Total Item Count</span></span>
- <span data-ttu-id="b4c7e-160">Exchange Mailbox Storage Used (Byte) [занято почтовыми ящиками Exchange (байт)]</span><span class="sxs-lookup"><span data-stu-id="b4c7e-160">Exchange Mailbox Storage Used (Byte)</span></span>
- <span data-ttu-id="b4c7e-161">SharePoint Total File Count (общее количество файлов SharePoint)</span><span class="sxs-lookup"><span data-stu-id="b4c7e-161">SharePoint Total File Count</span></span>
- <span data-ttu-id="b4c7e-162">SharePoint Site Storage Used (Byte) [занято сайтами SharePoint (байт)]</span><span class="sxs-lookup"><span data-stu-id="b4c7e-162">SharePoint Site Storage Used (Byte)</span></span>
- <span data-ttu-id="b4c7e-163">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="b4c7e-163">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="b4c7e-164">Пример</span><span class="sxs-lookup"><span data-stu-id="b4c7e-164">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b4c7e-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4c7e-165">Request</span></span>

<span data-ttu-id="b4c7e-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b4c7e-166">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365groupsactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365GroupsActivityDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="b4c7e-167">Ответ</span><span class="sxs-lookup"><span data-stu-id="b4c7e-167">Response</span></span>

<span data-ttu-id="b4c7e-168">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b4c7e-168">The following is an example of the response.</span></span>

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

<span data-ttu-id="b4c7e-169">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="b4c7e-169">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Group Display Name,Is Deleted,Owner Principal Name,Last Activity Date,Group Type,Member Count,Guest Count,Exchange Received Email Count,SharePoint Active File Count,Yammer Posted Message Count,Yammer Read Message Count,Yammer Liked Message Count,Exchange Mailbox Total Item Count,Exchange Mailbox Storage Used (Byte),SharePoint Total File Count,SharePoint Site Storage Used (Byte),Report Period
```
