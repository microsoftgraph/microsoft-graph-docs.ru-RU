# <a name="reportroot-getonedriveusagefilecounts"></a><span data-ttu-id="7c550-101">reportRoot: getOneDriveUsageFileCounts</span><span class="sxs-lookup"><span data-stu-id="7c550-101">reportRoot: getOneDriveUsageFileCounts</span></span>

<span data-ttu-id="7c550-102">Получение общего количества файлов на всех сайтах и количества активных файлов.</span><span class="sxs-lookup"><span data-stu-id="7c550-102">Get the total number of files across all sites and how many are active files.</span></span> <span data-ttu-id="7c550-103">Файл считается активным, если он был сохранен, синхронизирован, изменен в указанный период или им поделились в указанный период.</span><span class="sxs-lookup"><span data-stu-id="7c550-103">A file is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span>

> <span data-ttu-id="7c550-104">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: использование OneDrive для бизнеса](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span><span class="sxs-lookup"><span data-stu-id="7c550-104">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="7c550-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7c550-105">Permissions</span></span>

<span data-ttu-id="7c550-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7c550-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="7c550-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7c550-108">Permission type</span></span>                        | <span data-ttu-id="7c550-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7c550-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="7c550-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7c550-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="7c550-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c550-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="7c550-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7c550-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c550-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c550-113">Not supported.</span></span>                           |
| <span data-ttu-id="7c550-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7c550-114">Application</span></span>                            | <span data-ttu-id="7c550-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c550-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="7c550-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7c550-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="7c550-117">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="7c550-117">Function parameters</span></span>

<span data-ttu-id="7c550-118">В URL-адресе запроса укажите следующий параметр с действительным значением.</span><span class="sxs-lookup"><span data-stu-id="7c550-118">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="7c550-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="7c550-119">Parameter</span></span> | <span data-ttu-id="7c550-120">Тип</span><span class="sxs-lookup"><span data-stu-id="7c550-120">Type</span></span>   | <span data-ttu-id="7c550-121">Описание</span><span class="sxs-lookup"><span data-stu-id="7c550-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="7c550-122">period</span><span class="sxs-lookup"><span data-stu-id="7c550-122">period</span></span>    | <span data-ttu-id="7c550-123">строка</span><span class="sxs-lookup"><span data-stu-id="7c550-123">string</span></span> | <span data-ttu-id="7c550-124">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="7c550-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="7c550-125">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="7c550-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="7c550-126">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="7c550-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="7c550-127">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7c550-127">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="7c550-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7c550-128">Request headers</span></span>

| <span data-ttu-id="7c550-129">Имя</span><span class="sxs-lookup"><span data-stu-id="7c550-129">Name</span></span>          | <span data-ttu-id="7c550-130">Описание</span><span class="sxs-lookup"><span data-stu-id="7c550-130">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="7c550-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7c550-131">Authorization</span></span> | <span data-ttu-id="7c550-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7c550-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="7c550-134">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="7c550-134">If-None-Match</span></span> | <span data-ttu-id="7c550-135">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="7c550-135">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="7c550-136">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="7c550-136">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="7c550-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="7c550-137">Response</span></span>

<span data-ttu-id="7c550-138">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="7c550-138">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="7c550-139">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="7c550-139">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="7c550-140">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="7c550-140">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="7c550-141">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="7c550-141">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="7c550-142">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="7c550-142">Report Refresh Date</span></span>
- <span data-ttu-id="7c550-143">"Site Type" (Тип сайта);</span><span class="sxs-lookup"><span data-stu-id="7c550-143">Site Type</span></span>
- <span data-ttu-id="7c550-144">Total (всего)</span><span class="sxs-lookup"><span data-stu-id="7c550-144">Total</span></span>
- <span data-ttu-id="7c550-145">Active (активные)</span><span class="sxs-lookup"><span data-stu-id="7c550-145">Active</span></span>
- <span data-ttu-id="7c550-146">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="7c550-146">Report Date</span></span>
- <span data-ttu-id="7c550-147">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="7c550-147">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="7c550-148">Пример</span><span class="sxs-lookup"><span data-stu-id="7c550-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="7c550-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="7c550-149">Request</span></span>

<span data-ttu-id="7c550-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7c550-150">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getonedriveusagefilecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOneDriveUsageFileCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="7c550-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="7c550-151">Response</span></span>

<span data-ttu-id="7c550-152">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7c550-152">The following is an example of the response.</span></span>

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

<span data-ttu-id="7c550-153">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="7c550-153">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Total,Active,Report Date,Report Period
```
