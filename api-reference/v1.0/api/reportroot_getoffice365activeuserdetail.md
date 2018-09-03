# <a name="reportroot-getoffice365activeuserdetail"></a><span data-ttu-id="bdfa6-101">reportRoot: getOffice365ActiveUserDetail</span><span class="sxs-lookup"><span data-stu-id="bdfa6-101">reportRoot: getOffice365ActiveUserDetail</span></span>

<span data-ttu-id="bdfa6-102">Получение сведений об активных пользователях Office 365.</span><span class="sxs-lookup"><span data-stu-id="bdfa6-102">Get details about Office 365 active users.</span></span>

> <span data-ttu-id="bdfa6-103">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: активные пользователи](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span><span class="sxs-lookup"><span data-stu-id="bdfa6-103">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="bdfa6-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bdfa6-104">Permissions</span></span>

<span data-ttu-id="bdfa6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="bdfa6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="bdfa6-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bdfa6-107">Permission type</span></span>                        | <span data-ttu-id="bdfa6-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bdfa6-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="bdfa6-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bdfa6-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="bdfa6-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bdfa6-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="bdfa6-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bdfa6-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bdfa6-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bdfa6-112">Not supported.</span></span>                           |
| <span data-ttu-id="bdfa6-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bdfa6-113">Application</span></span>                            | <span data-ttu-id="bdfa6-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bdfa6-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="bdfa6-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bdfa6-115">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOffice365ActiveUserDetail(period='{period_value}')
GET /reports/getOffice365ActiveUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="bdfa6-116">Параметры функций</span><span class="sxs-lookup"><span data-stu-id="bdfa6-116">Function parameters</span></span>

<span data-ttu-id="bdfa6-117">В URL-адресе запроса укажите один из следующих параметров с действительным значением.</span><span class="sxs-lookup"><span data-stu-id="bdfa6-117">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="bdfa6-118">Параметр</span><span class="sxs-lookup"><span data-stu-id="bdfa6-118">Parameter</span></span> | <span data-ttu-id="bdfa6-119">Тип</span><span class="sxs-lookup"><span data-stu-id="bdfa6-119">Type</span></span>   | <span data-ttu-id="bdfa6-120">Описание</span><span class="sxs-lookup"><span data-stu-id="bdfa6-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="bdfa6-121">period</span><span class="sxs-lookup"><span data-stu-id="bdfa6-121">period</span></span>    | <span data-ttu-id="bdfa6-122">строка</span><span class="sxs-lookup"><span data-stu-id="bdfa6-122">string</span></span> | <span data-ttu-id="bdfa6-123">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="bdfa6-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="bdfa6-124">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="bdfa6-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="bdfa6-125">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="bdfa6-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="bdfa6-126">date</span><span class="sxs-lookup"><span data-stu-id="bdfa6-126">date</span></span>      | <span data-ttu-id="bdfa6-127">Дата</span><span class="sxs-lookup"><span data-stu-id="bdfa6-127">Date</span></span>   | <span data-ttu-id="bdfa6-128">Указывает дату, за которую вы хотите просмотреть пользователей, выполнивших какое-либо действие.</span><span class="sxs-lookup"><span data-stu-id="bdfa6-128">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="bdfa6-129">Значение {date_value} указывается в формате ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="bdfa6-129">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="bdfa6-130">Так как этот отчет доступен только за последние 30 дней, значение {date_value} должно быть датой из этого диапазона.</span><span class="sxs-lookup"><span data-stu-id="bdfa6-130">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="bdfa6-131">**Примечание.** В URL-адресе необходимо указать либо период, либо дату.</span><span class="sxs-lookup"><span data-stu-id="bdfa6-131">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bdfa6-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bdfa6-132">Request headers</span></span>

| <span data-ttu-id="bdfa6-133">Имя</span><span class="sxs-lookup"><span data-stu-id="bdfa6-133">Name</span></span>          | <span data-ttu-id="bdfa6-134">Описание</span><span class="sxs-lookup"><span data-stu-id="bdfa6-134">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="bdfa6-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bdfa6-135">Authorization</span></span> | <span data-ttu-id="bdfa6-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bdfa6-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="bdfa6-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="bdfa6-138">If-None-Match</span></span> | <span data-ttu-id="bdfa6-139">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="bdfa6-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="bdfa6-140">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="bdfa6-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="bdfa6-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="bdfa6-141">Response</span></span>

<span data-ttu-id="bdfa6-142">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="bdfa6-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="bdfa6-143">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="bdfa6-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="bdfa6-144">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="bdfa6-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="bdfa6-145">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="bdfa6-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="bdfa6-146">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="bdfa6-146">Report Refresh Date</span></span>
- <span data-ttu-id="bdfa6-147">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="bdfa6-147">User Principal Name</span></span>
- <span data-ttu-id="bdfa6-148">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="bdfa6-148">Display Name</span></span>
- <span data-ttu-id="bdfa6-149">"Is Deleted" (Удалено);</span><span class="sxs-lookup"><span data-stu-id="bdfa6-149">Is Deleted</span></span>
- <span data-ttu-id="bdfa6-150">"Deleted Date" (Дата удаления);</span><span class="sxs-lookup"><span data-stu-id="bdfa6-150">Deleted Date</span></span>
- <span data-ttu-id="bdfa6-151">"Has Exchange License" (Есть лицензия на Exchange);</span><span class="sxs-lookup"><span data-stu-id="bdfa6-151">Has Exchange License</span></span>
- <span data-ttu-id="bdfa6-152">"Has OneDrive License" (Есть лицензия на OneDrive);</span><span class="sxs-lookup"><span data-stu-id="bdfa6-152">Has OneDrive License</span></span>
- <span data-ttu-id="bdfa6-153">"Has SharePoint License" (Есть лицензия на SharePoint);</span><span class="sxs-lookup"><span data-stu-id="bdfa6-153">Has SharePoint License</span></span>
- <span data-ttu-id="bdfa6-154">"Has Skype For Business License" (Есть лицензия на Skype для бизнеса);</span><span class="sxs-lookup"><span data-stu-id="bdfa6-154">Has Skype For Business License</span></span>
- <span data-ttu-id="bdfa6-155">"Has Yammer License" (Есть лицензия на Yammer);</span><span class="sxs-lookup"><span data-stu-id="bdfa6-155">Has Yammer License</span></span>
- <span data-ttu-id="bdfa6-156">"Has Teams License" (Есть лицензия на Teams);</span><span class="sxs-lookup"><span data-stu-id="bdfa6-156">Has Teams License</span></span>
- <span data-ttu-id="bdfa6-157">"Exchange Last Activity Date" (Дата последнего действия в Exchange);</span><span class="sxs-lookup"><span data-stu-id="bdfa6-157">Exchange Last Activity Date</span></span>
- <span data-ttu-id="bdfa6-158">"OneDrive Last Activity Date" (Дата последнего действия в OneDrive);</span><span class="sxs-lookup"><span data-stu-id="bdfa6-158">OneDrive Last Activity Date</span></span>
- <span data-ttu-id="bdfa6-159">"SharePoint Last Activity Date" (Дата последнего действия в SharePoint);</span><span class="sxs-lookup"><span data-stu-id="bdfa6-159">SharePoint Last Activity Date</span></span>
- <span data-ttu-id="bdfa6-160">"Skype For Business Last Activity Date" (Дата последнего действия в Skype для бизнеса);</span><span class="sxs-lookup"><span data-stu-id="bdfa6-160">Skype For Business Last Activity Date</span></span>
- <span data-ttu-id="bdfa6-161">"Yammer Last Activity Date" (Дата последнего действия в Yammer);</span><span class="sxs-lookup"><span data-stu-id="bdfa6-161">Yammer Last Activity Date</span></span>
- <span data-ttu-id="bdfa6-162">"Teams Last Activity Date" (Дата последнего действия в Teams);</span><span class="sxs-lookup"><span data-stu-id="bdfa6-162">Teams Last Activity Date</span></span>
- <span data-ttu-id="bdfa6-163">"Exchange License Assign Date" (Дата назначения лицензии на Exchange);</span><span class="sxs-lookup"><span data-stu-id="bdfa6-163">Exchange License Assign Date</span></span>
- <span data-ttu-id="bdfa6-164">"OneDrive License Assign Date" (Дата назначения лицензии на OneDrive);</span><span class="sxs-lookup"><span data-stu-id="bdfa6-164">OneDrive License Assign Date</span></span>
- <span data-ttu-id="bdfa6-165">"SharePoint License Assign Date" (Дата назначения лицензии на SharePoint);</span><span class="sxs-lookup"><span data-stu-id="bdfa6-165">SharePoint License Assign Date</span></span>
- <span data-ttu-id="bdfa6-166">"Skype For Business License Assign Date" (Дата назначения лицензии на Skype для бизнеса);</span><span class="sxs-lookup"><span data-stu-id="bdfa6-166">Skype For Business License Assign Date</span></span>
- <span data-ttu-id="bdfa6-167">"Yammer License Assign Date" (Дата назначения лицензии на Yammer);</span><span class="sxs-lookup"><span data-stu-id="bdfa6-167">Yammer License Assign Date</span></span>
- <span data-ttu-id="bdfa6-168">"Teams License Assign Date" (Дата назначения лицензии на Teams);</span><span class="sxs-lookup"><span data-stu-id="bdfa6-168">Teams License Assign Date</span></span>
- <span data-ttu-id="bdfa6-169">"Assigned Products" (Назначенные продукты).</span><span class="sxs-lookup"><span data-stu-id="bdfa6-169">Assigned Products</span></span>

## <a name="example"></a><span data-ttu-id="bdfa6-170">Пример</span><span class="sxs-lookup"><span data-stu-id="bdfa6-170">Example</span></span>

#### <a name="request"></a><span data-ttu-id="bdfa6-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="bdfa6-171">Request</span></span>

<span data-ttu-id="bdfa6-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bdfa6-172">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activeuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActiveUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="bdfa6-173">Ответ</span><span class="sxs-lookup"><span data-stu-id="bdfa6-173">Response</span></span>

<span data-ttu-id="bdfa6-174">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="bdfa6-174">The following is an example of the response.</span></span>

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

<span data-ttu-id="bdfa6-175">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="bdfa6-175">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Has Exchange License,Has OneDrive License,Has SharePoint License,Has Skype For Business License,Has Yammer License,Has Teams License,Exchange Last Activity Date,OneDrive Last Activity Date,SharePoint Last Activity Date,Skype For Business Last Activity Date,Yammer Last Activity Date,Teams Last Activity Date,Exchange License Assign Date,OneDrive License Assign Date,SharePoint License Assign Date,Skype For Business License Assign Date,Yammer License Assign Date,Teams License Assign Date,Assigned Products
```
