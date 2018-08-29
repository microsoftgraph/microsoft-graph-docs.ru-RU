# <a name="reportroot-getteamsdeviceusageuserdetail"></a><span data-ttu-id="58a61-101">reportRoot: getTeamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="58a61-101">reportRoot: getTeamsDeviceUsageUserDetail</span></span>

<span data-ttu-id="58a61-102">Получение сведений об использовании устройств Microsoft Teams по каждому пользователю.</span><span class="sxs-lookup"><span data-stu-id="58a61-102">Get details about Microsoft Teams device usage by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="58a61-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="58a61-103">Permissions</span></span>

<span data-ttu-id="58a61-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="58a61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="58a61-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="58a61-106">Permission type</span></span>                        | <span data-ttu-id="58a61-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="58a61-107">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="58a61-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="58a61-108">Delegated (work or school account)</span></span>     | <span data-ttu-id="58a61-109">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="58a61-109">Reports.Read.All</span></span>                         |
| <span data-ttu-id="58a61-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="58a61-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58a61-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58a61-111">Not supported.</span></span>                           |
| <span data-ttu-id="58a61-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="58a61-112">Application</span></span>                            | <span data-ttu-id="58a61-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="58a61-113">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="58a61-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="58a61-114">HTTP request</span></span>

<!-- { "blockType": "samples" } -->

```http
GET /reports/getTeamsDeviceUsageUserDetail(period='{period_value}')
GET /reports/getTeamsDeviceUsageUserDetail(date={date_value})
```

## <a name="request-parameters"></a><span data-ttu-id="58a61-115">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="58a61-115">Request parameters</span></span>

<span data-ttu-id="58a61-116">В URL-адресе запроса укажите один из следующих параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="58a61-116">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="58a61-117">Параметр</span><span class="sxs-lookup"><span data-stu-id="58a61-117">Parameter</span></span> | <span data-ttu-id="58a61-118">Тип</span><span class="sxs-lookup"><span data-stu-id="58a61-118">Type</span></span>   | <span data-ttu-id="58a61-119">Описание</span><span class="sxs-lookup"><span data-stu-id="58a61-119">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="58a61-120">period</span><span class="sxs-lookup"><span data-stu-id="58a61-120">period</span></span>    | <span data-ttu-id="58a61-121">строка</span><span class="sxs-lookup"><span data-stu-id="58a61-121">string</span></span> | <span data-ttu-id="58a61-122">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="58a61-122">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="58a61-123">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="58a61-123">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="58a61-124">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="58a61-124">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="58a61-125">date</span><span class="sxs-lookup"><span data-stu-id="58a61-125">date</span></span>      | <span data-ttu-id="58a61-126">Date</span><span class="sxs-lookup"><span data-stu-id="58a61-126">Date</span></span>   | <span data-ttu-id="58a61-127">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="58a61-127">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="58a61-128">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="58a61-128">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="58a61-129">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="58a61-129">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="58a61-130">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="58a61-130">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="58a61-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="58a61-131">Request headers</span></span>

| <span data-ttu-id="58a61-132">Имя</span><span class="sxs-lookup"><span data-stu-id="58a61-132">Name</span></span>          | <span data-ttu-id="58a61-133">Описание</span><span class="sxs-lookup"><span data-stu-id="58a61-133">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="58a61-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="58a61-134">Authorization</span></span> | <span data-ttu-id="58a61-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="58a61-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="58a61-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="58a61-137">Response</span></span>

<span data-ttu-id="58a61-138">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="58a61-138">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="58a61-139">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="58a61-139">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="58a61-140">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="58a61-140">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="58a61-141">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="58a61-141">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="58a61-142">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="58a61-142">Report Refresh Date</span></span>
- <span data-ttu-id="58a61-143">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="58a61-143">User Principal Name</span></span>
- <span data-ttu-id="58a61-144">Last Activity Date (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="58a61-144">Last Activity Date</span></span>
- <span data-ttu-id="58a61-145">Is Deleted (Удален);</span><span class="sxs-lookup"><span data-stu-id="58a61-145">Is Deleted</span></span>
- <span data-ttu-id="58a61-146">Deleted Date (дата удаления);</span><span class="sxs-lookup"><span data-stu-id="58a61-146">Deleted Date</span></span>
- <span data-ttu-id="58a61-147">Used Web (использовал браузер);</span><span class="sxs-lookup"><span data-stu-id="58a61-147">Used Web</span></span>
- <span data-ttu-id="58a61-148">Used Windows Phone (использовал телефон с Windows);</span><span class="sxs-lookup"><span data-stu-id="58a61-148">Used Windows Phone</span></span>
- <span data-ttu-id="58a61-149">Used iOS (использовал iOS);</span><span class="sxs-lookup"><span data-stu-id="58a61-149">Used iOS</span></span>
- <span data-ttu-id="58a61-150">Used Mac (использовал Mac);</span><span class="sxs-lookup"><span data-stu-id="58a61-150">Used Mac</span></span>
- <span data-ttu-id="58a61-151">Used Android Phone (использовал телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="58a61-151">Used Android Phone</span></span>
- <span data-ttu-id="58a61-152">Used Windows (использовал Windows);</span><span class="sxs-lookup"><span data-stu-id="58a61-152">Used Windows</span></span>
- <span data-ttu-id="58a61-153">Report Period (отчетный период).</span><span class="sxs-lookup"><span data-stu-id="58a61-153">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="58a61-154">Пример</span><span class="sxs-lookup"><span data-stu-id="58a61-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="58a61-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="58a61-155">Request</span></span>

<span data-ttu-id="58a61-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="58a61-156">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getTeamsDeviceUsageUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="58a61-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="58a61-157">Response</span></span>

<span data-ttu-id="58a61-158">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="58a61-158">The following is an example of the response.</span></span>

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

<span data-ttu-id="58a61-159">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="58a61-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Is Deleted,Deleted Date,Used Web,Used Windows Phone,Used iOS,Used Mac,Used Android Phone,Used Windows,Report Period
```
