# <a name="reportroot-getonedriveactivityuserdetail"></a><span data-ttu-id="e6384-101">reportRoot: getOneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="e6384-101">reportRoot: getOneDriveActivityUserDetail</span></span>

<span data-ttu-id="e6384-102">Получите сведения о действиях в OneDrive с разбивкой по пользователям.</span><span class="sxs-lookup"><span data-stu-id="e6384-102">Get details about OneDrive activity by user.</span></span>

> <span data-ttu-id="e6384-103">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия в OneDrive для бизнеса](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span><span class="sxs-lookup"><span data-stu-id="e6384-103">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="permissions"></a><span data-ttu-id="e6384-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e6384-104">Permissions</span></span>

<span data-ttu-id="e6384-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e6384-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="e6384-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e6384-107">Permission type</span></span>                        | <span data-ttu-id="e6384-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e6384-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e6384-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e6384-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="e6384-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e6384-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e6384-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e6384-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6384-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6384-112">Not supported.</span></span>                           |
| <span data-ttu-id="e6384-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e6384-113">Application</span></span>                            | <span data-ttu-id="e6384-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e6384-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="e6384-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e6384-115">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOneDriveActivityUserDetail(period='{period_value}')
GET /reports/getOneDriveActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="e6384-116">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="e6384-116">Function parameters</span></span>

<span data-ttu-id="e6384-117">В URL-адресе запроса укажите один из следующих параметров с действительным значением.</span><span class="sxs-lookup"><span data-stu-id="e6384-117">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="e6384-118">Параметр</span><span class="sxs-lookup"><span data-stu-id="e6384-118">Parameter</span></span> | <span data-ttu-id="e6384-119">Тип</span><span class="sxs-lookup"><span data-stu-id="e6384-119">Type</span></span>   | <span data-ttu-id="e6384-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e6384-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="e6384-121">period</span><span class="sxs-lookup"><span data-stu-id="e6384-121">period</span></span>    | <span data-ttu-id="e6384-122">строка</span><span class="sxs-lookup"><span data-stu-id="e6384-122">string</span></span> | <span data-ttu-id="e6384-123">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="e6384-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="e6384-124">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="e6384-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="e6384-125">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="e6384-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="e6384-126">date</span><span class="sxs-lookup"><span data-stu-id="e6384-126">date</span></span>      | <span data-ttu-id="e6384-127">Дата</span><span class="sxs-lookup"><span data-stu-id="e6384-127">Date</span></span>   | <span data-ttu-id="e6384-128">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="e6384-128">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="e6384-129">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="e6384-129">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="e6384-130">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="e6384-130">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="e6384-131">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="e6384-131">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e6384-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e6384-132">Request headers</span></span>

| <span data-ttu-id="e6384-133">Имя</span><span class="sxs-lookup"><span data-stu-id="e6384-133">Name</span></span>          | <span data-ttu-id="e6384-134">Описание</span><span class="sxs-lookup"><span data-stu-id="e6384-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="e6384-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e6384-135">Authorization</span></span> | <span data-ttu-id="e6384-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e6384-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="e6384-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="e6384-138">If-None-Match</span></span> | <span data-ttu-id="e6384-139">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="e6384-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="e6384-140">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="e6384-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="e6384-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="e6384-141">Response</span></span>

<span data-ttu-id="e6384-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="e6384-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e6384-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="e6384-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e6384-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="e6384-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e6384-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="e6384-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="e6384-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="e6384-146">Report Refresh Date</span></span>
- <span data-ttu-id="e6384-147">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="e6384-147">User Principal Name</span></span>
- <span data-ttu-id="e6384-148">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="e6384-148">Is Deleted</span></span>
- <span data-ttu-id="e6384-149">"Deleted Date" (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="e6384-149">Deleted Date</span></span>
- <span data-ttu-id="e6384-150">"Last Activity Date" (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="e6384-150">Last Activity Date</span></span>
- <span data-ttu-id="e6384-151">"Viewed Or Edited File Count" (Количество просмотренных или измененных файлов);</span><span class="sxs-lookup"><span data-stu-id="e6384-151">Viewed Or Edited File Count</span></span>
- <span data-ttu-id="e6384-152">"Synced File Count" (Количество синхронизированных файлов);</span><span class="sxs-lookup"><span data-stu-id="e6384-152">Synced File Count</span></span>
- <span data-ttu-id="e6384-153">"Shared Internally File Count" (Количество файлов, к которым предоставлен доступ внутренним пользователям);</span><span class="sxs-lookup"><span data-stu-id="e6384-153">Shared Internally File Count</span></span>
- <span data-ttu-id="e6384-154">"Shared Externally File Count" (Количество файлов, к которым предоставлен доступ внешним пользователям);</span><span class="sxs-lookup"><span data-stu-id="e6384-154">Shared Externally File Count</span></span>
- <span data-ttu-id="e6384-155">"Assigned Products" (Назначенные продукты);</span><span class="sxs-lookup"><span data-stu-id="e6384-155">Assigned Products</span></span>
- <span data-ttu-id="e6384-156">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="e6384-156">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="e6384-157">Пример</span><span class="sxs-lookup"><span data-stu-id="e6384-157">Example</span></span>

#### <a name="request"></a><span data-ttu-id="e6384-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="e6384-158">Request</span></span>

<span data-ttu-id="e6384-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e6384-159">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getonedriveactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOneDriveActivityUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="e6384-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="e6384-160">Response</span></span>

<span data-ttu-id="e6384-161">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e6384-161">The following is an example of the response.</span></span>

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

<span data-ttu-id="e6384-162">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="e6384-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Viewed Or Edited File Count,Synced File Count,Shared Internally File Count,Shared Externally File Count,Assigned Products,Report Period
```
