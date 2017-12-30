# <a name="reportroot-getsharepointactivityuserdetail"></a><span data-ttu-id="7736a-101">reportRoot: getSharePointActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="7736a-101">reportRoot: getSharePointActivityUserDetail</span></span>

<span data-ttu-id="7736a-102">Получите сведения об активности пользователей в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="7736a-102">Get details about SharePoint activity by user.</span></span>

> <span data-ttu-id="7736a-103">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="7736a-103">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="7736a-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7736a-104">Permissions</span></span>

<span data-ttu-id="7736a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7736a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="7736a-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7736a-107">Permission type</span></span>                        | <span data-ttu-id="7736a-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7736a-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="7736a-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7736a-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="7736a-110">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7736a-110">Not supported.</span></span>                           |
| <span data-ttu-id="7736a-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7736a-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7736a-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7736a-112">Not supported.</span></span>                           |
| <span data-ttu-id="7736a-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7736a-113">Application</span></span>                            | <span data-ttu-id="7736a-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7736a-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="7736a-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7736a-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityUserDetail(period='{period_value}')
GET /reports/getSharePointActivityUserDetail(date={date_value})
```

## <a name="request-parameters"></a><span data-ttu-id="7736a-116">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="7736a-116">Request parameters</span></span>

<span data-ttu-id="7736a-117">В URL-адресе запроса укажите выбранный параметр запроса и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="7736a-117">In the request URL, provide the chosen query parameter with a valid value.</span></span>

| <span data-ttu-id="7736a-118">Параметр</span><span class="sxs-lookup"><span data-stu-id="7736a-118">Parameter</span></span> | <span data-ttu-id="7736a-119">Тип</span><span class="sxs-lookup"><span data-stu-id="7736a-119">Type</span></span>   | <span data-ttu-id="7736a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7736a-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="7736a-121">period</span><span class="sxs-lookup"><span data-stu-id="7736a-121">period</span></span>    | <span data-ttu-id="7736a-122">строка</span><span class="sxs-lookup"><span data-stu-id="7736a-122">string</span></span> | <span data-ttu-id="7736a-123">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="7736a-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="7736a-124">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="7736a-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="7736a-125">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="7736a-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="7736a-126">date</span><span class="sxs-lookup"><span data-stu-id="7736a-126">date</span></span>      | <span data-ttu-id="7736a-127">Дата</span><span class="sxs-lookup"><span data-stu-id="7736a-127">Date</span></span>   | <span data-ttu-id="7736a-128">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="7736a-128">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="7736a-129">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="7736a-129">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="7736a-130">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="7736a-130">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="7736a-131">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="7736a-131">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7736a-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7736a-132">Request headers</span></span>

| <span data-ttu-id="7736a-133">Имя</span><span class="sxs-lookup"><span data-stu-id="7736a-133">Name</span></span>          | <span data-ttu-id="7736a-134">Описание</span><span class="sxs-lookup"><span data-stu-id="7736a-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="7736a-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7736a-135">Authorization</span></span> | <span data-ttu-id="7736a-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7736a-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7736a-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="7736a-138">if-none-match</span></span> | <span data-ttu-id="7736a-139">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="7736a-139">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `304 Not Modified` response is returned.</span></span> <span data-ttu-id="7736a-140">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="7736a-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="7736a-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="7736a-141">Response</span></span>

<span data-ttu-id="7736a-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="7736a-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="7736a-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="7736a-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="7736a-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="7736a-144">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<span data-ttu-id="7736a-145">CSV-файл содержит столбцы со следующими заголовками.</span><span class="sxs-lookup"><span data-stu-id="7736a-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="7736a-146">Report Refresh Date (дата обновления отчета)</span><span class="sxs-lookup"><span data-stu-id="7736a-146">Report Refresh Date</span></span>
- <span data-ttu-id="7736a-147">User Principal Name (имя участника-пользователя)</span><span class="sxs-lookup"><span data-stu-id="7736a-147">User Principal Name</span></span>
- <span data-ttu-id="7736a-148">Is Deleted (удален)</span><span class="sxs-lookup"><span data-stu-id="7736a-148">Is Deleted</span></span>
- <span data-ttu-id="7736a-149">Deleted Date (дата удаления)</span><span class="sxs-lookup"><span data-stu-id="7736a-149">Deleted Date</span></span>
- <span data-ttu-id="7736a-150">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="7736a-150">Last Activity Date</span></span>
- <span data-ttu-id="7736a-151">Viewed Or Edited File Count (количество просмотренных или измененных файлов)</span><span class="sxs-lookup"><span data-stu-id="7736a-151">Viewed Or Edited File Count</span></span>
- <span data-ttu-id="7736a-152">Synced File Count (количество синхронизированных файлов)</span><span class="sxs-lookup"><span data-stu-id="7736a-152">Synced File Count</span></span>
- <span data-ttu-id="7736a-153">Shared Internally File Count (количество файлов, отправленных внутренним пользователям)</span><span class="sxs-lookup"><span data-stu-id="7736a-153">Shared Internally File Count</span></span>
- <span data-ttu-id="7736a-154">Shared Externally File Count (количество файлов, отправленных за пределы организации)</span><span class="sxs-lookup"><span data-stu-id="7736a-154">Shared Externally File Count</span></span>
- <span data-ttu-id="7736a-155">Visited Page Count (количество посещенных страниц)</span><span class="sxs-lookup"><span data-stu-id="7736a-155">Visited Page Count</span></span>
- <span data-ttu-id="7736a-156">Assigned Products (назначенные продукты)</span><span class="sxs-lookup"><span data-stu-id="7736a-156">Assigned Products</span></span>
- <span data-ttu-id="7736a-157">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="7736a-157">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="7736a-158">Пример</span><span class="sxs-lookup"><span data-stu-id="7736a-158">Example</span></span>

#### <a name="request"></a><span data-ttu-id="7736a-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="7736a-159">Request</span></span>

<span data-ttu-id="7736a-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7736a-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointActivityUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="7736a-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="7736a-161">Response</span></span>

<span data-ttu-id="7736a-162">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7736a-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="7736a-163">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="7736a-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Viewed Or Edited File Count,Synced File Count,Shared Internally File Count,Shared Externally File Count,Visited Page Count,Assigned Products,Report Period
```
