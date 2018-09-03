# <a name="reportroot-getemailactivitycounts"></a><span data-ttu-id="daa25-101">reportRoot: getEmailActivityCounts</span><span class="sxs-lookup"><span data-stu-id="daa25-101">reportRoot: getEmailActivityCounts</span></span>

<span data-ttu-id="daa25-102">Позволяет понять динамику работы с электронной почтой (сколько писем было отправлено, прочитано и получено) в организации.</span><span class="sxs-lookup"><span data-stu-id="daa25-102">Enables you to understand the trends of email activity (like how many were sent, read, and received) in your organization.</span></span>

> <span data-ttu-id="daa25-103">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span><span class="sxs-lookup"><span data-stu-id="daa25-103">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="permissions"></a><span data-ttu-id="daa25-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="daa25-104">Permissions</span></span>

<span data-ttu-id="daa25-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="daa25-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="daa25-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="daa25-107">Permission type</span></span>                        | <span data-ttu-id="daa25-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="daa25-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="daa25-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="daa25-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="daa25-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="daa25-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="daa25-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="daa25-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="daa25-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="daa25-112">Not supported.</span></span>                           |
| <span data-ttu-id="daa25-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="daa25-113">Application</span></span>                            | <span data-ttu-id="daa25-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="daa25-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="daa25-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="daa25-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="daa25-116">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="daa25-116">Function parameters</span></span>

<span data-ttu-id="daa25-117">В URL-адресе запроса укажите следующий параметр с действительным значением.</span><span class="sxs-lookup"><span data-stu-id="daa25-117">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="daa25-118">Параметр</span><span class="sxs-lookup"><span data-stu-id="daa25-118">Parameter</span></span> | <span data-ttu-id="daa25-119">Тип</span><span class="sxs-lookup"><span data-stu-id="daa25-119">Type</span></span>   | <span data-ttu-id="daa25-120">Описание</span><span class="sxs-lookup"><span data-stu-id="daa25-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="daa25-121">period</span><span class="sxs-lookup"><span data-stu-id="daa25-121">period</span></span>    | <span data-ttu-id="daa25-122">строка</span><span class="sxs-lookup"><span data-stu-id="daa25-122">string</span></span> | <span data-ttu-id="daa25-123">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="daa25-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="daa25-124">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="daa25-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="daa25-125">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="daa25-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="daa25-126">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="daa25-126">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="daa25-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="daa25-127">Request headers</span></span>

| <span data-ttu-id="daa25-128">Имя</span><span class="sxs-lookup"><span data-stu-id="daa25-128">Name</span></span>          | <span data-ttu-id="daa25-129">Описание</span><span class="sxs-lookup"><span data-stu-id="daa25-129">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="daa25-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="daa25-130">Authorization</span></span> | <span data-ttu-id="daa25-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="daa25-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="daa25-133">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="daa25-133">If-None-Match</span></span> | <span data-ttu-id="daa25-134">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="daa25-134">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="daa25-135">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="daa25-135">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="daa25-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="daa25-136">Response</span></span>

<span data-ttu-id="daa25-137">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="daa25-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="daa25-138">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="daa25-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="daa25-139">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="daa25-139">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="daa25-140">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="daa25-140">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="daa25-141">Report Refresh Date (дата обновления отчета)</span><span class="sxs-lookup"><span data-stu-id="daa25-141">Report Refresh Date</span></span>
- <span data-ttu-id="daa25-142">Send (отправлено)</span><span class="sxs-lookup"><span data-stu-id="daa25-142">Send</span></span>
- <span data-ttu-id="daa25-143">Receive (получено)</span><span class="sxs-lookup"><span data-stu-id="daa25-143">Receive</span></span>
- <span data-ttu-id="daa25-144">Read (прочитано)</span><span class="sxs-lookup"><span data-stu-id="daa25-144">Read</span></span>
- <span data-ttu-id="daa25-145">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="daa25-145">Report Date</span></span>
- <span data-ttu-id="daa25-146">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="daa25-146">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="daa25-147">Пример</span><span class="sxs-lookup"><span data-stu-id="daa25-147">Example</span></span>

#### <a name="request"></a><span data-ttu-id="daa25-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="daa25-148">Request</span></span>

<span data-ttu-id="daa25-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="daa25-149">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getemailactivitycounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getEmailActivityCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="daa25-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="daa25-150">Response</span></span>

<span data-ttu-id="daa25-151">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="daa25-151">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="daa25-152">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="daa25-152">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "ignored"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Send,Receive,Read,Report Date,Report Period
```
