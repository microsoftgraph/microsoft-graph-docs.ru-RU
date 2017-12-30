# <a name="reportroot-getskypeforbusinessactivityusercounts"></a><span data-ttu-id="574a3-101">reportRoot: getSkypeForBusinessActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="574a3-101">reportRoot: getSkypeForBusinessActivityUserCounts</span></span>

<span data-ttu-id="574a3-102">Отследите, как меняется количество уникальных организаторов и участников сеансов конференций, проводимых в вашей организации через Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="574a3-102">Get the trends on how many unique users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="574a3-103">Отчет также включает количество одноранговых сеансов.</span><span class="sxs-lookup"><span data-stu-id="574a3-103">The report also includes the number of peer-to-peer sessions.</span></span>

> <span data-ttu-id="574a3-104">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия в Skype для бизнеса](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span><span class="sxs-lookup"><span data-stu-id="574a3-104">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="574a3-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="574a3-105">Permissions</span></span>

<span data-ttu-id="574a3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="574a3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="574a3-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="574a3-108">Permission type</span></span>                        | <span data-ttu-id="574a3-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="574a3-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="574a3-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="574a3-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="574a3-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="574a3-111">Not supported.</span></span>                           |
| <span data-ttu-id="574a3-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="574a3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="574a3-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="574a3-113">Not supported.</span></span>                           |
| <span data-ttu-id="574a3-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="574a3-114">Application</span></span>                            | <span data-ttu-id="574a3-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="574a3-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="574a3-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="574a3-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessActivityUserCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="574a3-117">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="574a3-117">Request parameters</span></span>

<span data-ttu-id="574a3-118">В URL-адресе запроса укажите приведенный ниже параметр запроса и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="574a3-118">In the request URL, provide the following query parameter with a valid value.</span></span>

| <span data-ttu-id="574a3-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="574a3-119">Parameter</span></span> | <span data-ttu-id="574a3-120">Тип</span><span class="sxs-lookup"><span data-stu-id="574a3-120">Type</span></span>   | <span data-ttu-id="574a3-121">Описание</span><span class="sxs-lookup"><span data-stu-id="574a3-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="574a3-122">period</span><span class="sxs-lookup"><span data-stu-id="574a3-122">period</span></span>    | <span data-ttu-id="574a3-123">string</span><span class="sxs-lookup"><span data-stu-id="574a3-123">string</span></span> | <span data-ttu-id="574a3-124">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="574a3-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="574a3-125">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="574a3-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="574a3-126">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="574a3-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="574a3-127">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="574a3-127">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="574a3-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="574a3-128">Request headers</span></span>

| <span data-ttu-id="574a3-129">Имя</span><span class="sxs-lookup"><span data-stu-id="574a3-129">Name</span></span>          | <span data-ttu-id="574a3-130">Описание</span><span class="sxs-lookup"><span data-stu-id="574a3-130">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="574a3-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="574a3-131">Authorization</span></span> | <span data-ttu-id="574a3-p104">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="574a3-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="574a3-134">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="574a3-134">if-none-match</span></span> | <span data-ttu-id="574a3-135">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="574a3-135">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `304 Not Modified` response is returned.</span></span> <span data-ttu-id="574a3-136">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="574a3-136">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="574a3-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="574a3-137">Response</span></span>

<span data-ttu-id="574a3-138">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="574a3-138">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="574a3-139">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="574a3-139">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="574a3-140">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="574a3-140">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<span data-ttu-id="574a3-141">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="574a3-141">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="574a3-142">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="574a3-142">Report Refresh Date</span></span>
- <span data-ttu-id="574a3-143">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="574a3-143">Report Date</span></span>
- <span data-ttu-id="574a3-144">"Report Period" (Отчетный период);</span><span class="sxs-lookup"><span data-stu-id="574a3-144">Report Period</span></span>
- <span data-ttu-id="574a3-145">"Peer-to-peer" (Одноранговый сеанс);</span><span class="sxs-lookup"><span data-stu-id="574a3-145">Peer-to-peer network</span></span>
- <span data-ttu-id="574a3-146">"Organized" (Организаторы);</span><span class="sxs-lookup"><span data-stu-id="574a3-146">Organized</span></span>
- <span data-ttu-id="574a3-147">"Participated" (Участники).</span><span class="sxs-lookup"><span data-stu-id="574a3-147">Participated</span></span>

## <a name="example"></a><span data-ttu-id="574a3-148">Пример</span><span class="sxs-lookup"><span data-stu-id="574a3-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="574a3-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="574a3-149">Request</span></span>

<span data-ttu-id="574a3-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="574a3-150">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivityusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessActivityUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="574a3-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="574a3-151">Response</span></span>

<span data-ttu-id="574a3-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="574a3-152">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="574a3-153">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="574a3-153">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Peer-to-peer,Organized,Participated
```
