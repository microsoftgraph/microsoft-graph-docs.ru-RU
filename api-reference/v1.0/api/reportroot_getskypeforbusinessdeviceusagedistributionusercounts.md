# <a name="reportroot-getskypeforbusinessdeviceusagedistributionusercounts"></a><span data-ttu-id="313b2-101">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="313b2-101">reportRoot: getSkypeForBusinessDeviceUsageDistributionUserCounts</span></span>

<span data-ttu-id="313b2-102">Узнайте, сколько сотрудников организации используют уникальные устройства.</span><span class="sxs-lookup"><span data-stu-id="313b2-102">Get the number of users using unique devices in your organization.</span></span> <span data-ttu-id="313b2-103">В отчете будет показано количество пользователей Windows, телефонов с Windows, телефонов с Android, iPhone и iPad.</span><span class="sxs-lookup"><span data-stu-id="313b2-103">The report will show you the number of users per device including Windows, Windows phone, Android phone, iPhone, and iPad.</span></span>

> <span data-ttu-id="313b2-104">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span><span class="sxs-lookup"><span data-stu-id="313b2-104">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="313b2-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="313b2-105">Permissions</span></span>

<span data-ttu-id="313b2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="313b2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="313b2-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="313b2-108">Permission type</span></span>                        | <span data-ttu-id="313b2-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="313b2-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="313b2-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="313b2-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="313b2-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="313b2-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="313b2-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="313b2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="313b2-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="313b2-113">Not supported.</span></span>                           |
| <span data-ttu-id="313b2-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="313b2-114">Application</span></span>                            | <span data-ttu-id="313b2-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="313b2-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="313b2-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="313b2-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="313b2-117">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="313b2-117">Request parameters</span></span>

<span data-ttu-id="313b2-118">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="313b2-118">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="313b2-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="313b2-119">Parameter</span></span> | <span data-ttu-id="313b2-120">Тип</span><span class="sxs-lookup"><span data-stu-id="313b2-120">Type</span></span>   | <span data-ttu-id="313b2-121">Описание</span><span class="sxs-lookup"><span data-stu-id="313b2-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="313b2-122">period</span><span class="sxs-lookup"><span data-stu-id="313b2-122">period</span></span>    | <span data-ttu-id="313b2-123">строка</span><span class="sxs-lookup"><span data-stu-id="313b2-123">string</span></span> | <span data-ttu-id="313b2-124">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="313b2-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="313b2-125">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="313b2-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="313b2-126">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="313b2-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="313b2-127">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="313b2-127">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="313b2-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="313b2-128">Request headers</span></span>

| <span data-ttu-id="313b2-129">Имя</span><span class="sxs-lookup"><span data-stu-id="313b2-129">Name</span></span>          | <span data-ttu-id="313b2-130">Описание</span><span class="sxs-lookup"><span data-stu-id="313b2-130">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="313b2-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="313b2-131">Authorization</span></span> | <span data-ttu-id="313b2-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="313b2-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="313b2-134">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="313b2-134">If-None-Match</span></span> | <span data-ttu-id="313b2-135">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="313b2-135">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="313b2-136">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="313b2-136">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="313b2-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="313b2-137">Response</span></span>

<span data-ttu-id="313b2-138">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="313b2-138">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="313b2-139">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="313b2-139">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="313b2-140">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="313b2-140">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="313b2-141">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="313b2-141">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="313b2-142">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="313b2-142">Report Refresh Date</span></span>
- <span data-ttu-id="313b2-143">"Windows";</span><span class="sxs-lookup"><span data-stu-id="313b2-143">Windows</span></span>
- <span data-ttu-id="313b2-144">"Windows Phone";</span><span class="sxs-lookup"><span data-stu-id="313b2-144">Windows Phone</span></span>
- <span data-ttu-id="313b2-145">"Android Phone" (Телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="313b2-145">Android Phone</span></span>
- <span data-ttu-id="313b2-146">"iPhone";</span><span class="sxs-lookup"><span data-stu-id="313b2-146">iPhone</span></span>
- <span data-ttu-id="313b2-147">iPad</span><span class="sxs-lookup"><span data-stu-id="313b2-147">iPad</span></span>
- <span data-ttu-id="313b2-148">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="313b2-148">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="313b2-149">Пример</span><span class="sxs-lookup"><span data-stu-id="313b2-149">Example</span></span>

#### <a name="request"></a><span data-ttu-id="313b2-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="313b2-150">Request</span></span>

<span data-ttu-id="313b2-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="313b2-151">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinessdeviceusagedistributionusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="313b2-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="313b2-152">Response</span></span>

<span data-ttu-id="313b2-153">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="313b2-153">The following is an example of the response.</span></span>

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

<span data-ttu-id="313b2-154">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="313b2-154">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Windows,Windows Phone,Android Phone,iPhone,iPad,Report Period
```
