# <a name="reportroot-getskypeforbusinessdeviceusageusercounts"></a><span data-ttu-id="4796e-101">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="4796e-101">reportRoot: getSkypeForBusinessDeviceUsageUserCounts</span></span>

<span data-ttu-id="4796e-102">Отследите динамику использования по количеству пользователей в организации, подключавшихся с помощью приложения Skype для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="4796e-102">Get the usage trends on how many users in your organization have connected using the Skype for Business app.</span></span> <span data-ttu-id="4796e-103">Кроме того, вы получите статистические данные с разбивкой по типу устройства (Windows, телефон с Windows, телефон с Android, iPhone или iPad), на котором установлено клиентское приложение Skype для бизнеса, используемое в организации.</span><span class="sxs-lookup"><span data-stu-id="4796e-103">You will also get a breakdown by the type of device (Windows, Windows phone, Android phone, iPhone, or iPad) on which the Skype for Business client app is installed and used across your organization.</span></span>

> <span data-ttu-id="4796e-104">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: используемые клиенты Skype для бизнеса](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span><span class="sxs-lookup"><span data-stu-id="4796e-104">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="4796e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4796e-105">Permissions</span></span>

<span data-ttu-id="4796e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4796e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="4796e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4796e-108">Permission type</span></span>                        | <span data-ttu-id="4796e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4796e-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="4796e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4796e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="4796e-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4796e-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="4796e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4796e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4796e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4796e-113">Not supported.</span></span>                           |
| <span data-ttu-id="4796e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4796e-114">Application</span></span>                            | <span data-ttu-id="4796e-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4796e-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="4796e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4796e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageUserCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="4796e-117">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="4796e-117">Request parameters</span></span>

<span data-ttu-id="4796e-118">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="4796e-118">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="4796e-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="4796e-119">Parameter</span></span> | <span data-ttu-id="4796e-120">Тип</span><span class="sxs-lookup"><span data-stu-id="4796e-120">Type</span></span>   | <span data-ttu-id="4796e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="4796e-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="4796e-122">period</span><span class="sxs-lookup"><span data-stu-id="4796e-122">period</span></span>    | <span data-ttu-id="4796e-123">string</span><span class="sxs-lookup"><span data-stu-id="4796e-123">string</span></span> | <span data-ttu-id="4796e-124">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="4796e-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="4796e-125">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="4796e-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="4796e-126">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="4796e-126">These values follow the format D   where    represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="4796e-127">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4796e-127">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="4796e-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4796e-128">Request headers</span></span>

| <span data-ttu-id="4796e-129">Имя</span><span class="sxs-lookup"><span data-stu-id="4796e-129">Name</span></span>          | <span data-ttu-id="4796e-130">Описание</span><span class="sxs-lookup"><span data-stu-id="4796e-130">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="4796e-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4796e-131">Authorization</span></span> | <span data-ttu-id="4796e-p104">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4796e-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="4796e-134">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="4796e-134">If-None-Match</span></span> | <span data-ttu-id="4796e-135">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="4796e-135">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="4796e-136">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="4796e-136">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="4796e-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="4796e-137">Response</span></span>

<span data-ttu-id="4796e-138">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="4796e-138">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="4796e-139">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="4796e-139">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="4796e-140">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="4796e-140">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="4796e-141">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="4796e-141">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="4796e-142">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="4796e-142">Report Refresh Date</span></span>
- <span data-ttu-id="4796e-143">"Windows";</span><span class="sxs-lookup"><span data-stu-id="4796e-143">Windows</span></span>
- <span data-ttu-id="4796e-144">"Windows Phone";</span><span class="sxs-lookup"><span data-stu-id="4796e-144">Windows Phone</span></span>
- <span data-ttu-id="4796e-145">"Android Phone" (Телефон с Android);</span><span class="sxs-lookup"><span data-stu-id="4796e-145">Android Phone</span></span>
- <span data-ttu-id="4796e-146">"iPhone";</span><span class="sxs-lookup"><span data-stu-id="4796e-146">iPhone</span></span>
- <span data-ttu-id="4796e-147">"iPad";</span><span class="sxs-lookup"><span data-stu-id="4796e-147">iPad</span></span>
- <span data-ttu-id="4796e-148">"Report Date" (Дата отчета);</span><span class="sxs-lookup"><span data-stu-id="4796e-148">Report Date</span></span>
- <span data-ttu-id="4796e-149">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="4796e-149">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="4796e-150">Пример</span><span class="sxs-lookup"><span data-stu-id="4796e-150">Example</span></span>

#### <a name="request"></a><span data-ttu-id="4796e-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="4796e-151">Request</span></span>

<span data-ttu-id="4796e-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4796e-152">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusageusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessDeviceUsageUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="4796e-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="4796e-153">Response</span></span>

<span data-ttu-id="4796e-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4796e-154">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="4796e-155">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="4796e-155">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Windows,Windows Phone,Android Phone,iPhone,iPad,Report Date,Report Period
```
