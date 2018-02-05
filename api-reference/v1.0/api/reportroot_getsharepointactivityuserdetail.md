# <a name="reportroot-getsharepointactivityuserdetail"></a><span data-ttu-id="b1c7b-101">reportRoot: getSharePointActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="b1c7b-101">reportRoot: getSharePointActivityUserDetail</span></span>

<span data-ttu-id="b1c7b-102">Получите сведения об активности пользователей в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b1c7b-102">Get details about SharePoint activity by user.</span></span>

> <span data-ttu-id="b1c7b-103">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="b1c7b-103">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="b1c7b-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b1c7b-104">Permissions</span></span>

<span data-ttu-id="b1c7b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b1c7b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="b1c7b-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b1c7b-107">Permission type</span></span>                        | <span data-ttu-id="b1c7b-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b1c7b-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b1c7b-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b1c7b-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="b1c7b-110">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1c7b-110">Not supported.</span></span>                           |
| <span data-ttu-id="b1c7b-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b1c7b-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1c7b-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1c7b-112">Not supported.</span></span>                           |
| <span data-ttu-id="b1c7b-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b1c7b-113">Application</span></span>                            | <span data-ttu-id="b1c7b-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b1c7b-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="b1c7b-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b1c7b-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityUserDetail(period='{period_value}')
GET /reports/getSharePointActivityUserDetail(date={date_value})
```

## <a name="request-parameters"></a><span data-ttu-id="b1c7b-116">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="b1c7b-116">Request parameters</span></span>

<span data-ttu-id="b1c7b-117">В URL-адресе запроса укажите один из следующих параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="b1c7b-117">In the request URL, provide the following query parameter with a valid value.</span></span>

| <span data-ttu-id="b1c7b-118">Параметр</span><span class="sxs-lookup"><span data-stu-id="b1c7b-118">Parameter</span></span> | <span data-ttu-id="b1c7b-119">Тип</span><span class="sxs-lookup"><span data-stu-id="b1c7b-119">Type</span></span>   | <span data-ttu-id="b1c7b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b1c7b-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b1c7b-121">period</span><span class="sxs-lookup"><span data-stu-id="b1c7b-121">period</span></span>    | <span data-ttu-id="b1c7b-122">string</span><span class="sxs-lookup"><span data-stu-id="b1c7b-122">string</span></span> | <span data-ttu-id="b1c7b-123">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="b1c7b-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b1c7b-124">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="b1c7b-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b1c7b-125">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="b1c7b-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="b1c7b-126">date</span><span class="sxs-lookup"><span data-stu-id="b1c7b-126">date</span></span>      | <span data-ttu-id="b1c7b-127">Date</span><span class="sxs-lookup"><span data-stu-id="b1c7b-127">Date</span></span>   | <span data-ttu-id="b1c7b-128">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="b1c7b-128">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="b1c7b-129">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="b1c7b-129">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="b1c7b-130">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="b1c7b-130">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="b1c7b-131">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="b1c7b-131">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b1c7b-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b1c7b-132">Request headers</span></span>

| <span data-ttu-id="b1c7b-133">Имя</span><span class="sxs-lookup"><span data-stu-id="b1c7b-133">Name</span></span>          | <span data-ttu-id="b1c7b-134">Описание</span><span class="sxs-lookup"><span data-stu-id="b1c7b-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="b1c7b-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b1c7b-135">Authorization</span></span> | <span data-ttu-id="b1c7b-p104">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1c7b-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b1c7b-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="b1c7b-138">If-None-Match</span></span> | <span data-ttu-id="b1c7b-139">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="b1c7b-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="b1c7b-140">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="b1c7b-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="b1c7b-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1c7b-141">Response</span></span>

<span data-ttu-id="b1c7b-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="b1c7b-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b1c7b-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="b1c7b-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b1c7b-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="b1c7b-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b1c7b-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="b1c7b-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b1c7b-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="b1c7b-146">Report Refresh Date</span></span>
- <span data-ttu-id="b1c7b-147">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="b1c7b-147">User Principal Name</span></span>
- <span data-ttu-id="b1c7b-148">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="b1c7b-148">Is Deleted</span></span>
- <span data-ttu-id="b1c7b-149">"Deleted Date" (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="b1c7b-149">Deleted Date</span></span>
- <span data-ttu-id="b1c7b-150">"Last Activity Date" (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="b1c7b-150">Last Activity Date</span></span>
- <span data-ttu-id="b1c7b-151">"Viewed Or Edited File Count" (Количество просмотренных или измененных файлов);</span><span class="sxs-lookup"><span data-stu-id="b1c7b-151">Viewed Or Edited File Count</span></span>
- <span data-ttu-id="b1c7b-152">"Synced File Count" (Количество синхронизированных файлов);</span><span class="sxs-lookup"><span data-stu-id="b1c7b-152">Synced File Count</span></span>
- <span data-ttu-id="b1c7b-153">"Shared Internally File Count" (Количество файлов, к которым предоставлен доступ внутренним пользователям);</span><span class="sxs-lookup"><span data-stu-id="b1c7b-153">Shared Internally File Count</span></span>
- <span data-ttu-id="b1c7b-154">Shared Externally File Count (количество файлов, отправленных за пределы организации)</span><span class="sxs-lookup"><span data-stu-id="b1c7b-154">Shared Externally File Count</span></span>
- <span data-ttu-id="b1c7b-155">Visited Page Count (количество посещенных страниц)</span><span class="sxs-lookup"><span data-stu-id="b1c7b-155">Visited Page Count</span></span>
- <span data-ttu-id="b1c7b-156">Assigned Products (назначенные продукты)</span><span class="sxs-lookup"><span data-stu-id="b1c7b-156">Assigned Products</span></span>
- <span data-ttu-id="b1c7b-157">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="b1c7b-157">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="b1c7b-158">Пример</span><span class="sxs-lookup"><span data-stu-id="b1c7b-158">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b1c7b-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1c7b-159">Request</span></span>

<span data-ttu-id="b1c7b-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b1c7b-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointActivityUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="b1c7b-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1c7b-161">Response</span></span>

<span data-ttu-id="b1c7b-162">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b1c7b-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="b1c7b-163">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="b1c7b-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
