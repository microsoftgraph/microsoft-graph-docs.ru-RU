# <a name="reportroot-getmailboxusagedetail"></a><span data-ttu-id="f0877-101">reportRoot: getMailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="f0877-101">reportRoot: getMailboxUsageDetail</span></span>

<span data-ttu-id="f0877-102">Получите сведения об использовании почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="f0877-102">Get details about mailbox usage.</span></span>

> <span data-ttu-id="f0877-103">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="f0877-103">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="permissions"></a><span data-ttu-id="f0877-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f0877-104">Permissions</span></span>

<span data-ttu-id="f0877-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f0877-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="f0877-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f0877-107">Permission type</span></span>                        | <span data-ttu-id="f0877-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f0877-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="f0877-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f0877-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="f0877-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f0877-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="f0877-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f0877-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0877-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0877-112">Not supported.</span></span>                           |
| <span data-ttu-id="f0877-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f0877-113">Application</span></span>                            | <span data-ttu-id="f0877-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f0877-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="f0877-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f0877-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getMailboxUsageDetail(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="f0877-116">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="f0877-116">Function parameters</span></span>

<span data-ttu-id="f0877-117">В URL-адресе запроса укажите следующий параметр с действительным значением.</span><span class="sxs-lookup"><span data-stu-id="f0877-117">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="f0877-118">Параметр</span><span class="sxs-lookup"><span data-stu-id="f0877-118">Parameter</span></span> | <span data-ttu-id="f0877-119">Тип</span><span class="sxs-lookup"><span data-stu-id="f0877-119">Type</span></span>   | <span data-ttu-id="f0877-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f0877-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="f0877-121">period</span><span class="sxs-lookup"><span data-stu-id="f0877-121">period</span></span>    | <span data-ttu-id="f0877-122">строка</span><span class="sxs-lookup"><span data-stu-id="f0877-122">string</span></span> | <span data-ttu-id="f0877-123">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="f0877-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="f0877-124">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="f0877-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="f0877-125">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="f0877-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="f0877-126">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f0877-126">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="f0877-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f0877-127">Request headers</span></span>

| <span data-ttu-id="f0877-128">Имя</span><span class="sxs-lookup"><span data-stu-id="f0877-128">Name</span></span>          | <span data-ttu-id="f0877-129">Описание</span><span class="sxs-lookup"><span data-stu-id="f0877-129">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="f0877-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f0877-130">Authorization</span></span> | <span data-ttu-id="f0877-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f0877-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="f0877-133">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="f0877-133">If-None-Match</span></span> | <span data-ttu-id="f0877-134">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="f0877-134">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="f0877-135">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="f0877-135">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="f0877-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="f0877-136">Response</span></span>

<span data-ttu-id="f0877-137">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="f0877-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="f0877-138">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="f0877-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="f0877-139">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="f0877-139">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="f0877-140">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="f0877-140">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="f0877-141">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="f0877-141">Report Refresh Date</span></span>
- <span data-ttu-id="f0877-142">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="f0877-142">User Principal Name</span></span>
- <span data-ttu-id="f0877-143">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="f0877-143">Display Name</span></span>
- <span data-ttu-id="f0877-144">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="f0877-144">Is Deleted</span></span>
- <span data-ttu-id="f0877-145">Deleted Date (дата удаления)</span><span class="sxs-lookup"><span data-stu-id="f0877-145">Deleted Date</span></span>
- <span data-ttu-id="f0877-146">Created Date (дата создания)</span><span class="sxs-lookup"><span data-stu-id="f0877-146">Created Date</span></span>
- <span data-ttu-id="f0877-147">Last Activity Date (дата последнего действия)</span><span class="sxs-lookup"><span data-stu-id="f0877-147">Last Activity Date</span></span>
- <span data-ttu-id="f0877-148">Item Count (количество элементов)</span><span class="sxs-lookup"><span data-stu-id="f0877-148">Item Count</span></span>
- <span data-ttu-id="f0877-149">Storage Used (Byte) [использовано (байт)]</span><span class="sxs-lookup"><span data-stu-id="f0877-149">Storage Used (Byte)</span></span>
- <span data-ttu-id="f0877-150">Issue Warning Quota (Byte) [объем, при котором выводится предупреждение (байт)]</span><span class="sxs-lookup"><span data-stu-id="f0877-150">Issue Warning Quota (Byte)</span></span>
- <span data-ttu-id="f0877-151">Prohibit Send Quota (Byte) [объем, при котором блокируется отправка (байт)]</span><span class="sxs-lookup"><span data-stu-id="f0877-151">Prohibit Send Quota (Byte)</span></span>
- <span data-ttu-id="f0877-152">Prohibit Send/Receive Quota (Byte) [объем, при котором блокируются отправка и получение (байт)]</span><span class="sxs-lookup"><span data-stu-id="f0877-152">Prohibit Send/Receive Quota (Byte)</span></span>
- <span data-ttu-id="f0877-153">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="f0877-153">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="f0877-154">Пример</span><span class="sxs-lookup"><span data-stu-id="f0877-154">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f0877-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="f0877-155">Request</span></span>

<span data-ttu-id="f0877-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f0877-156">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getmailboxusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getMailboxUsageDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="f0877-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="f0877-157">Response</span></span>

<span data-ttu-id="f0877-158">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f0877-158">The following is an example of the response.</span></span>

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

<span data-ttu-id="f0877-159">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="f0877-159">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Created Date,Last Activity Date,Item Count,Storage Used (Byte),Issue Warning Quota (Byte),Prohibit Send Quota (Byte),Prohibit Send/Receive Quota (Byte),Report Period
```
