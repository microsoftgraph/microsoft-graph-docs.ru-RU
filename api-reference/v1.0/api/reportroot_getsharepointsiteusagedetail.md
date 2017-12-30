# <a name="reportroot-getsharepointsiteusagedetail"></a><span data-ttu-id="5fbf2-101">reportRoot: getSharePointSiteUsageDetail</span><span class="sxs-lookup"><span data-stu-id="5fbf2-101">reportRoot: getSharePointSiteUsageDetail</span></span>

<span data-ttu-id="5fbf2-102">Получение сведений об использовании сайтов SharePoint.</span><span class="sxs-lookup"><span data-stu-id="5fbf2-102">Get details about SharePoint site usage.</span></span>

> <span data-ttu-id="5fbf2-103">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: использование сайтов SharePoint](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span><span class="sxs-lookup"><span data-stu-id="5fbf2-103">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="5fbf2-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5fbf2-104">Permissions</span></span>

<span data-ttu-id="5fbf2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5fbf2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="5fbf2-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5fbf2-107">Permission type</span></span>                        | <span data-ttu-id="5fbf2-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5fbf2-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="5fbf2-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5fbf2-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="5fbf2-110">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5fbf2-110">Not supported.</span></span>                           |
| <span data-ttu-id="5fbf2-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5fbf2-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5fbf2-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5fbf2-112">Not supported.</span></span>                           |
| <span data-ttu-id="5fbf2-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5fbf2-113">Application</span></span>                            | <span data-ttu-id="5fbf2-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5fbf2-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="5fbf2-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5fbf2-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageDetail(period='{period_value}')
GET /reports/getSharePointSiteUsageDetail(date={date_value})
```

## <a name="request-parameters"></a><span data-ttu-id="5fbf2-116">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="5fbf2-116">Request parameters</span></span>

<span data-ttu-id="5fbf2-117">В URL-адресе запроса укажите выбранный параметр запроса и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="5fbf2-117">In the request URL, provide the chosen query parameter with a valid value.</span></span>

| <span data-ttu-id="5fbf2-118">Параметр</span><span class="sxs-lookup"><span data-stu-id="5fbf2-118">Parameter</span></span> | <span data-ttu-id="5fbf2-119">Тип</span><span class="sxs-lookup"><span data-stu-id="5fbf2-119">Type</span></span>   | <span data-ttu-id="5fbf2-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5fbf2-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="5fbf2-121">period</span><span class="sxs-lookup"><span data-stu-id="5fbf2-121">period</span></span>    | <span data-ttu-id="5fbf2-122">string</span><span class="sxs-lookup"><span data-stu-id="5fbf2-122">string</span></span> | <span data-ttu-id="5fbf2-123">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="5fbf2-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="5fbf2-124">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="5fbf2-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="5fbf2-125">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="5fbf2-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="5fbf2-126">date</span><span class="sxs-lookup"><span data-stu-id="5fbf2-126">date</span></span>      | <span data-ttu-id="5fbf2-127">Date</span><span class="sxs-lookup"><span data-stu-id="5fbf2-127">Date</span></span>   | <span data-ttu-id="5fbf2-128">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="5fbf2-128">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="5fbf2-129">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="5fbf2-129">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="5fbf2-130">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="5fbf2-130">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="5fbf2-131">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="5fbf2-131">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5fbf2-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5fbf2-132">Request headers</span></span>

| <span data-ttu-id="5fbf2-133">Имя</span><span class="sxs-lookup"><span data-stu-id="5fbf2-133">Name</span></span>          | <span data-ttu-id="5fbf2-134">Описание</span><span class="sxs-lookup"><span data-stu-id="5fbf2-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="5fbf2-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5fbf2-135">Authorization</span></span> | <span data-ttu-id="5fbf2-p104">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5fbf2-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5fbf2-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="5fbf2-138">if-none-match</span></span> | <span data-ttu-id="5fbf2-139">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="5fbf2-139">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `304 Not Modified` response is returned.</span></span> <span data-ttu-id="5fbf2-140">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="5fbf2-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="5fbf2-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="5fbf2-141">Response</span></span>

<span data-ttu-id="5fbf2-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="5fbf2-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="5fbf2-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="5fbf2-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="5fbf2-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="5fbf2-144">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<span data-ttu-id="5fbf2-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="5fbf2-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="5fbf2-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="5fbf2-146">Report Refresh Date</span></span>
- <span data-ttu-id="5fbf2-147">"Site URL" (URL-адрес сайта);</span><span class="sxs-lookup"><span data-stu-id="5fbf2-147">Site URL</span></span>
- <span data-ttu-id="5fbf2-148">"Owner Display Name" (Отображаемое имя владельца);</span><span class="sxs-lookup"><span data-stu-id="5fbf2-148">Owner Display Name</span></span>
- <span data-ttu-id="5fbf2-149">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="5fbf2-149">Is Deleted</span></span>
- <span data-ttu-id="5fbf2-150">"Last Activity Date" (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="5fbf2-150">Last Activity Date</span></span>
- <span data-ttu-id="5fbf2-151">"File Count" (Количество файлов);</span><span class="sxs-lookup"><span data-stu-id="5fbf2-151">File Count</span></span>
- <span data-ttu-id="5fbf2-152">"Active File Count" (Количество активных файлов);</span><span class="sxs-lookup"><span data-stu-id="5fbf2-152">Active File Count</span></span>
- <span data-ttu-id="5fbf2-153">"Page View Count" (Количество просмотров страницы);</span><span class="sxs-lookup"><span data-stu-id="5fbf2-153">Page View Count</span></span>
- <span data-ttu-id="5fbf2-154">"Visited Page Count" (Количество посещенных страниц);</span><span class="sxs-lookup"><span data-stu-id="5fbf2-154">Visited Page Count</span></span>
- <span data-ttu-id="5fbf2-155">"Storage Used (Byte)" (Используемый объем хранилища в байтах);</span><span class="sxs-lookup"><span data-stu-id="5fbf2-155">Storage Used (Byte)</span></span>
- <span data-ttu-id="5fbf2-156">"Storage Allocated (Byte)" (Объем выделенного хранилища в байтах);</span><span class="sxs-lookup"><span data-stu-id="5fbf2-156">Storage Allocated (Byte)</span></span>
- <span data-ttu-id="5fbf2-157">"Root Web Template" (Шаблон корневого веб-сайта);</span><span class="sxs-lookup"><span data-stu-id="5fbf2-157">Root Web Template</span></span>
- <span data-ttu-id="5fbf2-158">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="5fbf2-158">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="5fbf2-159">Пример</span><span class="sxs-lookup"><span data-stu-id="5fbf2-159">Example</span></span>

#### <a name="request"></a><span data-ttu-id="5fbf2-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="5fbf2-160">Request</span></span>

<span data-ttu-id="5fbf2-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5fbf2-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointSiteUsageDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="5fbf2-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="5fbf2-162">Response</span></span>

<span data-ttu-id="5fbf2-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5fbf2-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="5fbf2-164">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="5fbf2-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site URL,Owner Display Name,Is Deleted,Last Activity Date,File Count,Active File Count,Page View Count,Visited Page Count,Storage Used (Byte),Storage Allocated (Byte),Root Web Template,Report Period
```
