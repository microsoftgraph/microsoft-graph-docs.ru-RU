# <a name="reportroot-getoffice365groupsactivitycounts"></a><span data-ttu-id="ea837-101">reportRoot: getOffice365GroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="ea837-101">reportRoot: getOffice365GroupsActivityCounts</span></span>

<span data-ttu-id="ea837-102">Узнайте, сколько различных действий было в группах.</span><span class="sxs-lookup"><span data-stu-id="ea837-102">Get the number of group activities across group workloads.</span></span>

> <span data-ttu-id="ea837-103">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="ea837-103">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="ea837-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ea837-104">Permissions</span></span>

<span data-ttu-id="ea837-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ea837-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="ea837-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ea837-107">Permission type</span></span>                        | <span data-ttu-id="ea837-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ea837-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ea837-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ea837-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="ea837-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ea837-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ea837-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ea837-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea837-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea837-112">Not supported.</span></span>                           |
| <span data-ttu-id="ea837-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ea837-113">Application</span></span>                            | <span data-ttu-id="ea837-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ea837-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="ea837-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ea837-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="ea837-116">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="ea837-116">Request parameters</span></span>

<span data-ttu-id="ea837-117">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="ea837-117">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="ea837-118">Параметр</span><span class="sxs-lookup"><span data-stu-id="ea837-118">Parameter</span></span> | <span data-ttu-id="ea837-119">Тип</span><span class="sxs-lookup"><span data-stu-id="ea837-119">Type</span></span>   | <span data-ttu-id="ea837-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ea837-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="ea837-121">period</span><span class="sxs-lookup"><span data-stu-id="ea837-121">period</span></span>    | <span data-ttu-id="ea837-122">строка</span><span class="sxs-lookup"><span data-stu-id="ea837-122">string</span></span> | <span data-ttu-id="ea837-123">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="ea837-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="ea837-124">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="ea837-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="ea837-125">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="ea837-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="ea837-126">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea837-126">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="ea837-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ea837-127">Request headers</span></span>

| <span data-ttu-id="ea837-128">Имя</span><span class="sxs-lookup"><span data-stu-id="ea837-128">Name</span></span>          | <span data-ttu-id="ea837-129">Описание</span><span class="sxs-lookup"><span data-stu-id="ea837-129">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="ea837-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ea837-130">Authorization</span></span> | <span data-ttu-id="ea837-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea837-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="ea837-133">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="ea837-133">If-None-Match</span></span> | <span data-ttu-id="ea837-134">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="ea837-134">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="ea837-135">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="ea837-135">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="ea837-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="ea837-136">Response</span></span>

<span data-ttu-id="ea837-137">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="ea837-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ea837-138">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="ea837-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ea837-139">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="ea837-139">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ea837-140">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="ea837-140">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="ea837-141">Report Refresh Date (дата обновления отчета)</span><span class="sxs-lookup"><span data-stu-id="ea837-141">Report Refresh Date</span></span>
- <span data-ttu-id="ea837-142">Exchange Emails Received (получено писем Exchange)</span><span class="sxs-lookup"><span data-stu-id="ea837-142">Exchange Emails Received</span></span>
- <span data-ttu-id="ea837-143">Yammer Messages Posted (опубликовано сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="ea837-143">Yammer Messages Posted</span></span>
- <span data-ttu-id="ea837-144">Yammer Messages Read (прочитано сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="ea837-144">Yammer Messages Read</span></span>
- <span data-ttu-id="ea837-145">Yammer Messages Liked (понравилось сообщений в Yammer)</span><span class="sxs-lookup"><span data-stu-id="ea837-145">Yammer Messages Liked</span></span>
- <span data-ttu-id="ea837-146">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="ea837-146">Report Date</span></span>
- <span data-ttu-id="ea837-147">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="ea837-147">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="ea837-148">Пример</span><span class="sxs-lookup"><span data-stu-id="ea837-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ea837-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="ea837-149">Request</span></span>

<span data-ttu-id="ea837-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ea837-150">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365groupsactivitycounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365GroupsActivityCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="ea837-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="ea837-151">Response</span></span>

<span data-ttu-id="ea837-152">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ea837-152">The following is an example of the response.</span></span>

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

<span data-ttu-id="ea837-153">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="ea837-153">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Exchange Emails Received,Yammer Messages Posted,Yammer Messages Read,Yammer Messages Liked,Report Date,Report Period
```
