# <a name="reportroot-getteamsuseractivitycounts"></a><span data-ttu-id="f5b38-101">reportRoot: getTeamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="f5b38-101">reportRoot: getTeamsUserActivityCounts</span></span>

<span data-ttu-id="f5b38-102">Получение количества действий в Microsoft Teams по каждому типу.</span><span class="sxs-lookup"><span data-stu-id="f5b38-102">Get the number of Microsoft Teams activities by activity type.</span></span> <span data-ttu-id="f5b38-103">К типам действий относятся сообщения в чатах групп, сообщения в приватных чатах, звонки и собрания.</span><span class="sxs-lookup"><span data-stu-id="f5b38-103">The activity types are team chat messages, private chat messages, calls, and meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="f5b38-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f5b38-104">Permissions</span></span>

<span data-ttu-id="f5b38-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f5b38-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="f5b38-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f5b38-107">Permission type</span></span>                        | <span data-ttu-id="f5b38-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f5b38-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="f5b38-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f5b38-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="f5b38-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f5b38-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="f5b38-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f5b38-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5b38-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5b38-112">Not supported.</span></span>                           |
| <span data-ttu-id="f5b38-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f5b38-113">Application</span></span>                            | <span data-ttu-id="f5b38-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="f5b38-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="f5b38-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f5b38-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="f5b38-116">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="f5b38-116">Request parameters</span></span>

<span data-ttu-id="f5b38-117">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="f5b38-117">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="f5b38-118">Параметр</span><span class="sxs-lookup"><span data-stu-id="f5b38-118">Parameter</span></span> | <span data-ttu-id="f5b38-119">Тип</span><span class="sxs-lookup"><span data-stu-id="f5b38-119">Type</span></span>   | <span data-ttu-id="f5b38-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f5b38-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="f5b38-121">period</span><span class="sxs-lookup"><span data-stu-id="f5b38-121">period</span></span>    | <span data-ttu-id="f5b38-122">string</span><span class="sxs-lookup"><span data-stu-id="f5b38-122">string</span></span> | <span data-ttu-id="f5b38-123">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="f5b38-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="f5b38-124">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="f5b38-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="f5b38-125">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="f5b38-125">These values follow the format D   where    represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="f5b38-126">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f5b38-126">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="f5b38-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f5b38-127">Request headers</span></span>

| <span data-ttu-id="f5b38-128">Имя</span><span class="sxs-lookup"><span data-stu-id="f5b38-128">Name</span></span>          | <span data-ttu-id="f5b38-129">Описание</span><span class="sxs-lookup"><span data-stu-id="f5b38-129">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="f5b38-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f5b38-130">Authorization</span></span> | <span data-ttu-id="f5b38-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f5b38-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="f5b38-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5b38-133">Response</span></span>

<span data-ttu-id="f5b38-134">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="f5b38-134">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="f5b38-135">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="f5b38-135">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="f5b38-136">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="f5b38-136">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="f5b38-137">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="f5b38-137">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="f5b38-138">Report Refresh Date (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="f5b38-138">Report Refresh Date</span></span>
- <span data-ttu-id="f5b38-139">Report Date (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="f5b38-139">Report Date</span></span>
- <span data-ttu-id="f5b38-140">Team Chat Messages (Сообщения в чатах групп);</span><span class="sxs-lookup"><span data-stu-id="f5b38-140">Team Chat Messages</span></span>
- <span data-ttu-id="f5b38-141">Private Chat Messages (Сообщения в приватных чатах);</span><span class="sxs-lookup"><span data-stu-id="f5b38-141">Private Chat Messages</span></span>
- <span data-ttu-id="f5b38-142">Calls (Звонки);</span><span class="sxs-lookup"><span data-stu-id="f5b38-142">Calls</span></span>
- <span data-ttu-id="f5b38-143">Meetings (собрания);</span><span class="sxs-lookup"><span data-stu-id="f5b38-143">Meetings</span></span>
- <span data-ttu-id="f5b38-144">Report Period (отчетный период).</span><span class="sxs-lookup"><span data-stu-id="f5b38-144">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="f5b38-145">Пример</span><span class="sxs-lookup"><span data-stu-id="f5b38-145">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f5b38-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="f5b38-146">Request</span></span>

<span data-ttu-id="f5b38-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f5b38-147">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivitycounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getTeamsUserActivityCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="f5b38-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5b38-148">Response</span></span>

<span data-ttu-id="f5b38-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f5b38-149">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
<span data-ttu-id="f5b38-150">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="f5b38-150">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Team Chat Messages,Private Chat Messages,Calls,Meetings,Report Period
```
