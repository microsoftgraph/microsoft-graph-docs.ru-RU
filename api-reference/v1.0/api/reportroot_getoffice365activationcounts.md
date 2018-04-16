# <a name="reportroot-getoffice365activationcounts"></a><span data-ttu-id="27324-101">reportRoot: getOffice365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="27324-101">reportRoot: getOffice365ActivationCounts</span></span>

<span data-ttu-id="27324-102">Получите количество активаций Office 365 на компьютерах и мобильных устройствах.</span><span class="sxs-lookup"><span data-stu-id="27324-102">Get the count of Office 365 activations on desktops and devices.</span></span>

> <span data-ttu-id="27324-103">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: активации Microsoft Office](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="27324-103">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="27324-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="27324-104">Permissions</span></span>

<span data-ttu-id="27324-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="27324-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="27324-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="27324-107">Permission type</span></span>                        | <span data-ttu-id="27324-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="27324-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="27324-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="27324-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="27324-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="27324-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="27324-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="27324-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27324-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27324-112">Not supported.</span></span>                           |
| <span data-ttu-id="27324-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="27324-113">Application</span></span>                            | <span data-ttu-id="27324-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="27324-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="27324-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="27324-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationCounts
```

## <a name="request-headers"></a><span data-ttu-id="27324-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="27324-116">Request headers</span></span>

| <span data-ttu-id="27324-117">Имя</span><span class="sxs-lookup"><span data-stu-id="27324-117">Name</span></span>          | <span data-ttu-id="27324-118">Описание</span><span class="sxs-lookup"><span data-stu-id="27324-118">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="27324-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="27324-119">Authorization</span></span> | <span data-ttu-id="27324-p102">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="27324-p102">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="27324-122">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="27324-122">If-None-Match</span></span> | <span data-ttu-id="27324-123">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="27324-123">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="27324-124">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="27324-124">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="27324-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="27324-125">Response</span></span>

<span data-ttu-id="27324-126">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="27324-126">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="27324-127">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="27324-127">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="27324-128">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="27324-128">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="27324-129">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="27324-129">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="27324-130">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="27324-130">Report Refresh Date</span></span>
- <span data-ttu-id="27324-131">Product Type (Тип продукта)</span><span class="sxs-lookup"><span data-stu-id="27324-131">Product Type</span></span>
- <span data-ttu-id="27324-132">Windows</span><span class="sxs-lookup"><span data-stu-id="27324-132">Windows</span></span>
- <span data-ttu-id="27324-133">Mac</span><span class="sxs-lookup"><span data-stu-id="27324-133">Mac</span></span>
- <span data-ttu-id="27324-134">Android</span><span class="sxs-lookup"><span data-stu-id="27324-134">Android</span></span>
- <span data-ttu-id="27324-135">iOS</span><span class="sxs-lookup"><span data-stu-id="27324-135">iOS</span></span>
- <span data-ttu-id="27324-136">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="27324-136">Windows 10 Mobile</span></span>

## <a name="example"></a><span data-ttu-id="27324-137">Пример</span><span class="sxs-lookup"><span data-stu-id="27324-137">Example</span></span>

#### <a name="request"></a><span data-ttu-id="27324-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="27324-138">Request</span></span>

<span data-ttu-id="27324-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="27324-139">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationcounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationCounts
```

#### <a name="response"></a><span data-ttu-id="27324-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="27324-140">Response</span></span>

<span data-ttu-id="27324-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="27324-141">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="27324-142">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="27324-142">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Product Type,Windows,Mac,Android,iOS,Windows 10 Mobile
```
