# <a name="reportroot-getyammerdeviceusagedistributionusercounts"></a><span data-ttu-id="90bc1-101">reportRoot: getYammerDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="90bc1-101">reportRoot: getYammerDeviceUsageDistributionUserCounts</span></span>

<span data-ttu-id="90bc1-102">Получите сведения о количестве пользователей с разбивкой по типам устройств.</span><span class="sxs-lookup"><span data-stu-id="90bc1-102">Get the number of users by device type.</span></span>

> <span data-ttu-id="90bc1-103">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span><span class="sxs-lookup"><span data-stu-id="90bc1-103">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="90bc1-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="90bc1-104">Permissions</span></span>

<span data-ttu-id="90bc1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="90bc1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="90bc1-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="90bc1-107">Permission type</span></span>                        | <span data-ttu-id="90bc1-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="90bc1-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="90bc1-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="90bc1-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="90bc1-110">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90bc1-110">Not supported.</span></span>                           |
| <span data-ttu-id="90bc1-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="90bc1-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90bc1-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90bc1-112">Not supported.</span></span>                           |
| <span data-ttu-id="90bc1-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="90bc1-113">Application</span></span>                            | <span data-ttu-id="90bc1-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="90bc1-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="90bc1-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="90bc1-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="90bc1-116">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="90bc1-116">Request parameters</span></span>

<span data-ttu-id="90bc1-117">В URL-адресе запроса укажите следующий параметр запроса и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="90bc1-117">In the request URL, provide the following query parameter with a valid value.</span></span>

| <span data-ttu-id="90bc1-118">Параметр</span><span class="sxs-lookup"><span data-stu-id="90bc1-118">Parameter</span></span> | <span data-ttu-id="90bc1-119">Тип</span><span class="sxs-lookup"><span data-stu-id="90bc1-119">Type</span></span>   | <span data-ttu-id="90bc1-120">Описание</span><span class="sxs-lookup"><span data-stu-id="90bc1-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="90bc1-121">period</span><span class="sxs-lookup"><span data-stu-id="90bc1-121">period</span></span>    | <span data-ttu-id="90bc1-122">строка</span><span class="sxs-lookup"><span data-stu-id="90bc1-122">string</span></span> | <span data-ttu-id="90bc1-123">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="90bc1-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="90bc1-124">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="90bc1-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="90bc1-125">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="90bc1-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="90bc1-126">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="90bc1-126">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="90bc1-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="90bc1-127">Request headers</span></span>

| <span data-ttu-id="90bc1-128">Имя</span><span class="sxs-lookup"><span data-stu-id="90bc1-128">Name</span></span>          | <span data-ttu-id="90bc1-129">Описание</span><span class="sxs-lookup"><span data-stu-id="90bc1-129">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="90bc1-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="90bc1-130">Authorization</span></span> | <span data-ttu-id="90bc1-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="90bc1-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="90bc1-133">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="90bc1-133">if-none-match</span></span> | <span data-ttu-id="90bc1-134">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код ответа `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="90bc1-134">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `304 Not Modified` response is returned.</span></span> <span data-ttu-id="90bc1-135">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="90bc1-135">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="90bc1-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="90bc1-136">Response</span></span>

<span data-ttu-id="90bc1-137">В случае успешного выполнения этот метод возвращает ответ `302 Found`, который перенаправляет на URL-адрес с предварительной аутентификацией для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="90bc1-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="90bc1-138">Этот URL-адрес можно найти в заголовке ответа `Location`.</span><span class="sxs-lookup"><span data-stu-id="90bc1-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="90bc1-139">URL-адреса с предварительной аутентификацией действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="90bc1-139">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<span data-ttu-id="90bc1-140">CSV-файл содержит столбцы со следующими заголовками.</span><span class="sxs-lookup"><span data-stu-id="90bc1-140">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="90bc1-141">Report Refresh Date (дата обновления отчета)</span><span class="sxs-lookup"><span data-stu-id="90bc1-141">Report Refresh Date</span></span>
- <span data-ttu-id="90bc1-142">Web (браузер)</span><span class="sxs-lookup"><span data-stu-id="90bc1-142">Web</span></span>
- <span data-ttu-id="90bc1-143">Windows Phone (телефон с Windows)</span><span class="sxs-lookup"><span data-stu-id="90bc1-143">Windows Phone</span></span>
- <span data-ttu-id="90bc1-144">Android Phone (телефон с Android)</span><span class="sxs-lookup"><span data-stu-id="90bc1-144">Office for Android Phone</span></span>
- <span data-ttu-id="90bc1-145">iPhone</span><span class="sxs-lookup"><span data-stu-id="90bc1-145">iPhone</span></span>
- <span data-ttu-id="90bc1-146">iPad</span><span class="sxs-lookup"><span data-stu-id="90bc1-146">iPad</span></span>
- <span data-ttu-id="90bc1-147">Other (другие)</span><span class="sxs-lookup"><span data-stu-id="90bc1-147">Other</span></span>
- <span data-ttu-id="90bc1-148">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="90bc1-148">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="90bc1-149">Пример</span><span class="sxs-lookup"><span data-stu-id="90bc1-149">Example</span></span>

#### <a name="request"></a><span data-ttu-id="90bc1-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="90bc1-150">Request</span></span>

<span data-ttu-id="90bc1-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="90bc1-151">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusagedistributionusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerDeviceUsageDistributionUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="90bc1-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="90bc1-152">Response</span></span>

<span data-ttu-id="90bc1-153">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="90bc1-153">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="90bc1-154">Скачанный после перенаправления 302 CSV-файл будет иметь следующую схему.</span><span class="sxs-lookup"><span data-stu-id="90bc1-154">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iPhone,iPad,Other,Report Period
```
