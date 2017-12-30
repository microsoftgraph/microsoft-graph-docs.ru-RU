# <a name="reportroot-getyammergroupsactivitydetail"></a><span data-ttu-id="ddb86-101">reportRoot: getYammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="ddb86-101">reportRoot: getYammerGroupsActivityDetail</span></span>

<span data-ttu-id="ddb86-102">Получите сведения об активности в группах Yammer.</span><span class="sxs-lookup"><span data-stu-id="ddb86-102">Get details about Yammer groups activity by group.</span></span>

> <span data-ttu-id="ddb86-103">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span><span class="sxs-lookup"><span data-stu-id="ddb86-103">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="ddb86-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ddb86-104">Permissions</span></span>

<span data-ttu-id="ddb86-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ddb86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="ddb86-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ddb86-107">Permission type</span></span>                        | <span data-ttu-id="ddb86-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ddb86-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ddb86-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ddb86-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="ddb86-110">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ddb86-110">Not supported.</span></span>                           |
| <span data-ttu-id="ddb86-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ddb86-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ddb86-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ddb86-112">Not supported.</span></span>                           |
| <span data-ttu-id="ddb86-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ddb86-113">Application</span></span>                            | <span data-ttu-id="ddb86-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ddb86-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="ddb86-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ddb86-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityDetail(period='{period_value}')
GET /reports/getYammerGroupsActivityDetail(date={date_value})
```

## <a name="request-parameters"></a><span data-ttu-id="ddb86-116">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="ddb86-116">Request parameters</span></span>

<span data-ttu-id="ddb86-117">В URL-адресе запроса укажите выбранный параметр запроса и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="ddb86-117">In the request URL, provide the chosen query parameter with a valid value.</span></span>

| <span data-ttu-id="ddb86-118">Параметр</span><span class="sxs-lookup"><span data-stu-id="ddb86-118">Parameter</span></span> | <span data-ttu-id="ddb86-119">Тип</span><span class="sxs-lookup"><span data-stu-id="ddb86-119">Type</span></span>   | <span data-ttu-id="ddb86-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ddb86-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="ddb86-121">period</span><span class="sxs-lookup"><span data-stu-id="ddb86-121">period</span></span>    | <span data-ttu-id="ddb86-122">строка</span><span class="sxs-lookup"><span data-stu-id="ddb86-122">string</span></span> | <span data-ttu-id="ddb86-123">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="ddb86-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="ddb86-124">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="ddb86-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="ddb86-125">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="ddb86-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="ddb86-126">date</span><span class="sxs-lookup"><span data-stu-id="ddb86-126">date</span></span>      | <span data-ttu-id="ddb86-127">Дата</span><span class="sxs-lookup"><span data-stu-id="ddb86-127">Date</span></span>   | <span data-ttu-id="ddb86-128">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="ddb86-128">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="ddb86-129">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="ddb86-129">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="ddb86-130">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="ddb86-130">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="ddb86-131">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="ddb86-131">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ddb86-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ddb86-132">Request headers</span></span>

| <span data-ttu-id="ddb86-133">Имя</span><span class="sxs-lookup"><span data-stu-id="ddb86-133">Name</span></span>          | <span data-ttu-id="ddb86-134">Описание</span><span class="sxs-lookup"><span data-stu-id="ddb86-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="ddb86-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ddb86-135">Authorization</span></span> | <span data-ttu-id="ddb86-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ddb86-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ddb86-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="ddb86-138">if-none-match</span></span> | <span data-ttu-id="ddb86-139">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код ответа `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="ddb86-139">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `304 Not Modified` response is returned.</span></span> <span data-ttu-id="ddb86-140">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="ddb86-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="ddb86-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="ddb86-141">Response</span></span>

<span data-ttu-id="ddb86-142">В случае успешного выполнения этот метод возвращает ответ `302 Found`, который перенаправляет на URL-адрес с предварительной аутентификацией для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="ddb86-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ddb86-143">Этот URL-адрес можно найти в заголовке ответа `Location`.</span><span class="sxs-lookup"><span data-stu-id="ddb86-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ddb86-144">URL-адреса с предварительной аутентификацией действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="ddb86-144">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<span data-ttu-id="ddb86-145">CSV-файл содержит столбцы со следующими заголовками.</span><span class="sxs-lookup"><span data-stu-id="ddb86-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="ddb86-146">Report Refresh Date (дата обновления отчета)</span><span class="sxs-lookup"><span data-stu-id="ddb86-146">Report Refresh Date</span></span>
- <span data-ttu-id="ddb86-147">Group Display Name (отображаемое имя группы)</span><span class="sxs-lookup"><span data-stu-id="ddb86-147">Group Display Name</span></span>
- <span data-ttu-id="ddb86-148">Is Deleted (удален)</span><span class="sxs-lookup"><span data-stu-id="ddb86-148">Is Deleted</span></span>
- <span data-ttu-id="ddb86-149">Owner Principal Name (имя участника-владельца)</span><span class="sxs-lookup"><span data-stu-id="ddb86-149">Owner Principal Name</span></span>
- <span data-ttu-id="ddb86-150">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="ddb86-150">Last Activity Date</span></span>
- <span data-ttu-id="ddb86-151">Group Type (тип группы)</span><span class="sxs-lookup"><span data-stu-id="ddb86-151">Group Type</span></span>
- <span data-ttu-id="ddb86-152">Office 365 Connected (подключены к Office 365)</span><span class="sxs-lookup"><span data-stu-id="ddb86-152">Office 365 Connected</span></span>
- <span data-ttu-id="ddb86-153">Member Count (количество участников)</span><span class="sxs-lookup"><span data-stu-id="ddb86-153">Member Count</span></span>
- <span data-ttu-id="ddb86-154">Posted Count (количество опубликованных сообщений)</span><span class="sxs-lookup"><span data-stu-id="ddb86-154">Posted Count</span></span>
- <span data-ttu-id="ddb86-155">Read Count (количество прочитанных сообщений)</span><span class="sxs-lookup"><span data-stu-id="ddb86-155">Read Count</span></span>
- <span data-ttu-id="ddb86-156">Liked Count (количество понравившихся сообщений)</span><span class="sxs-lookup"><span data-stu-id="ddb86-156">Liked Count</span></span>
- <span data-ttu-id="ddb86-157">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="ddb86-157">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="ddb86-158">Пример</span><span class="sxs-lookup"><span data-stu-id="ddb86-158">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ddb86-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="ddb86-159">Request</span></span>

<span data-ttu-id="ddb86-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ddb86-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerGroupsActivityDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="ddb86-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="ddb86-161">Response</span></span>

<span data-ttu-id="ddb86-162">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ddb86-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="ddb86-163">Скачанный после перенаправления 302 CSV-файл будет иметь следующую схему.</span><span class="sxs-lookup"><span data-stu-id="ddb86-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Group Display Name,Is Deleted,Owner Principal Name,Last Activity Date,Group Type,Office 365 Connected,Member Count,Posted Count,Read Count,Liked Count,Report Period
```
