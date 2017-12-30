# <a name="reportroot-getemailappusageversionsusercounts"></a><span data-ttu-id="3dd9e-101">reportRoot: getEmailAppUsageVersionsUserCounts</span><span class="sxs-lookup"><span data-stu-id="3dd9e-101">reportRoot: getEmailAppUsageVersionsUserCounts</span></span>

<span data-ttu-id="3dd9e-102">Узнайте, сколько уникальных пользователей у каждой версии Outlook для компьютера.</span><span class="sxs-lookup"><span data-stu-id="3dd9e-102">Get the count of unique users by Outlook desktop version.</span></span>

> <span data-ttu-id="3dd9e-103">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span><span class="sxs-lookup"><span data-stu-id="3dd9e-103">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="3dd9e-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3dd9e-104">Permissions</span></span>

<span data-ttu-id="3dd9e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3dd9e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="3dd9e-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3dd9e-107">Permission type</span></span>                        | <span data-ttu-id="3dd9e-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3dd9e-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="3dd9e-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3dd9e-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="3dd9e-110">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3dd9e-110">Not supported.</span></span>                           |
| <span data-ttu-id="3dd9e-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3dd9e-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3dd9e-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3dd9e-112">Not supported.</span></span>                           |
| <span data-ttu-id="3dd9e-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3dd9e-113">Application</span></span>                            | <span data-ttu-id="3dd9e-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3dd9e-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="3dd9e-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3dd9e-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageVersionsUserCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="3dd9e-116">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="3dd9e-116">Request parameters</span></span>

<span data-ttu-id="3dd9e-117">В URL-адресе запроса укажите следующий параметр запроса и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="3dd9e-117">In the request URL, provide the following query parameter with a valid value.</span></span>

| <span data-ttu-id="3dd9e-118">Параметр</span><span class="sxs-lookup"><span data-stu-id="3dd9e-118">Parameter</span></span> | <span data-ttu-id="3dd9e-119">Тип</span><span class="sxs-lookup"><span data-stu-id="3dd9e-119">Type</span></span>   | <span data-ttu-id="3dd9e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3dd9e-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="3dd9e-121">period</span><span class="sxs-lookup"><span data-stu-id="3dd9e-121">period</span></span>    | <span data-ttu-id="3dd9e-122">строка</span><span class="sxs-lookup"><span data-stu-id="3dd9e-122">string</span></span> | <span data-ttu-id="3dd9e-123">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="3dd9e-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="3dd9e-124">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="3dd9e-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="3dd9e-125">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="3dd9e-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="3dd9e-126">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3dd9e-126">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="3dd9e-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3dd9e-127">Request headers</span></span>

| <span data-ttu-id="3dd9e-128">Имя</span><span class="sxs-lookup"><span data-stu-id="3dd9e-128">Name</span></span>          | <span data-ttu-id="3dd9e-129">Описание</span><span class="sxs-lookup"><span data-stu-id="3dd9e-129">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="3dd9e-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3dd9e-130">Authorization</span></span> | <span data-ttu-id="3dd9e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3dd9e-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="3dd9e-133">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="3dd9e-133">if-none-match</span></span> | <span data-ttu-id="3dd9e-134">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код ответа `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="3dd9e-134">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `304 Not Modified` response is returned.</span></span> <span data-ttu-id="3dd9e-135">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="3dd9e-135">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="3dd9e-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="3dd9e-136">Response</span></span>

<span data-ttu-id="3dd9e-137">В случае успешного выполнения этот метод возвращает ответ `302 Found`, который перенаправляет на URL-адрес с предварительной аутентификацией для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="3dd9e-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="3dd9e-138">Этот URL-адрес можно найти в заголовке ответа `Location`.</span><span class="sxs-lookup"><span data-stu-id="3dd9e-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="3dd9e-139">URL-адреса с предварительной аутентификацией действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="3dd9e-139">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<span data-ttu-id="3dd9e-140">CSV-файл содержит столбцы со следующими заголовками.</span><span class="sxs-lookup"><span data-stu-id="3dd9e-140">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="3dd9e-141">Report Refresh Date (дата обновления отчета)</span><span class="sxs-lookup"><span data-stu-id="3dd9e-141">Report Refresh Date</span></span>
- <span data-ttu-id="3dd9e-142">Outlook 2016</span><span class="sxs-lookup"><span data-stu-id="3dd9e-142">Outlook 2016</span></span>
- <span data-ttu-id="3dd9e-143">Outlook 2013</span><span class="sxs-lookup"><span data-stu-id="3dd9e-143">Outlook 2013</span></span>
- <span data-ttu-id="3dd9e-144">Outlook 2010</span><span class="sxs-lookup"><span data-stu-id="3dd9e-144">Outlook 2010</span></span>
- <span data-ttu-id="3dd9e-145">Outlook 2007</span><span class="sxs-lookup"><span data-stu-id="3dd9e-145">Outlook 2007</span></span>
- <span data-ttu-id="3dd9e-146">Undetermined (не определено)</span><span class="sxs-lookup"><span data-stu-id="3dd9e-146">Undetermined</span></span>
- <span data-ttu-id="3dd9e-147">Report Period (отчетный период)</span><span class="sxs-lookup"><span data-stu-id="3dd9e-147">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="3dd9e-148">Пример</span><span class="sxs-lookup"><span data-stu-id="3dd9e-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="3dd9e-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="3dd9e-149">Request</span></span>

<span data-ttu-id="3dd9e-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3dd9e-150">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageversionsusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getEmailAppUsageVersionsUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="3dd9e-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="3dd9e-151">Response</span></span>

<span data-ttu-id="3dd9e-152">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3dd9e-152">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="3dd9e-153">Скачанный после перенаправления 302 CSV-файл будет иметь следующую схему.</span><span class="sxs-lookup"><span data-stu-id="3dd9e-153">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Outlook 2016,Outlook 2013,Outlook 2010,Outlook 2007,Undetermined,Report Period
```
