# <a name="reportroot-getsharepointsiteusagefilecounts"></a><span data-ttu-id="f8aac-101">reportRoot: getSharePointSiteUsageFileCounts</span><span class="sxs-lookup"><span data-stu-id="f8aac-101">reportRoot: getSharePointSiteUsageFileCounts</span></span>

<span data-ttu-id="f8aac-102">Узнайте, сколько всего файлов на всех сайтах и сколько из них активны.</span><span class="sxs-lookup"><span data-stu-id="f8aac-102">Get the total number of files across all sites and the number of active files.</span></span> <span data-ttu-id="f8aac-103">Файл (пользователь или система) считается активным, если он был сохранен, синхронизирован, изменен или отправлен в указанный период.</span><span class="sxs-lookup"><span data-stu-id="f8aac-103">A file (user or system) is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span>

> <span data-ttu-id="f8aac-104">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span><span class="sxs-lookup"><span data-stu-id="f8aac-104">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="f8aac-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f8aac-105">Permissions</span></span>

<span data-ttu-id="f8aac-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f8aac-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="f8aac-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f8aac-108">Permission type</span></span>                        | <span data-ttu-id="f8aac-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f8aac-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="f8aac-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f8aac-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f8aac-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8aac-111">Not supported.</span></span>                           |
| <span data-ttu-id="f8aac-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f8aac-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8aac-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8aac-113">Not supported.</span></span>                           |
| <span data-ttu-id="f8aac-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f8aac-114">Application</span></span>                            | <span data-ttu-id="f8aac-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f8aac-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="f8aac-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f8aac-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageFileCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="f8aac-117">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="f8aac-117">Request parameters</span></span>

<span data-ttu-id="f8aac-118">В URL-адресе запроса укажите следующий параметр запроса и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="f8aac-118">In the request URL, provide the following query parameter with a valid value.</span></span>

| <span data-ttu-id="f8aac-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="f8aac-119">Parameter</span></span> | <span data-ttu-id="f8aac-120">Тип</span><span class="sxs-lookup"><span data-stu-id="f8aac-120">Type</span></span>   | <span data-ttu-id="f8aac-121">Описание</span><span class="sxs-lookup"><span data-stu-id="f8aac-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="f8aac-122">period</span><span class="sxs-lookup"><span data-stu-id="f8aac-122">period</span></span>    | <span data-ttu-id="f8aac-123">строка</span><span class="sxs-lookup"><span data-stu-id="f8aac-123">string</span></span> | <span data-ttu-id="f8aac-124">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="f8aac-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="f8aac-125">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="f8aac-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="f8aac-126">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="f8aac-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="f8aac-127">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f8aac-127">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="f8aac-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f8aac-128">Request headers</span></span>

| <span data-ttu-id="f8aac-129">Имя</span><span class="sxs-lookup"><span data-stu-id="f8aac-129">Name</span></span>          | <span data-ttu-id="f8aac-130">Описание</span><span class="sxs-lookup"><span data-stu-id="f8aac-130">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="f8aac-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f8aac-131">Authorization</span></span> | <span data-ttu-id="f8aac-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f8aac-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f8aac-134">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="f8aac-134">if-none-match</span></span> | <span data-ttu-id="f8aac-135">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код ответа `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="f8aac-135">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `304 Not Modified` response is returned.</span></span> <span data-ttu-id="f8aac-136">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="f8aac-136">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="f8aac-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="f8aac-137">Response</span></span>

<span data-ttu-id="f8aac-138">В случае успешного выполнения этот метод возвращает ответ `302 Found`, который перенаправляет на URL-адрес с предварительной аутентификацией для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="f8aac-138">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="f8aac-139">Этот URL-адрес можно найти в заголовке ответа `Location`.</span><span class="sxs-lookup"><span data-stu-id="f8aac-139">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="f8aac-140">URL-адреса с предварительной аутентификацией действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="f8aac-140">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<span data-ttu-id="f8aac-141">CSV-файл содержит столбцы со следующими заголовками.</span><span class="sxs-lookup"><span data-stu-id="f8aac-141">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="f8aac-142">Report Refresh Date (дата обновления отчета)</span><span class="sxs-lookup"><span data-stu-id="f8aac-142">Report Refresh Date</span></span>
- <span data-ttu-id="f8aac-143">Site Type (тип сайта)</span><span class="sxs-lookup"><span data-stu-id="f8aac-143">Site Type</span></span>
- <span data-ttu-id="f8aac-144">Total (всего)</span><span class="sxs-lookup"><span data-stu-id="f8aac-144">total</span></span>
- <span data-ttu-id="f8aac-145">Active (активные)</span><span class="sxs-lookup"><span data-stu-id="f8aac-145">Active</span></span>
- <span data-ttu-id="f8aac-146">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="f8aac-146">Report Date</span></span>
- <span data-ttu-id="f8aac-147">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="f8aac-147">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="f8aac-148">Пример</span><span class="sxs-lookup"><span data-stu-id="f8aac-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f8aac-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="f8aac-149">Request</span></span>

<span data-ttu-id="f8aac-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f8aac-150">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagefilecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSharePointSiteUsageFileCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="f8aac-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="f8aac-151">Response</span></span>

<span data-ttu-id="f8aac-152">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f8aac-152">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="f8aac-153">Скачанный после перенаправления 302 CSV-файл будет иметь следующую схему.</span><span class="sxs-lookup"><span data-stu-id="f8aac-153">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Total,Active,Report Date,Report Period
```
