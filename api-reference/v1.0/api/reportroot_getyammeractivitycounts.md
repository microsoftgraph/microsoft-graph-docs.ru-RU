# <a name="reportroot-getyammeractivitycounts"></a><span data-ttu-id="69372-101">reportRoot: getYammerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="69372-101">reportRoot: getYammerActivityCounts</span></span>

<span data-ttu-id="69372-102">Отслеживайте динамику активности пользователей в Yammer по количеству опубликованных, прочитанных и понравившихся сообщений.</span><span class="sxs-lookup"><span data-stu-id="69372-102">Get the trends on the amount of Yammer activity in your organization by how many messages were posted, read, and liked.</span></span>

> <span data-ttu-id="69372-103">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span><span class="sxs-lookup"><span data-stu-id="69372-103">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="permissions"></a><span data-ttu-id="69372-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="69372-104">Permissions</span></span>

<span data-ttu-id="69372-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="69372-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="69372-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="69372-107">Permission type</span></span>                        | <span data-ttu-id="69372-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="69372-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="69372-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="69372-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="69372-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="69372-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="69372-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="69372-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69372-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69372-112">Not supported.</span></span>                           |
| <span data-ttu-id="69372-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="69372-113">Application</span></span>                            | <span data-ttu-id="69372-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="69372-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="69372-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="69372-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="69372-116">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="69372-116">Function parameters</span></span>

<span data-ttu-id="69372-117">В URL-адресе запроса укажите следующий параметр с действительными значениями.</span><span class="sxs-lookup"><span data-stu-id="69372-117">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="69372-118">Параметр</span><span class="sxs-lookup"><span data-stu-id="69372-118">Parameter</span></span> | <span data-ttu-id="69372-119">Тип</span><span class="sxs-lookup"><span data-stu-id="69372-119">Type</span></span>   | <span data-ttu-id="69372-120">Описание</span><span class="sxs-lookup"><span data-stu-id="69372-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="69372-121">period</span><span class="sxs-lookup"><span data-stu-id="69372-121">period</span></span>    | <span data-ttu-id="69372-122">строка</span><span class="sxs-lookup"><span data-stu-id="69372-122">string</span></span> | <span data-ttu-id="69372-123">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="69372-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="69372-124">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="69372-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="69372-125">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="69372-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="69372-126">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="69372-126">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="69372-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="69372-127">Request headers</span></span>

| <span data-ttu-id="69372-128">Имя</span><span class="sxs-lookup"><span data-stu-id="69372-128">Name</span></span>          | <span data-ttu-id="69372-129">Описание</span><span class="sxs-lookup"><span data-stu-id="69372-129">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="69372-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="69372-130">Authorization</span></span> | <span data-ttu-id="69372-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="69372-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="69372-133">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="69372-133">If-None-Match</span></span> | <span data-ttu-id="69372-134">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="69372-134">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="69372-135">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="69372-135">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="69372-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="69372-136">Response</span></span>

<span data-ttu-id="69372-137">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="69372-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="69372-138">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="69372-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="69372-139">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="69372-139">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="69372-140">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="69372-140">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="69372-141">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="69372-141">Report Refresh Date</span></span>
- <span data-ttu-id="69372-142">"Liked" (Понравилось);</span><span class="sxs-lookup"><span data-stu-id="69372-142">Liked</span></span>
- <span data-ttu-id="69372-143">"Posted" (Опубликовано);</span><span class="sxs-lookup"><span data-stu-id="69372-143">Posted</span></span>
- <span data-ttu-id="69372-144">"Read" (Чтение);</span><span class="sxs-lookup"><span data-stu-id="69372-144">Read</span></span>
- <span data-ttu-id="69372-145">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="69372-145">Report Date</span></span>
- <span data-ttu-id="69372-146">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="69372-146">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="69372-147">Пример</span><span class="sxs-lookup"><span data-stu-id="69372-147">Example</span></span>

#### <a name="request"></a><span data-ttu-id="69372-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="69372-148">Request</span></span>

<span data-ttu-id="69372-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="69372-149">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammeractivitycounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerActivityCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="69372-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="69372-150">Response</span></span>

<span data-ttu-id="69372-151">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="69372-151">The following is an example of the response.</span></span>

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

<span data-ttu-id="69372-152">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="69372-152">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Liked,Posted,Read,Report Date,Report Period
```
