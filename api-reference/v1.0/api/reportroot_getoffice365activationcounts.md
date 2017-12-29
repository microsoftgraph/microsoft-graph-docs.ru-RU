# <a name="reportroot-getoffice365activationcounts"></a><span data-ttu-id="b12b8-101">reportRoot: getOffice365ActivationCounts</span><span class="sxs-lookup"><span data-stu-id="b12b8-101">reportRoot: getOffice365ActivationCounts</span></span>

<span data-ttu-id="b12b8-102">Получите количество активаций Office 365 на компьютерах и мобильных устройствах.</span><span class="sxs-lookup"><span data-stu-id="b12b8-102">Get the count of Office 365 activations on desktops and devices.</span></span>

> <span data-ttu-id="b12b8-103">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: активации Microsoft Office](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="b12b8-103">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="b12b8-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b12b8-104">Permissions</span></span>

<span data-ttu-id="b12b8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b12b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="b12b8-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b12b8-107">Permission type</span></span>                        | <span data-ttu-id="b12b8-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b12b8-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b12b8-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b12b8-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="b12b8-110">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b12b8-110">Not supported.</span></span>                           |
| <span data-ttu-id="b12b8-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b12b8-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b12b8-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b12b8-112">Not supported.</span></span>                           |
| <span data-ttu-id="b12b8-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b12b8-113">Application</span></span>                            | <span data-ttu-id="b12b8-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b12b8-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="b12b8-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b12b8-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationCounts
```

## <a name="request-headers"></a><span data-ttu-id="b12b8-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b12b8-116">Request headers</span></span>

| <span data-ttu-id="b12b8-117">Имя</span><span class="sxs-lookup"><span data-stu-id="b12b8-117">Name</span></span>          | <span data-ttu-id="b12b8-118">Описание</span><span class="sxs-lookup"><span data-stu-id="b12b8-118">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="b12b8-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b12b8-119">Authorization</span></span> | <span data-ttu-id="b12b8-p102">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b12b8-p102">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="b12b8-122">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="b12b8-122">if-none-match</span></span> | <span data-ttu-id="b12b8-123">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="b12b8-123">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `304 Not Modified` response is returned.</span></span> <span data-ttu-id="b12b8-124">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="b12b8-124">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="b12b8-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="b12b8-125">Response</span></span>

<span data-ttu-id="b12b8-126">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="b12b8-126">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b12b8-127">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="b12b8-127">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b12b8-128">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="b12b8-128">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<span data-ttu-id="b12b8-129">CSV-файл содержит столбцы со следующими заголовками.</span><span class="sxs-lookup"><span data-stu-id="b12b8-129">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b12b8-130">Report Refresh Date (Дата обновления отчета)</span><span class="sxs-lookup"><span data-stu-id="b12b8-130">Report Refresh Date</span></span>
- <span data-ttu-id="b12b8-131">Product Type (Тип продукта)</span><span class="sxs-lookup"><span data-stu-id="b12b8-131">Product External Content Type</span></span>
- <span data-ttu-id="b12b8-132">Windows</span><span class="sxs-lookup"><span data-stu-id="b12b8-132">Windows</span></span>
- <span data-ttu-id="b12b8-133">Mac</span><span class="sxs-lookup"><span data-stu-id="b12b8-133">"mac"</span></span>
- <span data-ttu-id="b12b8-134">Android</span><span class="sxs-lookup"><span data-stu-id="b12b8-134">Android</span></span>
- <span data-ttu-id="b12b8-135">iOS</span><span class="sxs-lookup"><span data-stu-id="b12b8-135">iOS</span></span>
- <span data-ttu-id="b12b8-136">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="b12b8-136">Windows 10 Mobile</span></span>

## <a name="example"></a><span data-ttu-id="b12b8-137">Пример</span><span class="sxs-lookup"><span data-stu-id="b12b8-137">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b12b8-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="b12b8-138">Request</span></span>

<span data-ttu-id="b12b8-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b12b8-139">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationcounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationCounts
```

#### <a name="response"></a><span data-ttu-id="b12b8-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="b12b8-140">Response</span></span>

<span data-ttu-id="b12b8-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b12b8-141">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="b12b8-142">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="b12b8-142">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
