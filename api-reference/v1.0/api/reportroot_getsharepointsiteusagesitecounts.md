# <a name="reportroot-getsharepointsiteusagesitecounts"></a><span data-ttu-id="3bf56-101">reportRoot: getSharePointSiteUsageSiteCounts</span><span class="sxs-lookup"><span data-stu-id="3bf56-101">reportRoot: getSharePointSiteUsageSiteCounts</span></span>

<span data-ttu-id="3bf56-102">Узнайте, сколько всего файлов на всех сайтах и сколько из них активны.</span><span class="sxs-lookup"><span data-stu-id="3bf56-102">Get the total number of files across all sites and the number of active files.</span></span> <span data-ttu-id="3bf56-103">Файл (пользователь или система) считается активным, если он был сохранен, синхронизирован, изменен в указанный период или им поделились в указанный период.</span><span class="sxs-lookup"><span data-stu-id="3bf56-103">A file (user or system) is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span>

> <span data-ttu-id="3bf56-104">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: использование сайтов SharePoint](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span><span class="sxs-lookup"><span data-stu-id="3bf56-104">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="3bf56-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3bf56-105">Permissions</span></span>

<span data-ttu-id="3bf56-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3bf56-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="3bf56-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3bf56-108">Permission type</span></span>                        | <span data-ttu-id="3bf56-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3bf56-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="3bf56-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3bf56-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="3bf56-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3bf56-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="3bf56-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3bf56-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3bf56-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3bf56-113">Not supported.</span></span>                           |
| <span data-ttu-id="3bf56-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3bf56-114">Application</span></span>                            | <span data-ttu-id="3bf56-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3bf56-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="3bf56-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3bf56-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageSiteCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="3bf56-117">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="3bf56-117">Request parameters</span></span>

<span data-ttu-id="3bf56-118">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="3bf56-118">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="3bf56-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="3bf56-119">Parameter</span></span> | <span data-ttu-id="3bf56-120">Тип</span><span class="sxs-lookup"><span data-stu-id="3bf56-120">Type</span></span>   | <span data-ttu-id="3bf56-121">Описание</span><span class="sxs-lookup"><span data-stu-id="3bf56-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="3bf56-122">period</span><span class="sxs-lookup"><span data-stu-id="3bf56-122">period</span></span>    | <span data-ttu-id="3bf56-123">строка</span><span class="sxs-lookup"><span data-stu-id="3bf56-123">string</span></span> | <span data-ttu-id="3bf56-124">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="3bf56-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="3bf56-125">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="3bf56-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="3bf56-126">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="3bf56-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="3bf56-127">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3bf56-127">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="3bf56-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3bf56-128">Request headers</span></span>

| <span data-ttu-id="3bf56-129">Имя</span><span class="sxs-lookup"><span data-stu-id="3bf56-129">Name</span></span>          | <span data-ttu-id="3bf56-130">Описание</span><span class="sxs-lookup"><span data-stu-id="3bf56-130">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="3bf56-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3bf56-131">Authorization</span></span> | <span data-ttu-id="3bf56-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3bf56-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="3bf56-134">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="3bf56-134">If-None-Match</span></span> | <span data-ttu-id="3bf56-135">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="3bf56-135">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="3bf56-136">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="3bf56-136">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="3bf56-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="3bf56-137">Response</span></span>

<span data-ttu-id="3bf56-138">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="3bf56-138">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="3bf56-139">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="3bf56-139">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="3bf56-140">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="3bf56-140">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="3bf56-141">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="3bf56-141">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="3bf56-142">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="3bf56-142">Report Refresh Date</span></span>
- <span data-ttu-id="3bf56-143">"Site Type" (Тип сайта);</span><span class="sxs-lookup"><span data-stu-id="3bf56-143">Site Type</span></span>
- <span data-ttu-id="3bf56-144">Total (всего)</span><span class="sxs-lookup"><span data-stu-id="3bf56-144">Total</span></span>
- <span data-ttu-id="3bf56-145">Active (активные)</span><span class="sxs-lookup"><span data-stu-id="3bf56-145">Active</span></span>
- <span data-ttu-id="3bf56-146">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="3bf56-146">Report Date</span></span>
- <span data-ttu-id="3bf56-147">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="3bf56-147">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="3bf56-148">Пример</span><span class="sxs-lookup"><span data-stu-id="3bf56-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="3bf56-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="3bf56-149">Request</span></span>

<span data-ttu-id="3bf56-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3bf56-150">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointsiteusagesitecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointSiteUsageSiteCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="3bf56-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="3bf56-151">Response</span></span>

<span data-ttu-id="3bf56-152">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3bf56-152">The following is an example of the response.</span></span>

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

<span data-ttu-id="3bf56-153">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="3bf56-153">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Total,Active,Report Date,Report Period
```
