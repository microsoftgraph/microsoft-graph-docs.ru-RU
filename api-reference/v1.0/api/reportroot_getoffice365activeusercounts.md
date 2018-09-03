# <a name="reportroot-getoffice365activeusercounts"></a><span data-ttu-id="6a622-101">reportRoot: getOffice365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="6a622-101">reportRoot: getOffice365ActiveUserCounts</span></span>

<span data-ttu-id="6a622-102">Получение количества активных пользователей за каждый день отчетного периода по продукту.</span><span class="sxs-lookup"><span data-stu-id="6a622-102">Get the count of daily active users in the reporting period by product.</span></span>

> <span data-ttu-id="6a622-103">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: активные пользователи](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="6a622-103">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="6a622-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6a622-104">Permissions</span></span>

<span data-ttu-id="6a622-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6a622-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="6a622-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6a622-107">Permission type</span></span>                        | <span data-ttu-id="6a622-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6a622-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="6a622-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6a622-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="6a622-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a622-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="6a622-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6a622-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a622-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a622-112">Not supported.</span></span>                           |
| <span data-ttu-id="6a622-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6a622-113">Application</span></span>                            | <span data-ttu-id="6a622-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a622-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="6a622-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6a622-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="6a622-116">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="6a622-116">Function parameters</span></span>

<span data-ttu-id="6a622-117">В URL-адресе запроса укажите следующий параметр с действительным значением.</span><span class="sxs-lookup"><span data-stu-id="6a622-117">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="6a622-118">Параметр</span><span class="sxs-lookup"><span data-stu-id="6a622-118">Parameter</span></span> | <span data-ttu-id="6a622-119">Тип</span><span class="sxs-lookup"><span data-stu-id="6a622-119">Type</span></span>   | <span data-ttu-id="6a622-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6a622-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="6a622-121">period</span><span class="sxs-lookup"><span data-stu-id="6a622-121">period</span></span>    | <span data-ttu-id="6a622-122">строка</span><span class="sxs-lookup"><span data-stu-id="6a622-122">string</span></span> | <span data-ttu-id="6a622-123">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="6a622-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="6a622-124">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="6a622-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="6a622-125">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="6a622-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="6a622-126">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6a622-126">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="6a622-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6a622-127">Request headers</span></span>

| <span data-ttu-id="6a622-128">Имя</span><span class="sxs-lookup"><span data-stu-id="6a622-128">Name</span></span>          | <span data-ttu-id="6a622-129">Описание</span><span class="sxs-lookup"><span data-stu-id="6a622-129">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="6a622-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6a622-130">Authorization</span></span> | <span data-ttu-id="6a622-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6a622-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="6a622-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="6a622-133">Response</span></span>

<span data-ttu-id="6a622-134">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="6a622-134">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="6a622-135">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="6a622-135">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="6a622-136">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="6a622-136">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="6a622-137">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="6a622-137">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="6a622-138">Report Refresh Date (Дата обновления отчета)</span><span class="sxs-lookup"><span data-stu-id="6a622-138">Report Refresh Date</span></span>
- <span data-ttu-id="6a622-139">Office 365</span><span class="sxs-lookup"><span data-stu-id="6a622-139">Office 365</span></span>
- <span data-ttu-id="6a622-140">Exchange</span><span class="sxs-lookup"><span data-stu-id="6a622-140">Exchange</span></span>
- <span data-ttu-id="6a622-141">OneDrive</span><span class="sxs-lookup"><span data-stu-id="6a622-141">OneDrive</span></span>
- <span data-ttu-id="6a622-142">SharePoint</span><span class="sxs-lookup"><span data-stu-id="6a622-142">SharePoint</span></span>
- <span data-ttu-id="6a622-143">Skype для бизнеса</span><span class="sxs-lookup"><span data-stu-id="6a622-143">Skype For Business</span></span> 
- <span data-ttu-id="6a622-144">Yammer</span><span class="sxs-lookup"><span data-stu-id="6a622-144">Yammer</span></span>
- <span data-ttu-id="6a622-145">Teams</span><span class="sxs-lookup"><span data-stu-id="6a622-145">Teams</span></span>
- <span data-ttu-id="6a622-146">Report Date (Дата отчета)</span><span class="sxs-lookup"><span data-stu-id="6a622-146">Report Date</span></span>
- <span data-ttu-id="6a622-147">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="6a622-147">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="6a622-148">Пример</span><span class="sxs-lookup"><span data-stu-id="6a622-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="6a622-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="6a622-149">Request</span></span>

<span data-ttu-id="6a622-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6a622-150">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activeusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActiveUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="6a622-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="6a622-151">Response</span></span>

<span data-ttu-id="6a622-152">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6a622-152">The following is an example of the response.</span></span>

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

<span data-ttu-id="6a622-153">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="6a622-153">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Office 365,Exchange,OneDrive,SharePoint,Skype For Business,Yammer,Teams,Report Date,Report Period
```
