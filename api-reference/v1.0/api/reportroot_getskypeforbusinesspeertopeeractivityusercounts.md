# <a name="reportroot-getskypeforbusinesspeertopeeractivityusercounts"></a><span data-ttu-id="2c2e5-101">reportRoot: getSkypeForBusinessPeerToPeerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="2c2e5-101">reportRoot: getSkypeForBusinessPeerToPeerActivityUserCounts</span></span>

<span data-ttu-id="2c2e5-102">Отследите динамику использования по количеству уникальных пользователей и типу проведенных в организации одноранговых сеансов.</span><span class="sxs-lookup"><span data-stu-id="2c2e5-102">Get usage trends on the number of unique users and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="2c2e5-103">Такие типы включают обмен мгновенными сообщениями, предоставление общего доступа к приложениям, аудио, видео, а также передачу файлов в одноранговых сеансах.</span><span class="sxs-lookup"><span data-stu-id="2c2e5-103">Types of sessions include IM, audio, video, application sharing, and file transfers in peer-to-peer sessions.</span></span>

> <span data-ttu-id="2c2e5-104">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия в одноранговых сеансах Skype для бизнеса](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span><span class="sxs-lookup"><span data-stu-id="2c2e5-104">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="permissions"></a><span data-ttu-id="2c2e5-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2c2e5-105">Permissions</span></span>

<span data-ttu-id="2c2e5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2c2e5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="2c2e5-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2c2e5-108">Permission type</span></span>                        | <span data-ttu-id="2c2e5-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2c2e5-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="2c2e5-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2c2e5-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="2c2e5-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c2e5-111">Not supported.</span></span>                           |
| <span data-ttu-id="2c2e5-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2c2e5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c2e5-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c2e5-113">Not supported.</span></span>                           |
| <span data-ttu-id="2c2e5-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2c2e5-114">Application</span></span>                            | <span data-ttu-id="2c2e5-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2c2e5-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="2c2e5-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2c2e5-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessPeerToPeerActivityUserCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="2c2e5-117">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="2c2e5-117">Request parameters</span></span>

<span data-ttu-id="2c2e5-118">В URL-адресе запроса укажите приведенный ниже параметр запроса и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="2c2e5-118">In the request URL, provide the following query parameter with a valid value.</span></span>

| <span data-ttu-id="2c2e5-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="2c2e5-119">Parameter</span></span> | <span data-ttu-id="2c2e5-120">Тип</span><span class="sxs-lookup"><span data-stu-id="2c2e5-120">Type</span></span>   | <span data-ttu-id="2c2e5-121">Описание</span><span class="sxs-lookup"><span data-stu-id="2c2e5-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="2c2e5-122">period</span><span class="sxs-lookup"><span data-stu-id="2c2e5-122">period</span></span>    | <span data-ttu-id="2c2e5-123">string</span><span class="sxs-lookup"><span data-stu-id="2c2e5-123">string</span></span> | <span data-ttu-id="2c2e5-124">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="2c2e5-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="2c2e5-125">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="2c2e5-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="2c2e5-126">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="2c2e5-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="2c2e5-127">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2c2e5-127">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="2c2e5-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2c2e5-128">Request headers</span></span>

| <span data-ttu-id="2c2e5-129">Имя</span><span class="sxs-lookup"><span data-stu-id="2c2e5-129">Name</span></span>          | <span data-ttu-id="2c2e5-130">Описание</span><span class="sxs-lookup"><span data-stu-id="2c2e5-130">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="2c2e5-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2c2e5-131">Authorization</span></span> | <span data-ttu-id="2c2e5-p104">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2c2e5-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2c2e5-134">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="2c2e5-134">if-none-match</span></span> | <span data-ttu-id="2c2e5-135">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="2c2e5-135">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `304 Not Modified` response is returned.</span></span> <span data-ttu-id="2c2e5-136">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="2c2e5-136">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="2c2e5-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c2e5-137">Response</span></span>

<span data-ttu-id="2c2e5-138">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="2c2e5-138">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="2c2e5-139">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="2c2e5-139">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="2c2e5-140">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="2c2e5-140">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<span data-ttu-id="2c2e5-141">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="2c2e5-141">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="2c2e5-142">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="2c2e5-142">Report Refresh Date</span></span>
- <span data-ttu-id="2c2e5-143">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="2c2e5-143">Report Date</span></span>
- <span data-ttu-id="2c2e5-144">"Report Period" (Отчетный период);</span><span class="sxs-lookup"><span data-stu-id="2c2e5-144">Report Period</span></span>
- <span data-ttu-id="2c2e5-145">"IM" (Обмен мгновенными сообщениями);</span><span class="sxs-lookup"><span data-stu-id="2c2e5-145">IM</span></span>
- <span data-ttu-id="2c2e5-146">"Audio" (Аудио);</span><span class="sxs-lookup"><span data-stu-id="2c2e5-146">Audio</span></span>
- <span data-ttu-id="2c2e5-147">"Video" (Видео);</span><span class="sxs-lookup"><span data-stu-id="2c2e5-147">Video</span></span>
- <span data-ttu-id="2c2e5-148">"App Sharing" (Общий доступ к приложениям);</span><span class="sxs-lookup"><span data-stu-id="2c2e5-148">App sharing</span></span>
- <span data-ttu-id="2c2e5-149">"File Transfer" (Передача файлов).</span><span class="sxs-lookup"><span data-stu-id="2c2e5-149">File Transfer</span></span>

## <a name="example"></a><span data-ttu-id="2c2e5-150">Пример</span><span class="sxs-lookup"><span data-stu-id="2c2e5-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="2c2e5-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="2c2e5-151">Request</span></span>

<span data-ttu-id="2c2e5-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2c2e5-152">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessPeerToPeerActivityUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="2c2e5-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c2e5-153">Response</span></span>

<span data-ttu-id="2c2e5-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2c2e5-154">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="2c2e5-155">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="2c2e5-155">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio,Video,App Sharing,File Transfer
```
