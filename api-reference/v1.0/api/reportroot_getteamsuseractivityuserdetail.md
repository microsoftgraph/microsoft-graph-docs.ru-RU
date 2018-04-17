# <a name="reportroot-getteamsuseractivityuserdetail"></a><span data-ttu-id="b67ad-101">reportRoot: getTeamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="b67ad-101">reportRoot: getTeamsUserActivityUserDetail</span></span>

<span data-ttu-id="b67ad-102">Получение сведения о действиях отдельных пользователей Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="b67ad-102">Get details about Microsoft Teams user activity by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="b67ad-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b67ad-103">Permissions</span></span>

<span data-ttu-id="b67ad-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b67ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="b67ad-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b67ad-106">Permission type</span></span>                        | <span data-ttu-id="b67ad-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b67ad-107">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b67ad-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b67ad-108">Delegated (work or school account)</span></span>     | <span data-ttu-id="b67ad-109">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b67ad-109">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b67ad-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b67ad-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b67ad-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b67ad-111">Not supported.</span></span>                           |
| <span data-ttu-id="b67ad-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b67ad-112">Application</span></span>                            | <span data-ttu-id="b67ad-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b67ad-113">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="b67ad-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b67ad-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserDetail(period='{period_value}')
GET /reports/getTeamsUserActivityUserDetail(date={date_value})
```

## <a name="request-parameters"></a><span data-ttu-id="b67ad-115">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="b67ad-115">Request parameters</span></span>

<span data-ttu-id="b67ad-116">В URL-адресе запроса укажите один из следующих параметров и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="b67ad-116">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="b67ad-117">Параметр</span><span class="sxs-lookup"><span data-stu-id="b67ad-117">Parameter</span></span> | <span data-ttu-id="b67ad-118">Тип</span><span class="sxs-lookup"><span data-stu-id="b67ad-118">Type</span></span>   | <span data-ttu-id="b67ad-119">Описание</span><span class="sxs-lookup"><span data-stu-id="b67ad-119">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b67ad-120">period</span><span class="sxs-lookup"><span data-stu-id="b67ad-120">period</span></span>    | <span data-ttu-id="b67ad-121">string</span><span class="sxs-lookup"><span data-stu-id="b67ad-121">string</span></span> | <span data-ttu-id="b67ad-122">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="b67ad-122">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b67ad-123">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="b67ad-123">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b67ad-124">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="b67ad-124">These values follow the format D   where    represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="b67ad-125">date</span><span class="sxs-lookup"><span data-stu-id="b67ad-125">date</span></span>      | <span data-ttu-id="b67ad-126">Date</span><span class="sxs-lookup"><span data-stu-id="b67ad-126">Date</span></span>   | <span data-ttu-id="b67ad-127">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="b67ad-127">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="b67ad-128">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="b67ad-128">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="b67ad-129">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="b67ad-129">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="b67ad-130">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="b67ad-130">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b67ad-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b67ad-131">Request headers</span></span>

| <span data-ttu-id="b67ad-132">Имя</span><span class="sxs-lookup"><span data-stu-id="b67ad-132">Name</span></span>          | <span data-ttu-id="b67ad-133">Описание</span><span class="sxs-lookup"><span data-stu-id="b67ad-133">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="b67ad-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b67ad-134">Authorization</span></span> | <span data-ttu-id="b67ad-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b67ad-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="b67ad-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="b67ad-137">Response</span></span>

<span data-ttu-id="b67ad-138">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="b67ad-138">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b67ad-139">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="b67ad-139">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b67ad-140">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="b67ad-140">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b67ad-141">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="b67ad-141">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="b67ad-142">Report Refresh Date (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="b67ad-142">Report Refresh Date</span></span>
- <span data-ttu-id="b67ad-143">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="b67ad-143">User Principal Name</span></span>
- <span data-ttu-id="b67ad-144">Last Activity Date (Дата последнего действия);</span><span class="sxs-lookup"><span data-stu-id="b67ad-144">Last Activity Date</span></span>
- <span data-ttu-id="b67ad-145">Is Deleted (Удален);</span><span class="sxs-lookup"><span data-stu-id="b67ad-145">Is Deleted</span></span>
- <span data-ttu-id="b67ad-146">Deleted Date (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="b67ad-146">Deleted Date</span></span>
- <span data-ttu-id="b67ad-147">Assigned Products (Назначенные продукты);</span><span class="sxs-lookup"><span data-stu-id="b67ad-147">Assigned Products</span></span>
- <span data-ttu-id="b67ad-148">Team Chat Messages Count (Количество сообщений в чатах групп);</span><span class="sxs-lookup"><span data-stu-id="b67ad-148">Team Chat Message Count</span></span>
- <span data-ttu-id="b67ad-149">Private Chat Message Count (Количество сообщений в приватных чатах);</span><span class="sxs-lookup"><span data-stu-id="b67ad-149">Private Chat Message Count</span></span>
- <span data-ttu-id="b67ad-150">Call Count (Количество звонков);</span><span class="sxs-lookup"><span data-stu-id="b67ad-150">Call Count</span></span>
- <span data-ttu-id="b67ad-151">Meeting Count (Количество собраний);</span><span class="sxs-lookup"><span data-stu-id="b67ad-151">Meeting Count</span></span>
- <span data-ttu-id="b67ad-152">Has Other Action (Есть другое действие);</span><span class="sxs-lookup"><span data-stu-id="b67ad-152">Has Other Action</span></span>
- <span data-ttu-id="b67ad-153">Report Period (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="b67ad-153">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="b67ad-154">Пример</span><span class="sxs-lookup"><span data-stu-id="b67ad-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b67ad-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="b67ad-155">Request</span></span>

<span data-ttu-id="b67ad-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b67ad-156">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getTeamsUserActivityUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="b67ad-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="b67ad-157">Response</span></span>

<span data-ttu-id="b67ad-158">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b67ad-158">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="b67ad-159">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="b67ad-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Is Deleted,Deleted Date,Assigned Products,Team Chat Message Count,Private Chat Message Count,Call Count,Meeting Count,Has Other Action,Report Period
```
