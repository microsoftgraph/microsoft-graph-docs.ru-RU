# <a name="reportroot-getyammerdeviceusagedistributionusercounts"></a><span data-ttu-id="c4f46-101">reportRoot: getYammerDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="c4f46-101">reportRoot: getYammerDeviceUsageDistributionUserCounts</span></span>

<span data-ttu-id="c4f46-102">Получите сведения о количестве пользователей с разбивкой по типам устройств.</span><span class="sxs-lookup"><span data-stu-id="c4f46-102">Get the number of users by device type.</span></span>

> <span data-ttu-id="c4f46-103">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="c4f46-103">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="c4f46-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c4f46-104">Permissions</span></span>

<span data-ttu-id="c4f46-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c4f46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="c4f46-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c4f46-107">Permission type</span></span>                        | <span data-ttu-id="c4f46-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c4f46-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="c4f46-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c4f46-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="c4f46-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c4f46-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="c4f46-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c4f46-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4f46-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4f46-112">Not supported.</span></span>                           |
| <span data-ttu-id="c4f46-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c4f46-113">Application</span></span>                            | <span data-ttu-id="c4f46-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c4f46-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="c4f46-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c4f46-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="c4f46-116">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="c4f46-116">Function parameters</span></span>

<span data-ttu-id="c4f46-117">В URL-адресе запроса укажите следующий параметр с действительным значением.</span><span class="sxs-lookup"><span data-stu-id="c4f46-117">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="c4f46-118">Параметр</span><span class="sxs-lookup"><span data-stu-id="c4f46-118">Parameter</span></span> | <span data-ttu-id="c4f46-119">Тип</span><span class="sxs-lookup"><span data-stu-id="c4f46-119">Type</span></span>   | <span data-ttu-id="c4f46-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c4f46-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="c4f46-121">period</span><span class="sxs-lookup"><span data-stu-id="c4f46-121">period</span></span>    | <span data-ttu-id="c4f46-122">строка</span><span class="sxs-lookup"><span data-stu-id="c4f46-122">string</span></span> | <span data-ttu-id="c4f46-123">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="c4f46-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="c4f46-124">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="c4f46-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="c4f46-125">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="c4f46-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="c4f46-126">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c4f46-126">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="c4f46-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c4f46-127">Request headers</span></span>

| <span data-ttu-id="c4f46-128">Имя</span><span class="sxs-lookup"><span data-stu-id="c4f46-128">Name</span></span>          | <span data-ttu-id="c4f46-129">Описание</span><span class="sxs-lookup"><span data-stu-id="c4f46-129">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="c4f46-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c4f46-130">Authorization</span></span> | <span data-ttu-id="c4f46-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c4f46-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="c4f46-133">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="c4f46-133">If-None-Match</span></span> | <span data-ttu-id="c4f46-134">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="c4f46-134">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="c4f46-135">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="c4f46-135">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="c4f46-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="c4f46-136">Response</span></span>

<span data-ttu-id="c4f46-137">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="c4f46-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="c4f46-138">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="c4f46-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="c4f46-139">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="c4f46-139">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="c4f46-140">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="c4f46-140">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="c4f46-141">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="c4f46-141">Report Refresh Date</span></span>
- <span data-ttu-id="c4f46-142">"Web" (Интернет);</span><span class="sxs-lookup"><span data-stu-id="c4f46-142">Web</span></span>
- <span data-ttu-id="c4f46-143">"Windows Phone";</span><span class="sxs-lookup"><span data-stu-id="c4f46-143">Windows Phone</span></span>
- <span data-ttu-id="c4f46-144">"Android Phone" (Телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="c4f46-144">Android Phone</span></span>
- <span data-ttu-id="c4f46-145">"iPhone";</span><span class="sxs-lookup"><span data-stu-id="c4f46-145">iPhone</span></span>
- <span data-ttu-id="c4f46-146">iPad</span><span class="sxs-lookup"><span data-stu-id="c4f46-146">iPad</span></span>
- <span data-ttu-id="c4f46-147">Other (другие)</span><span class="sxs-lookup"><span data-stu-id="c4f46-147">Other</span></span>
- <span data-ttu-id="c4f46-148">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="c4f46-148">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="c4f46-149">Пример</span><span class="sxs-lookup"><span data-stu-id="c4f46-149">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c4f46-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4f46-150">Request</span></span>

<span data-ttu-id="c4f46-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c4f46-151">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammerdeviceusagedistributionusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerDeviceUsageDistributionUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="c4f46-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="c4f46-152">Response</span></span>

<span data-ttu-id="c4f46-153">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c4f46-153">The following is an example of the response.</span></span>

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

<span data-ttu-id="c4f46-154">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="c4f46-154">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iPhone,iPad,Other,Report Period
```
