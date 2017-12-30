# <a name="reportroot-getoffice365servicesusercounts"></a><span data-ttu-id="199dd-101">reportRoot: getOffice365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="199dd-101">reportRoot: getOffice365ServicesUserCounts</span></span>

<span data-ttu-id="199dd-102">Узнайте, сколько пользователей были активны и неактивны в каждой службе.</span><span class="sxs-lookup"><span data-stu-id="199dd-102">Get the count of users by activity type and service.</span></span>

> <span data-ttu-id="199dd-103">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="199dd-103">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="199dd-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="199dd-104">Permissions</span></span>

<span data-ttu-id="199dd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="199dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="199dd-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="199dd-107">Permission type</span></span>                        | <span data-ttu-id="199dd-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="199dd-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="199dd-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="199dd-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="199dd-110">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="199dd-110">Not supported.</span></span>                           |
| <span data-ttu-id="199dd-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="199dd-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="199dd-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="199dd-112">Not supported.</span></span>                           |
| <span data-ttu-id="199dd-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="199dd-113">Application</span></span>                            | <span data-ttu-id="199dd-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="199dd-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="199dd-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="199dd-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ServicesUserCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="199dd-116">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="199dd-116">Request parameters</span></span>

<span data-ttu-id="199dd-117">В URL-адресе запроса укажите следующий параметр запроса и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="199dd-117">In the request URL, provide the following query parameter with a valid value.</span></span>

| <span data-ttu-id="199dd-118">Параметр</span><span class="sxs-lookup"><span data-stu-id="199dd-118">Parameter</span></span> | <span data-ttu-id="199dd-119">Тип</span><span class="sxs-lookup"><span data-stu-id="199dd-119">Type</span></span>   | <span data-ttu-id="199dd-120">Описание</span><span class="sxs-lookup"><span data-stu-id="199dd-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="199dd-121">period</span><span class="sxs-lookup"><span data-stu-id="199dd-121">period</span></span>    | <span data-ttu-id="199dd-122">строка</span><span class="sxs-lookup"><span data-stu-id="199dd-122">string</span></span> | <span data-ttu-id="199dd-123">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="199dd-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="199dd-124">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="199dd-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="199dd-125">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="199dd-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="199dd-126">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="199dd-126">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="199dd-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="199dd-127">Request headers</span></span>

| <span data-ttu-id="199dd-128">Имя</span><span class="sxs-lookup"><span data-stu-id="199dd-128">Name</span></span>          | <span data-ttu-id="199dd-129">Описание</span><span class="sxs-lookup"><span data-stu-id="199dd-129">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="199dd-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="199dd-130">Authorization</span></span> | <span data-ttu-id="199dd-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="199dd-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="199dd-133">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="199dd-133">if-none-match</span></span> | <span data-ttu-id="199dd-134">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код ответа `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="199dd-134">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `304 Not Modified` response is returned.</span></span> <span data-ttu-id="199dd-135">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="199dd-135">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="199dd-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="199dd-136">Response</span></span>

<span data-ttu-id="199dd-137">В случае успешного выполнения этот метод возвращает ответ `302 Found`, который перенаправляет на URL-адрес с предварительной аутентификацией для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="199dd-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="199dd-138">Этот URL-адрес можно найти в заголовке ответа `Location`.</span><span class="sxs-lookup"><span data-stu-id="199dd-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="199dd-139">URL-адреса с предварительной аутентификацией действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="199dd-139">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<span data-ttu-id="199dd-140">CSV-файл содержит столбцы со следующими заголовками.</span><span class="sxs-lookup"><span data-stu-id="199dd-140">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="199dd-141">Report Refresh Date (дата обновления отчета)</span><span class="sxs-lookup"><span data-stu-id="199dd-141">Report Refresh Date</span></span>
- <span data-ttu-id="199dd-142">Exchange Active (активны в Exchange)</span><span class="sxs-lookup"><span data-stu-id="199dd-142">Exchange Active</span></span>
- <span data-ttu-id="199dd-143">Exchange Inactive (неактивны в Exchange)</span><span class="sxs-lookup"><span data-stu-id="199dd-143">Exchange Inactive</span></span>
- <span data-ttu-id="199dd-144">OneDrive Active (активны в OneDrive)</span><span class="sxs-lookup"><span data-stu-id="199dd-144">OneDrive Active</span></span>
- <span data-ttu-id="199dd-145">OneDrive Inactive (неактивны в OneDrive)</span><span class="sxs-lookup"><span data-stu-id="199dd-145">OneDrive Inactive</span></span>
- <span data-ttu-id="199dd-146">SharePoint Active (активны в SharePoint)</span><span class="sxs-lookup"><span data-stu-id="199dd-146">SharePoint Active</span></span>
- <span data-ttu-id="199dd-147">SharePoint Inactive (неактивны в SharePoint)</span><span class="sxs-lookup"><span data-stu-id="199dd-147">SharePoint Inactive</span></span>
- <span data-ttu-id="199dd-148">Skype For Business Active (активны в Skype для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="199dd-148">Skype For Business Active</span></span>
- <span data-ttu-id="199dd-149">Skype For Business Inactive (неактивны в Skype для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="199dd-149">Skype For Business Inactive</span></span>
- <span data-ttu-id="199dd-150">Yammer Active (активны в Yammer)</span><span class="sxs-lookup"><span data-stu-id="199dd-150">Yammer Active</span></span>
- <span data-ttu-id="199dd-151">Yammer Inactive (неактивны в Yammer)</span><span class="sxs-lookup"><span data-stu-id="199dd-151">Yammer Inactive</span></span>
- <span data-ttu-id="199dd-152">Teams Active (активны в Teams)</span><span class="sxs-lookup"><span data-stu-id="199dd-152">Teams Active</span></span>
- <span data-ttu-id="199dd-153">Teams Inactive (неактивны в Teams)</span><span class="sxs-lookup"><span data-stu-id="199dd-153">Teams Inactive</span></span>
- <span data-ttu-id="199dd-154">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="199dd-154">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="199dd-155">Пример</span><span class="sxs-lookup"><span data-stu-id="199dd-155">Example</span></span>

#### <a name="request"></a><span data-ttu-id="199dd-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="199dd-156">Request</span></span>

<span data-ttu-id="199dd-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="199dd-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365servicesusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ServicesUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="199dd-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="199dd-158">Response</span></span>

<span data-ttu-id="199dd-159">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="199dd-159">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="199dd-160">Скачанный после перенаправления 302 CSV-файл будет иметь следующую схему.</span><span class="sxs-lookup"><span data-stu-id="199dd-160">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Exchange Active,Exchange Inactive,OneDrive Active,OneDrive Inactive,SharePoint Active,SharePoint Inactive,Skype For Business Active,Skype For Business Inactive,Yammer Active,Yammer Inactive,Teams Active,Teams Inactive,Report Period
```
