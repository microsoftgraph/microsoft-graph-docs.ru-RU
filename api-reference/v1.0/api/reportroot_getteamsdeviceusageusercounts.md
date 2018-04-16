# <a name="reportroot-getteamsdeviceusageusercounts"></a><span data-ttu-id="14ba0-101">reportRoot: getTeamsDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="14ba0-101">reportRoot: getTeamsDeviceUsageUserCounts</span></span>

<span data-ttu-id="14ba0-102">Получение сведений о количестве уникальных пользователей Microsoft Teams в день с сортировкой по типам устройств.</span><span class="sxs-lookup"><span data-stu-id="14ba0-102">Get the number of Microsoft Teams daily unique users by device type.</span></span>

## <a name="permissions"></a><span data-ttu-id="14ba0-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="14ba0-103">Permissions</span></span>

<span data-ttu-id="14ba0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="14ba0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="14ba0-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="14ba0-106">Permission type</span></span>                        | <span data-ttu-id="14ba0-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="14ba0-107">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="14ba0-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="14ba0-108">Delegated (work or school account)</span></span>     | <span data-ttu-id="14ba0-109">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="14ba0-109">Reports.Read.All</span></span>                         |
| <span data-ttu-id="14ba0-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="14ba0-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14ba0-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14ba0-111">Not supported.</span></span>                           |
| <span data-ttu-id="14ba0-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="14ba0-112">Application</span></span>                            | <span data-ttu-id="14ba0-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="14ba0-113">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="14ba0-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="14ba0-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageUserCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="14ba0-115">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="14ba0-115">Request parameters</span></span>

<span data-ttu-id="14ba0-116">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="14ba0-116">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="14ba0-117">Параметр</span><span class="sxs-lookup"><span data-stu-id="14ba0-117">Parameter</span></span> | <span data-ttu-id="14ba0-118">Тип</span><span class="sxs-lookup"><span data-stu-id="14ba0-118">Type</span></span>   | <span data-ttu-id="14ba0-119">Описание</span><span class="sxs-lookup"><span data-stu-id="14ba0-119">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="14ba0-120">period</span><span class="sxs-lookup"><span data-stu-id="14ba0-120">period</span></span>    | <span data-ttu-id="14ba0-121">string</span><span class="sxs-lookup"><span data-stu-id="14ba0-121">string</span></span> | <span data-ttu-id="14ba0-122">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="14ba0-122">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="14ba0-123">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="14ba0-123">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="14ba0-124">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="14ba0-124">These values follow the format D   where    represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="14ba0-125">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="14ba0-125">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="14ba0-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="14ba0-126">Request headers</span></span>

| <span data-ttu-id="14ba0-127">Имя</span><span class="sxs-lookup"><span data-stu-id="14ba0-127">Name</span></span>          | <span data-ttu-id="14ba0-128">Описание</span><span class="sxs-lookup"><span data-stu-id="14ba0-128">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="14ba0-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="14ba0-129">Authorization</span></span> | <span data-ttu-id="14ba0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="14ba0-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="14ba0-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="14ba0-132">Response</span></span>

<span data-ttu-id="14ba0-133">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="14ba0-133">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="14ba0-134">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="14ba0-134">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="14ba0-135">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="14ba0-135">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="14ba0-136">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="14ba0-136">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="14ba0-137">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="14ba0-137">Report Refresh Date</span></span>
- <span data-ttu-id="14ba0-138">"Web" (Интернет);</span><span class="sxs-lookup"><span data-stu-id="14ba0-138">Web</span></span>
- <span data-ttu-id="14ba0-139">"Windows Phone";</span><span class="sxs-lookup"><span data-stu-id="14ba0-139">Windows Phone</span></span>
- <span data-ttu-id="14ba0-140">"Android Phone" (Телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="14ba0-140">Android Phone</span></span>
- <span data-ttu-id="14ba0-141">"iOS";</span><span class="sxs-lookup"><span data-stu-id="14ba0-141">iOS</span></span>
- <span data-ttu-id="14ba0-142">"Mac";</span><span class="sxs-lookup"><span data-stu-id="14ba0-142">Mac</span></span>
- <span data-ttu-id="14ba0-143">"Windows";</span><span class="sxs-lookup"><span data-stu-id="14ba0-143">Windows</span></span>
- <span data-ttu-id="14ba0-144">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="14ba0-144">Report Date</span></span>
- <span data-ttu-id="14ba0-145">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="14ba0-145">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="14ba0-146">Пример</span><span class="sxs-lookup"><span data-stu-id="14ba0-146">Example</span></span>

#### <a name="request"></a><span data-ttu-id="14ba0-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="14ba0-147">Request</span></span>

<span data-ttu-id="14ba0-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="14ba0-148">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getTeamsDeviceUsageUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="14ba0-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="14ba0-149">Response</span></span>

<span data-ttu-id="14ba0-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="14ba0-150">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="14ba0-151">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="14ba0-151">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Web,Windows Phone,Android Phone,iOS,Mac,Windows,Report Date,Report Period
```
