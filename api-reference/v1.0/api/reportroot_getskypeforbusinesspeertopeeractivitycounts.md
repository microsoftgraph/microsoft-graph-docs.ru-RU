# <a name="reportroot-getskypeforbusinesspeertopeeractivitycounts"></a><span data-ttu-id="81d35-101">reportRoot: getSkypeForBusinessPeerToPeerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="81d35-101">reportRoot: getSkypeForBusinessPeerToPeerActivityCounts</span></span>

<span data-ttu-id="81d35-102">Отслеживайте динамику использования по количеству и типу проведенных в организации сеансов</span><span class="sxs-lookup"><span data-stu-id="81d35-102">Get usage trends on the number and type of sessions held in your organization.</span></span> <span data-ttu-id="81d35-103">(обмен мгновенными сообщениями, аудио, видео, общий доступ к приложениям и передача файлов).</span><span class="sxs-lookup"><span data-stu-id="81d35-103">Types of sessions include IM, audio, video, application sharing, and file transfer.</span></span>

> <span data-ttu-id="81d35-104">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span><span class="sxs-lookup"><span data-stu-id="81d35-104">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="permissions"></a><span data-ttu-id="81d35-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="81d35-105">Permissions</span></span>

<span data-ttu-id="81d35-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="81d35-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="81d35-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="81d35-108">Permission type</span></span>                        | <span data-ttu-id="81d35-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="81d35-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="81d35-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="81d35-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="81d35-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="81d35-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="81d35-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="81d35-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81d35-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81d35-113">Not supported.</span></span>                           |
| <span data-ttu-id="81d35-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="81d35-114">Application</span></span>                            | <span data-ttu-id="81d35-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="81d35-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="81d35-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="81d35-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessPeerToPeerActivityCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="81d35-117">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="81d35-117">Request parameters</span></span>

<span data-ttu-id="81d35-118">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="81d35-118">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="81d35-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="81d35-119">Parameter</span></span> | <span data-ttu-id="81d35-120">Тип</span><span class="sxs-lookup"><span data-stu-id="81d35-120">Type</span></span>   | <span data-ttu-id="81d35-121">Описание</span><span class="sxs-lookup"><span data-stu-id="81d35-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="81d35-122">period</span><span class="sxs-lookup"><span data-stu-id="81d35-122">period</span></span>    | <span data-ttu-id="81d35-123">строка</span><span class="sxs-lookup"><span data-stu-id="81d35-123">string</span></span> | <span data-ttu-id="81d35-124">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="81d35-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="81d35-125">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="81d35-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="81d35-126">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="81d35-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="81d35-127">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="81d35-127">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="81d35-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="81d35-128">Request headers</span></span>

| <span data-ttu-id="81d35-129">Имя</span><span class="sxs-lookup"><span data-stu-id="81d35-129">Name</span></span>          | <span data-ttu-id="81d35-130">Описание</span><span class="sxs-lookup"><span data-stu-id="81d35-130">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="81d35-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="81d35-131">Authorization</span></span> | <span data-ttu-id="81d35-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="81d35-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="81d35-134">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="81d35-134">If-None-Match</span></span> | <span data-ttu-id="81d35-135">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="81d35-135">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="81d35-136">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="81d35-136">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="81d35-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="81d35-137">Response</span></span>

<span data-ttu-id="81d35-138">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="81d35-138">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="81d35-139">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="81d35-139">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="81d35-140">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="81d35-140">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="81d35-141">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="81d35-141">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="81d35-142">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="81d35-142">Report Refresh Date</span></span>
- <span data-ttu-id="81d35-143">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="81d35-143">Report Date</span></span>
- <span data-ttu-id="81d35-144">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="81d35-144">Report Period</span></span>
- <span data-ttu-id="81d35-145">"IM" (Обмен мгновенными сообщениями);</span><span class="sxs-lookup"><span data-stu-id="81d35-145">IM</span></span>
- <span data-ttu-id="81d35-146">Audio (аудио)</span><span class="sxs-lookup"><span data-stu-id="81d35-146">Audio</span></span>
- <span data-ttu-id="81d35-147">Video (видео)</span><span class="sxs-lookup"><span data-stu-id="81d35-147">Video</span></span>
- <span data-ttu-id="81d35-148">"App Sharing" (Общий доступ к приложениям);</span><span class="sxs-lookup"><span data-stu-id="81d35-148">App Sharing</span></span>
- <span data-ttu-id="81d35-149">"File Transfer" (Передача файлов).</span><span class="sxs-lookup"><span data-stu-id="81d35-149">File Transfer</span></span>

## <a name="example"></a><span data-ttu-id="81d35-150">Пример</span><span class="sxs-lookup"><span data-stu-id="81d35-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="81d35-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="81d35-151">Request</span></span>

<span data-ttu-id="81d35-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="81d35-152">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getskypeforbusinesspeertopeeractivitycounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessPeerToPeerActivityCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="81d35-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="81d35-153">Response</span></span>

<span data-ttu-id="81d35-154">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="81d35-154">The following is an example of the response.</span></span>

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

<span data-ttu-id="81d35-155">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="81d35-155">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio,Video,App Sharing,File Transfer
```
