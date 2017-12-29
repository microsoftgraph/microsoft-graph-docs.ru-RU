# <a name="reportroot-getskypeforbusinessorganizeractivitycounts"></a><span data-ttu-id="d004d-101">reportRoot: getSkypeForBusinessOrganizerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="d004d-101">reportRoot: getSkypeForBusinessOrganizerActivityCounts</span></span>

<span data-ttu-id="d004d-102">Получение сведений о том, как меняется количество и тип сеансов конференц-связи, проводимых и организуемых пользователями в организации.</span><span class="sxs-lookup"><span data-stu-id="d004d-102">Get usage trends on the number and type of conference sessions held and organized by users in your organization.</span></span> <span data-ttu-id="d004d-103">Такие типы включают обмен мгновенными сообщениями, общий доступ к приложениям, аудио, видео, а также веб-конференции, конференции с возможностью присоединения по прямому или обратному звонку (сторонняя служба или корпорация Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="d004d-103">Types of conference sessions include IM, audio/video, application sharing, web, dial-in/out - 3rd party, and Dial-in/out Microsoft.</span></span>

> <span data-ttu-id="d004d-104">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия организатора конференций в Skype для бизнеса](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span><span class="sxs-lookup"><span data-stu-id="d004d-104">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).</span></span>

## <a name="permissions"></a><span data-ttu-id="d004d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d004d-105">Permissions</span></span>

<span data-ttu-id="d004d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d004d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="d004d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d004d-108">Permission type</span></span>                        | <span data-ttu-id="d004d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d004d-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="d004d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d004d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d004d-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d004d-111">Not supported.</span></span>                           |
| <span data-ttu-id="d004d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d004d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d004d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d004d-113">Not supported.</span></span>                           |
| <span data-ttu-id="d004d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d004d-114">Application</span></span>                            | <span data-ttu-id="d004d-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d004d-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="d004d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d004d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessOrganizerActivityCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="d004d-117">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="d004d-117">Request parameters</span></span>

<span data-ttu-id="d004d-118">В URL-адресе запроса укажите указанный ниже параметр запроса и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="d004d-118">In the request URL, provide the following query parameter with a valid value.</span></span>

| <span data-ttu-id="d004d-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="d004d-119">Parameter</span></span> | <span data-ttu-id="d004d-120">Тип</span><span class="sxs-lookup"><span data-stu-id="d004d-120">Type</span></span>   | <span data-ttu-id="d004d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d004d-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="d004d-122">period</span><span class="sxs-lookup"><span data-stu-id="d004d-122">period</span></span>    | <span data-ttu-id="d004d-123">string</span><span class="sxs-lookup"><span data-stu-id="d004d-123">string</span></span> | <span data-ttu-id="d004d-124">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="d004d-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="d004d-125">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="d004d-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="d004d-126">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="d004d-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="d004d-127">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d004d-127">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="d004d-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d004d-128">Request headers</span></span>

| <span data-ttu-id="d004d-129">Имя</span><span class="sxs-lookup"><span data-stu-id="d004d-129">Name</span></span>          | <span data-ttu-id="d004d-130">Описание</span><span class="sxs-lookup"><span data-stu-id="d004d-130">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="d004d-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d004d-131">Authorization</span></span> | <span data-ttu-id="d004d-p104">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d004d-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d004d-134">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="d004d-134">if-none-match</span></span> | <span data-ttu-id="d004d-135">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="d004d-135">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `304 Not Modified` response is returned.</span></span> <span data-ttu-id="d004d-136">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="d004d-136">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="d004d-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="d004d-137">Response</span></span>

<span data-ttu-id="d004d-138">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="d004d-138">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d004d-139">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="d004d-139">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d004d-140">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="d004d-140">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<span data-ttu-id="d004d-141">CSV-файл содержит столбцы со следующими заголовками.</span><span class="sxs-lookup"><span data-stu-id="d004d-141">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="d004d-142">Report Refresh Date (Дата обновления отчета)</span><span class="sxs-lookup"><span data-stu-id="d004d-142">Report Refresh Date</span></span>
- <span data-ttu-id="d004d-143">Report Date (Дата отчета)</span><span class="sxs-lookup"><span data-stu-id="d004d-143">Report Date</span></span>
- <span data-ttu-id="d004d-144">Report Period (Отчетный период)</span><span class="sxs-lookup"><span data-stu-id="d004d-144">Report Period</span></span>
- <span data-ttu-id="d004d-145">IM (Обмен мгновенными сообщениями)</span><span class="sxs-lookup"><span data-stu-id="d004d-145">IM</span></span>
- <span data-ttu-id="d004d-146">Audio/Video (Аудио и видео)</span><span class="sxs-lookup"><span data-stu-id="d004d-146">Audio/Video</span></span>
- <span data-ttu-id="d004d-147">App Sharing (Общий доступ к приложениям)</span><span class="sxs-lookup"><span data-stu-id="d004d-147">App sharing</span></span>
- <span data-ttu-id="d004d-148">Web (Интернет)</span><span class="sxs-lookup"><span data-stu-id="d004d-148">Web</span></span>
- <span data-ttu-id="d004d-149">Dial-in/out 3rd Party (Конференции с возможностью присоединения по прямому или обратному звонку, сторонняя служба)</span><span class="sxs-lookup"><span data-stu-id="d004d-149">Dial-in/out 3rd Party</span></span>
- <span data-ttu-id="d004d-150">Dial-in/out Microsoft (Конференции с возможностью присоединения по прямому или обратному звонку, корпорация Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d004d-150">Dial-in/out Microsoft</span></span>

## <a name="example"></a><span data-ttu-id="d004d-151">Пример</span><span class="sxs-lookup"><span data-stu-id="d004d-151">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d004d-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="d004d-152">Request</span></span>

<span data-ttu-id="d004d-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d004d-153">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessorganizeractivitycounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessOrganizerActivityCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="d004d-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="d004d-154">Response</span></span>

<span data-ttu-id="d004d-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d004d-155">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="d004d-156">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="d004d-156">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,IM,Audio/Video,App Sharing,Web,Dial-in/out 3rd Party,Dial-in/out Microsoft
```
