# <a name="reportroot-getoffice365groupsactivitystorage"></a><span data-ttu-id="70392-101">reportRoot: getOffice365GroupsActivityStorage</span><span class="sxs-lookup"><span data-stu-id="70392-101">reportRoot: getOffice365GroupsActivityStorage</span></span>

<span data-ttu-id="70392-102">Узнайте, сколько места в хранилище занято всеми почтовыми ящиками и сайтами групп.</span><span class="sxs-lookup"><span data-stu-id="70392-102">Get the total storage used across all group mailboxes and group sites.</span></span>

> <span data-ttu-id="70392-103">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span><span class="sxs-lookup"><span data-stu-id="70392-103">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="70392-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="70392-104">Permissions</span></span>

<span data-ttu-id="70392-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="70392-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="70392-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="70392-107">Permission type</span></span>                        | <span data-ttu-id="70392-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="70392-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="70392-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="70392-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="70392-110">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70392-110">Not supported.</span></span>                           |
| <span data-ttu-id="70392-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="70392-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70392-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70392-112">Not supported.</span></span>                           |
| <span data-ttu-id="70392-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="70392-113">Application</span></span>                            | <span data-ttu-id="70392-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="70392-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="70392-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="70392-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityStorage(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="70392-116">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="70392-116">Request parameters</span></span>

<span data-ttu-id="70392-117">В URL-адресе запроса укажите следующий параметр и действительное значение.</span><span class="sxs-lookup"><span data-stu-id="70392-117">In the request URL, provide the following query parameter with a valid value.</span></span>

| <span data-ttu-id="70392-118">Параметр</span><span class="sxs-lookup"><span data-stu-id="70392-118">Parameter</span></span> | <span data-ttu-id="70392-119">Тип</span><span class="sxs-lookup"><span data-stu-id="70392-119">Type</span></span>   | <span data-ttu-id="70392-120">Описание</span><span class="sxs-lookup"><span data-stu-id="70392-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="70392-121">period</span><span class="sxs-lookup"><span data-stu-id="70392-121">period</span></span>    | <span data-ttu-id="70392-122">string</span><span class="sxs-lookup"><span data-stu-id="70392-122">string</span></span> | <span data-ttu-id="70392-123">Указывает отчетный период.</span><span class="sxs-lookup"><span data-stu-id="70392-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="70392-124">Поддерживаемые значения {period_value}: D7, D30, D90 и D180.</span><span class="sxs-lookup"><span data-stu-id="70392-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="70392-125">Эти значения указываются в формате D*n*, где *n* — количество дней в отчетном периоде.</span><span class="sxs-lookup"><span data-stu-id="70392-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="70392-126">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="70392-126">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="70392-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="70392-127">Request headers</span></span>

| <span data-ttu-id="70392-128">Имя</span><span class="sxs-lookup"><span data-stu-id="70392-128">Name</span></span>          | <span data-ttu-id="70392-129">Описание</span><span class="sxs-lookup"><span data-stu-id="70392-129">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="70392-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="70392-130">Authorization</span></span> | <span data-ttu-id="70392-p103">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="70392-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="70392-133">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="70392-133">If-None-Match</span></span> | <span data-ttu-id="70392-134">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="70392-134">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="70392-135">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="70392-135">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="70392-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="70392-136">Response</span></span>

<span data-ttu-id="70392-137">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="70392-137">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="70392-138">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="70392-138">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="70392-139">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="70392-139">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="70392-140">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="70392-140">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="70392-141">Report Refresh Date (дата обновления отчета)</span><span class="sxs-lookup"><span data-stu-id="70392-141">Report Refresh Date</span></span>
- <span data-ttu-id="70392-142">Mailbox Storage Used (Byte) [занято почтовыми ящиками (байт)]</span><span class="sxs-lookup"><span data-stu-id="70392-142">Mailbox Storage Used (Byte)</span></span>
- <span data-ttu-id="70392-143">Site Storage Used (Byte) [занято сайтами (байт)]</span><span class="sxs-lookup"><span data-stu-id="70392-143">Site Storage Used (Byte)</span></span>
- <span data-ttu-id="70392-144">Report Date (дата отчета)</span><span class="sxs-lookup"><span data-stu-id="70392-144">Report Date</span></span>
- <span data-ttu-id="70392-145">"Report Period" (Отчетный период).</span><span class="sxs-lookup"><span data-stu-id="70392-145">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="70392-146">Пример</span><span class="sxs-lookup"><span data-stu-id="70392-146">Example</span></span>

#### <a name="request"></a><span data-ttu-id="70392-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="70392-147">Request</span></span>

<span data-ttu-id="70392-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="70392-148">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitystorage"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365GroupsActivityStorage(period='D7')
```

#### <a name="response"></a><span data-ttu-id="70392-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="70392-149">Response</span></span>

<span data-ttu-id="70392-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="70392-150">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="70392-151">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="70392-151">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Mailbox Storage Used (Byte),Site Storage Used (Byte),Report Date,Report Period
```
