# <a name="reportroot-getmailboxusagemailboxcounts"></a><span data-ttu-id="79277-101">reportRoot: getMailboxUsageMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="79277-101">reportRoot: getMailboxUsageMailboxCounts</span></span>

<span data-ttu-id="79277-102">Узнайте, сколько всего почтовых ящиков в организации и сколько из них были активный в отчетный период.</span><span class="sxs-lookup"><span data-stu-id="79277-102">Get the total number of user mailboxes in your organization and how many are active each day of the reporting period.</span></span> <span data-ttu-id="79277-103">Почтовый ящик считается активным, если пользователь отправил или прочитал по крайней мере одно письмо.</span><span class="sxs-lookup"><span data-stu-id="79277-103">A mailbox is considered active if the user sent or read any email.</span></span>

> <span data-ttu-id="79277-104">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="79277-104">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="79277-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="79277-105">Permissions</span></span>

<span data-ttu-id="79277-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="79277-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="79277-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="79277-108">Permission type</span></span>                        | <span data-ttu-id="79277-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="79277-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="79277-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79277-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="79277-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79277-111">Not supported.</span></span>                           |
| <span data-ttu-id="79277-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="79277-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79277-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79277-113">Not supported.</span></span>                           |
| <span data-ttu-id="79277-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="79277-114">Application</span></span>                            | <span data-ttu-id="79277-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="79277-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="79277-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="79277-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageMailboxCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="79277-117">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="79277-117">Request parameters</span></span>

<span data-ttu-id="79277-118">В URL-адресе запроса укажите следующий параметр запроса и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="79277-118">In the request URL, provide the following query parameter with a valid value.</span></span>

| <span data-ttu-id="79277-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="79277-119">Parameter</span></span> | <span data-ttu-id="79277-120">Тип</span><span class="sxs-lookup"><span data-stu-id="79277-120">Type</span></span>   | <span data-ttu-id="79277-121">Описание</span><span class="sxs-lookup"><span data-stu-id="79277-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="79277-122">period</span><span class="sxs-lookup"><span data-stu-id="79277-122">period</span></span>    | <span data-ttu-id="79277-123">строка</span><span class="sxs-lookup"><span data-stu-id="79277-123">string</span></span> | <span data-ttu-id="79277-124">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="79277-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="79277-125">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="79277-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="79277-126">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="79277-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="79277-127">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79277-127">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="79277-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="79277-128">Request headers</span></span>

| <span data-ttu-id="79277-129">Имя</span><span class="sxs-lookup"><span data-stu-id="79277-129">Name</span></span>          | <span data-ttu-id="79277-130">Описание</span><span class="sxs-lookup"><span data-stu-id="79277-130">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="79277-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="79277-131">Authorization</span></span> | <span data-ttu-id="79277-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79277-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="79277-134">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="79277-134">if-none-match</span></span> | <span data-ttu-id="79277-135">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код ответа `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="79277-135">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `304 Not Modified` response is returned.</span></span> <span data-ttu-id="79277-136">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="79277-136">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="79277-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="79277-137">Response</span></span>

<span data-ttu-id="79277-138">В случае успешного выполнения этот метод возвращает ответ `302 Found`, который перенаправляет на URL-адрес с предварительной аутентификацией для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="79277-138">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="79277-139">Этот URL-адрес можно найти в заголовке ответа `Location`.</span><span class="sxs-lookup"><span data-stu-id="79277-139">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="79277-140">URL-адреса с предварительной аутентификацией действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="79277-140">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<span data-ttu-id="79277-141">CSV-файл содержит столбцы со следующими заголовками.</span><span class="sxs-lookup"><span data-stu-id="79277-141">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="79277-142">Report Refresh Date (дата обновления отчета)</span><span class="sxs-lookup"><span data-stu-id="79277-142">Report Refresh Date</span></span>
- <span data-ttu-id="79277-143">Total (всего)</span><span class="sxs-lookup"><span data-stu-id="79277-143">total</span></span>
- <span data-ttu-id="79277-144">Active (активные)</span><span class="sxs-lookup"><span data-stu-id="79277-144">Active</span></span>
- <span data-ttu-id="79277-145">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="79277-145">Report Date</span></span>
- <span data-ttu-id="79277-146">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="79277-146">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="79277-147">Пример</span><span class="sxs-lookup"><span data-stu-id="79277-147">Example</span></span>

#### <a name="request"></a><span data-ttu-id="79277-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="79277-148">Request</span></span>

<span data-ttu-id="79277-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="79277-149">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getmailboxusagemailboxcounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getMailboxUsageMailboxCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="79277-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="79277-150">Response</span></span>

<span data-ttu-id="79277-151">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="79277-151">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="79277-152">Скачанный после перенаправления 302 CSV-файл будет иметь следующую схему.</span><span class="sxs-lookup"><span data-stu-id="79277-152">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Total,Active,Report Date,Report Period
```
