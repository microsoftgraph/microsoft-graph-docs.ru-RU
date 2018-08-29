# <a name="reportroot-getteamsdeviceusagedistributionusercounts"></a><span data-ttu-id="922df-101">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="922df-101">reportRoot: getTeamsDeviceUsageDistributionUserCounts</span></span>

<span data-ttu-id="922df-102">Получение количества уникальных пользователей Microsoft Teams с сортировкой по типам устройств за выбранный период.</span><span class="sxs-lookup"><span data-stu-id="922df-102">Get the number of Microsoft Teams unique users by device type over the selected time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="922df-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="922df-103">Permissions</span></span>

<span data-ttu-id="922df-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="922df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="922df-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="922df-106">Permission type</span></span>                        | <span data-ttu-id="922df-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="922df-107">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="922df-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="922df-108">Delegated (work or school account)</span></span>     | <span data-ttu-id="922df-109">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="922df-109">Reports.Read.All</span></span>                         |
| <span data-ttu-id="922df-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="922df-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="922df-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="922df-111">Not supported.</span></span>                           |
| <span data-ttu-id="922df-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="922df-112">Application</span></span>                            | <span data-ttu-id="922df-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="922df-113">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="922df-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="922df-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageDistributionUserCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="922df-115">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="922df-115">Request parameters</span></span>

<span data-ttu-id="922df-116">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="922df-116">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="922df-117">Параметр</span><span class="sxs-lookup"><span data-stu-id="922df-117">Parameter</span></span> | <span data-ttu-id="922df-118">Тип</span><span class="sxs-lookup"><span data-stu-id="922df-118">Type</span></span>   | <span data-ttu-id="922df-119">Описание</span><span class="sxs-lookup"><span data-stu-id="922df-119">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="922df-120">period</span><span class="sxs-lookup"><span data-stu-id="922df-120">period</span></span>    | <span data-ttu-id="922df-121">строка</span><span class="sxs-lookup"><span data-stu-id="922df-121">string</span></span> | <span data-ttu-id="922df-122">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="922df-122">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="922df-123">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="922df-123">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="922df-124">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="922df-124">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="922df-125">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="922df-125">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="922df-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="922df-126">Request headers</span></span>

| <span data-ttu-id="922df-127">Имя</span><span class="sxs-lookup"><span data-stu-id="922df-127">Name</span></span>          | <span data-ttu-id="922df-128">Описание</span><span class="sxs-lookup"><span data-stu-id="922df-128">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="922df-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="922df-129">Authorization</span></span> | <span data-ttu-id="922df-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="922df-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="922df-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="922df-132">Response</span></span>

<span data-ttu-id="922df-133">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="922df-133">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="922df-134">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="922df-134">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="922df-135">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="922df-135">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="922df-136">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="922df-136">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="922df-137">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="922df-137">Report Refresh Date</span></span>
- <span data-ttu-id="922df-138">"Web" (Интернет);</span><span class="sxs-lookup"><span data-stu-id="922df-138">Web</span></span>
- <span data-ttu-id="922df-139">"Windows Phone";</span><span class="sxs-lookup"><span data-stu-id="922df-139">Windows Phone</span></span>
- <span data-ttu-id="922df-140">"Android Phone" (Телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="922df-140">Android Phone</span></span>
- <span data-ttu-id="922df-141">"iOS";</span><span class="sxs-lookup"><span data-stu-id="922df-141">iOS</span></span>
- <span data-ttu-id="922df-142">"Mac";</span><span class="sxs-lookup"><span data-stu-id="922df-142">Mac</span></span>
- <span data-ttu-id="922df-143">"Windows";</span><span class="sxs-lookup"><span data-stu-id="922df-143">Windows</span></span>
- <span data-ttu-id="922df-144">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="922df-144">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="922df-145">Пример</span><span class="sxs-lookup"><span data-stu-id="922df-145">Example</span></span>

#### <a name="request"></a><span data-ttu-id="922df-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="922df-146">Request</span></span>

<span data-ttu-id="922df-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="922df-147">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusagedistributionusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="922df-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="922df-148">Response</span></span>

<span data-ttu-id="922df-149">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="922df-149">The following is an example of the response.</span></span>

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

<span data-ttu-id="922df-150">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="922df-150">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iOS,Mac,Windows,Report Period
```
