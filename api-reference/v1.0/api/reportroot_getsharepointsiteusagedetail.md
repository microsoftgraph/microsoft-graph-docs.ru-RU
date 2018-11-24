# <a name="reportroot-getsharepointsiteusagedetail"></a><span data-ttu-id="8d33d-101">reportRoot: getSharePointSiteUsageDetail</span><span class="sxs-lookup"><span data-stu-id="8d33d-101">reportRoot: getSharePointSiteUsageDetail</span></span>

<span data-ttu-id="8d33d-102">Получение сведений об использовании сайтов SharePoint.</span><span class="sxs-lookup"><span data-stu-id="8d33d-102">Get details about SharePoint site usage.</span></span>

> <span data-ttu-id="8d33d-103">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: использование сайтов SharePoint](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span><span class="sxs-lookup"><span data-stu-id="8d33d-103">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="8d33d-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8d33d-104">Permissions</span></span>

<span data-ttu-id="8d33d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8d33d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="8d33d-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8d33d-107">Permission type</span></span>                        | <span data-ttu-id="8d33d-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8d33d-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="8d33d-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8d33d-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="8d33d-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8d33d-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="8d33d-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8d33d-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d33d-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d33d-112">Not supported.</span></span>                           |
| <span data-ttu-id="8d33d-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8d33d-113">Application</span></span>                            | <span data-ttu-id="8d33d-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8d33d-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="8d33d-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8d33d-115">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getSharePointSiteUsageDetail(period='{period_value}')
GET /reports/getSharePointSiteUsageDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="8d33d-116">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="8d33d-116">Function parameters</span></span>

<span data-ttu-id="8d33d-117">В URL-адресе запроса укажите один из следующих параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="8d33d-117">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="8d33d-118">Параметр</span><span class="sxs-lookup"><span data-stu-id="8d33d-118">Parameter</span></span> | <span data-ttu-id="8d33d-119">Тип</span><span class="sxs-lookup"><span data-stu-id="8d33d-119">Type</span></span>   | <span data-ttu-id="8d33d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8d33d-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="8d33d-121">period</span><span class="sxs-lookup"><span data-stu-id="8d33d-121">period</span></span>    | <span data-ttu-id="8d33d-122">string</span><span class="sxs-lookup"><span data-stu-id="8d33d-122">string</span></span> | <span data-ttu-id="8d33d-123">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="8d33d-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="8d33d-124">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="8d33d-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="8d33d-125">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="8d33d-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="8d33d-126">date</span><span class="sxs-lookup"><span data-stu-id="8d33d-126">date</span></span>      | <span data-ttu-id="8d33d-127">Date</span><span class="sxs-lookup"><span data-stu-id="8d33d-127">Date</span></span>   | <span data-ttu-id="8d33d-128">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="8d33d-128">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="8d33d-129">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="8d33d-129">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="8d33d-130">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="8d33d-130">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="8d33d-131">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="8d33d-131">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8d33d-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8d33d-132">Request headers</span></span>

| <span data-ttu-id="8d33d-133">Имя</span><span class="sxs-lookup"><span data-stu-id="8d33d-133">Name</span></span>          | <span data-ttu-id="8d33d-134">Описание</span><span class="sxs-lookup"><span data-stu-id="8d33d-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="8d33d-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8d33d-135">Authorization</span></span> | <span data-ttu-id="8d33d-p104">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8d33d-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="8d33d-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="8d33d-138">If-None-Match</span></span> | <span data-ttu-id="8d33d-139">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="8d33d-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="8d33d-140">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="8d33d-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="8d33d-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d33d-141">Response</span></span>

<span data-ttu-id="8d33d-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="8d33d-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="8d33d-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="8d33d-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="8d33d-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="8d33d-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="8d33d-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="8d33d-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="8d33d-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="8d33d-146">Report Refresh Date</span></span>
- <span data-ttu-id="8d33d-147">Идентификатор сайта</span><span class="sxs-lookup"><span data-stu-id="8d33d-147">Site Id</span></span>
- <span data-ttu-id="8d33d-148">"Site URL" (URL-адрес сайта);</span><span class="sxs-lookup"><span data-stu-id="8d33d-148">Site URL</span></span>
- <span data-ttu-id="8d33d-149">"Owner Display Name" (Отображаемое имя владельца);</span><span class="sxs-lookup"><span data-stu-id="8d33d-149">Owner Display Name</span></span>
- <span data-ttu-id="8d33d-150">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="8d33d-150">Is Deleted</span></span>
- <span data-ttu-id="8d33d-151">"Last Activity Date" (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="8d33d-151">Last Activity Date</span></span>
- <span data-ttu-id="8d33d-152">"File Count" (Количество файлов);</span><span class="sxs-lookup"><span data-stu-id="8d33d-152">File Count</span></span>
- <span data-ttu-id="8d33d-153">"Active File Count" (Количество активных файлов);</span><span class="sxs-lookup"><span data-stu-id="8d33d-153">Active File Count</span></span>
- <span data-ttu-id="8d33d-154">"Page View Count" (Количество просмотров страницы);</span><span class="sxs-lookup"><span data-stu-id="8d33d-154">Page View Count</span></span>
- <span data-ttu-id="8d33d-155">"Visited Page Count" (Количество посещенных страниц);</span><span class="sxs-lookup"><span data-stu-id="8d33d-155">Visited Page Count</span></span>
- <span data-ttu-id="8d33d-156">"Storage Used (Byte)" (Используемый объем хранилища в байтах);</span><span class="sxs-lookup"><span data-stu-id="8d33d-156">Storage Used (Byte)</span></span>
- <span data-ttu-id="8d33d-157">"Storage Allocated (Byte)" (Объем выделенного хранилища в байтах);</span><span class="sxs-lookup"><span data-stu-id="8d33d-157">Storage Allocated (Byte)</span></span>
- <span data-ttu-id="8d33d-158">"Root Web Template" (Шаблон корневого веб-сайта);</span><span class="sxs-lookup"><span data-stu-id="8d33d-158">Root Web Template</span></span>
- <span data-ttu-id="8d33d-159">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="8d33d-159">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="8d33d-160">Пример</span><span class="sxs-lookup"><span data-stu-id="8d33d-160">Example</span></span>

#### <a name="request"></a><span data-ttu-id="8d33d-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d33d-161">Request</span></span>

<span data-ttu-id="8d33d-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8d33d-162">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointsiteusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointSiteUsageDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="8d33d-163">Ответ</span><span class="sxs-lookup"><span data-stu-id="8d33d-163">Response</span></span>

<span data-ttu-id="8d33d-164">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8d33d-164">The following is an example of the response.</span></span>

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

<span data-ttu-id="8d33d-165">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="8d33d-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Id,Site URL,Owner Display Name,Is Deleted,Last Activity Date,File Count,Active File Count,Page View Count,Visited Page Count,Storage Used (Byte),Storage Allocated (Byte),Root Web Template,Report Period
```
