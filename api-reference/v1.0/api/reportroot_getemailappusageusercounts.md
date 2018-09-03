# <a name="reportroot-getemailappusageusercounts"></a><span data-ttu-id="fee1b-101">reportRoot: getEmailAppUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="fee1b-101">reportRoot: getEmailAppUsageUserCounts</span></span>

<span data-ttu-id="fee1b-102">Получение числа уникальных пользователей, которые подключались к Exchange Online с помощью приложения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="fee1b-102">Get the count of unique users that connected to Exchange Online using any email app.</span></span>

> <span data-ttu-id="fee1b-103">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Центре администрирования Office 365 — использование почтовых приложений](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span><span class="sxs-lookup"><span data-stu-id="fee1b-103">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="fee1b-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fee1b-104">Permissions</span></span>

<span data-ttu-id="fee1b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fee1b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="fee1b-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fee1b-107">Permission type</span></span>                        | <span data-ttu-id="fee1b-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fee1b-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="fee1b-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fee1b-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="fee1b-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fee1b-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="fee1b-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fee1b-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fee1b-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fee1b-112">Not supported.</span></span>                           |
| <span data-ttu-id="fee1b-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fee1b-113">Application</span></span>                            | <span data-ttu-id="fee1b-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fee1b-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="fee1b-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fee1b-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="fee1b-116">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="fee1b-116">Function parameters</span></span>

<span data-ttu-id="fee1b-117">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="fee1b-117">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="fee1b-118">Параметр</span><span class="sxs-lookup"><span data-stu-id="fee1b-118">Parameter</span></span> | <span data-ttu-id="fee1b-119">Тип</span><span class="sxs-lookup"><span data-stu-id="fee1b-119">Type</span></span>   | <span data-ttu-id="fee1b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="fee1b-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="fee1b-121">period</span><span class="sxs-lookup"><span data-stu-id="fee1b-121">period</span></span>    | <span data-ttu-id="fee1b-122">строка</span><span class="sxs-lookup"><span data-stu-id="fee1b-122">string</span></span> | <span data-ttu-id="fee1b-123">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="fee1b-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="fee1b-124">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="fee1b-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="fee1b-125">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="fee1b-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="fee1b-126">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fee1b-126">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="fee1b-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fee1b-127">Request headers</span></span>

| <span data-ttu-id="fee1b-128">Имя</span><span class="sxs-lookup"><span data-stu-id="fee1b-128">Name</span></span>          | <span data-ttu-id="fee1b-129">Описание</span><span class="sxs-lookup"><span data-stu-id="fee1b-129">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="fee1b-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fee1b-130">Authorization</span></span> | <span data-ttu-id="fee1b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fee1b-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="fee1b-133">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="fee1b-133">If-None-Match</span></span> | <span data-ttu-id="fee1b-134">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="fee1b-134">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="fee1b-135">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="fee1b-135">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="fee1b-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="fee1b-136">Response</span></span>

<span data-ttu-id="fee1b-137">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="fee1b-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="fee1b-138">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="fee1b-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="fee1b-139">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="fee1b-139">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="fee1b-140">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="fee1b-140">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="fee1b-141">Report Refresh Date (дата обновления отчета)</span><span class="sxs-lookup"><span data-stu-id="fee1b-141">Report Refresh Date</span></span>
- <span data-ttu-id="fee1b-142">Mail For Mac (Mail для Mac)</span><span class="sxs-lookup"><span data-stu-id="fee1b-142">Mail For Mac</span></span>
- <span data-ttu-id="fee1b-143">"Outlook For Mac" (Outlook для Mac);</span><span class="sxs-lookup"><span data-stu-id="fee1b-143">Outlook For Mac</span></span>
- <span data-ttu-id="fee1b-144">"Outlook For Windows" (Outlook для Windows);</span><span class="sxs-lookup"><span data-stu-id="fee1b-144">Outlook For Windows</span></span>
- <span data-ttu-id="fee1b-145">"Outlook For Mobile" (Outlook для мобильных устройств);</span><span class="sxs-lookup"><span data-stu-id="fee1b-145">Outlook For Mobile</span></span>
- <span data-ttu-id="fee1b-146">"Other For Mobile" (Другое для мобильных устройств);</span><span class="sxs-lookup"><span data-stu-id="fee1b-146">Other For Mobile</span></span>
- <span data-ttu-id="fee1b-147">"Outlook For Web" (Outlook для браузера);</span><span class="sxs-lookup"><span data-stu-id="fee1b-147">Outlook For Web</span></span>
- <span data-ttu-id="fee1b-148">"POP3 App" (Приложение с поддержкой POP3);</span><span class="sxs-lookup"><span data-stu-id="fee1b-148">POP3 App</span></span>
- <span data-ttu-id="fee1b-149">"IMAP4 App" (Приложение с поддержкой IMAP4);</span><span class="sxs-lookup"><span data-stu-id="fee1b-149">IMAP4 App</span></span>
- <span data-ttu-id="fee1b-150">SMTP App (Приложение с поддержкой SMTP)</span><span class="sxs-lookup"><span data-stu-id="fee1b-150">SMTP App</span></span>
- <span data-ttu-id="fee1b-151">Report Date (Дата отчета)</span><span class="sxs-lookup"><span data-stu-id="fee1b-151">Report Date</span></span>
- <span data-ttu-id="fee1b-152">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="fee1b-152">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="fee1b-153">Пример</span><span class="sxs-lookup"><span data-stu-id="fee1b-153">Example</span></span>

#### <a name="request"></a><span data-ttu-id="fee1b-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="fee1b-154">Request</span></span>

<span data-ttu-id="fee1b-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fee1b-155">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getemailappusageusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getEmailAppUsageUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="fee1b-156">Ответ</span><span class="sxs-lookup"><span data-stu-id="fee1b-156">Response</span></span>

<span data-ttu-id="fee1b-157">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="fee1b-157">The following is an example of the response.</span></span>

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

<span data-ttu-id="fee1b-158">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="fee1b-158">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Mail For Mac,Outlook For Mac,Outlook For Windows,Outlook For Mobile,Other For Mobile,Outlook For Web,POP3 App,IMAP4 App,SMTP App,Report Date,Report Period
```
