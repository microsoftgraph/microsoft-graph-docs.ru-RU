# <a name="reportroot-getmailboxusagestorage"></a><span data-ttu-id="57d2d-101">reportRoot: getMailboxUsageStorage</span><span class="sxs-lookup"><span data-stu-id="57d2d-101">reportRoot: getMailboxUsageStorage</span></span>

<span data-ttu-id="57d2d-102">Узнайте, сколько места занято в хранилище организации.</span><span class="sxs-lookup"><span data-stu-id="57d2d-102">Get the amount of storage used in your organization.</span></span>

> <span data-ttu-id="57d2d-103">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: использование почтовых ящиков](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="57d2d-103">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="57d2d-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="57d2d-104">Permissions</span></span>

<span data-ttu-id="57d2d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="57d2d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="57d2d-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="57d2d-107">Permission type</span></span>                        | <span data-ttu-id="57d2d-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="57d2d-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="57d2d-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="57d2d-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="57d2d-110">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57d2d-110">Not supported.</span></span>                           |
| <span data-ttu-id="57d2d-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="57d2d-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57d2d-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57d2d-112">Not supported.</span></span>                           |
| <span data-ttu-id="57d2d-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="57d2d-113">Application</span></span>                            | <span data-ttu-id="57d2d-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="57d2d-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="57d2d-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="57d2d-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageStorage(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="57d2d-116">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="57d2d-116">Request parameters</span></span>

<span data-ttu-id="57d2d-117">В URL-адресе запроса укажите приведенный ниже параметр запроса и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="57d2d-117">In the request URL, provide the following query parameter with a valid value.</span></span>

| <span data-ttu-id="57d2d-118">Параметр</span><span class="sxs-lookup"><span data-stu-id="57d2d-118">Parameter</span></span> | <span data-ttu-id="57d2d-119">Тип</span><span class="sxs-lookup"><span data-stu-id="57d2d-119">Type</span></span>   | <span data-ttu-id="57d2d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="57d2d-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="57d2d-121">period</span><span class="sxs-lookup"><span data-stu-id="57d2d-121">period</span></span>    | <span data-ttu-id="57d2d-122">string</span><span class="sxs-lookup"><span data-stu-id="57d2d-122">string</span></span> | <span data-ttu-id="57d2d-123">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="57d2d-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="57d2d-124">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="57d2d-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="57d2d-125">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="57d2d-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="57d2d-126">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="57d2d-126">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="57d2d-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="57d2d-127">Request headers</span></span>

| <span data-ttu-id="57d2d-128">Имя</span><span class="sxs-lookup"><span data-stu-id="57d2d-128">Name</span></span>          | <span data-ttu-id="57d2d-129">Описание</span><span class="sxs-lookup"><span data-stu-id="57d2d-129">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="57d2d-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="57d2d-130">Authorization</span></span> | <span data-ttu-id="57d2d-p103">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="57d2d-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="57d2d-133">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="57d2d-133">if-none-match</span></span> | <span data-ttu-id="57d2d-134">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="57d2d-134">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `304 Not Modified` response is returned.</span></span> <span data-ttu-id="57d2d-135">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="57d2d-135">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="57d2d-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="57d2d-136">Response</span></span>

<span data-ttu-id="57d2d-137">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="57d2d-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="57d2d-138">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="57d2d-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="57d2d-139">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="57d2d-139">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<span data-ttu-id="57d2d-140">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="57d2d-140">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="57d2d-141">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="57d2d-141">Report Refresh Date</span></span>
- <span data-ttu-id="57d2d-142">"Storage Used (Byte)" (Используемый объем хранилища в байтах);</span><span class="sxs-lookup"><span data-stu-id="57d2d-142">Storage Used (Byte)</span></span>
- <span data-ttu-id="57d2d-143">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="57d2d-143">Report Date</span></span>
- <span data-ttu-id="57d2d-144">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="57d2d-144">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="57d2d-145">Пример</span><span class="sxs-lookup"><span data-stu-id="57d2d-145">Example</span></span>

#### <a name="request"></a><span data-ttu-id="57d2d-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="57d2d-146">Request</span></span>

<span data-ttu-id="57d2d-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="57d2d-147">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagestorage"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getMailboxUsageStorage(period='D7')
```

#### <a name="response"></a><span data-ttu-id="57d2d-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="57d2d-148">Response</span></span>

<span data-ttu-id="57d2d-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="57d2d-149">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="57d2d-150">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="57d2d-150">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Storage Used (Byte),Report Date,Report Period
```
