# <a name="reportroot-getoffice365activationsuserdetail"></a><span data-ttu-id="b67f1-101">reportRoot: getOffice365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="b67f1-101">reportRoot: getOffice365ActivationsUserDetail</span></span>

<span data-ttu-id="b67f1-102">Получите сведения о пользователях, которые активировали Office 365.</span><span class="sxs-lookup"><span data-stu-id="b67f1-102">Get details about users who have activated Office 365.</span></span>

> <span data-ttu-id="b67f1-103">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="b67f1-103">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="b67f1-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b67f1-104">Permissions</span></span>

<span data-ttu-id="b67f1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b67f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="b67f1-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b67f1-107">Permission type</span></span>                        | <span data-ttu-id="b67f1-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b67f1-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b67f1-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b67f1-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="b67f1-110">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b67f1-110">Not supported.</span></span>                           |
| <span data-ttu-id="b67f1-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b67f1-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b67f1-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b67f1-112">Not supported.</span></span>                           |
| <span data-ttu-id="b67f1-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b67f1-113">Application</span></span>                            | <span data-ttu-id="b67f1-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b67f1-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="b67f1-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b67f1-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserDetail
```

## <a name="request-headers"></a><span data-ttu-id="b67f1-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b67f1-116">Request headers</span></span>

| <span data-ttu-id="b67f1-117">Имя</span><span class="sxs-lookup"><span data-stu-id="b67f1-117">Name</span></span>          | <span data-ttu-id="b67f1-118">Описание</span><span class="sxs-lookup"><span data-stu-id="b67f1-118">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="b67f1-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b67f1-119">Authorization</span></span> | <span data-ttu-id="b67f1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b67f1-p102">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="b67f1-122">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="b67f1-122">if-none-match</span></span> | <span data-ttu-id="b67f1-123">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код ответа `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="b67f1-123">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `304 Not Modified` response is returned.</span></span> <span data-ttu-id="b67f1-124">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="b67f1-124">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="b67f1-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="b67f1-125">Response</span></span>

<span data-ttu-id="b67f1-126">В случае успешного выполнения этот метод возвращает ответ `302 Found`, который перенаправляет на URL-адрес с предварительной аутентификацией для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="b67f1-126">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b67f1-127">Этот URL-адрес можно найти в заголовке ответа `Location`.</span><span class="sxs-lookup"><span data-stu-id="b67f1-127">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b67f1-128">URL-адреса с предварительной аутентификацией действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="b67f1-128">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<span data-ttu-id="b67f1-129">CSV-файл содержит столбцы со следующими заголовками.</span><span class="sxs-lookup"><span data-stu-id="b67f1-129">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b67f1-130">Report Refresh Date (дата обновления отчета)</span><span class="sxs-lookup"><span data-stu-id="b67f1-130">Report Refresh Date</span></span>
- <span data-ttu-id="b67f1-131">User Principal Name (имя участника-пользователя)</span><span class="sxs-lookup"><span data-stu-id="b67f1-131">User Principal Name</span></span>
- <span data-ttu-id="b67f1-132">Display Name (отображаемое имя)</span><span class="sxs-lookup"><span data-stu-id="b67f1-132">Display Name</span></span>
- <span data-ttu-id="b67f1-133">Product Type (тип продукта)</span><span class="sxs-lookup"><span data-stu-id="b67f1-133">Product External Content Type</span></span>
- <span data-ttu-id="b67f1-134">Last Activated Date (дата последней активации)</span><span class="sxs-lookup"><span data-stu-id="b67f1-134">Last Activated Date</span></span>
- <span data-ttu-id="b67f1-135">Windows</span><span class="sxs-lookup"><span data-stu-id="b67f1-135">Windows</span></span>
- <span data-ttu-id="b67f1-136">Mac</span><span class="sxs-lookup"><span data-stu-id="b67f1-136">"mac"</span></span>
- <span data-ttu-id="b67f1-137">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="b67f1-137">Windows 10 Mobile</span></span>
- <span data-ttu-id="b67f1-138">iOS</span><span class="sxs-lookup"><span data-stu-id="b67f1-138">iOS</span></span>
- <span data-ttu-id="b67f1-139">Android</span><span class="sxs-lookup"><span data-stu-id="b67f1-139">Android</span></span>

## <a name="example"></a><span data-ttu-id="b67f1-140">Пример</span><span class="sxs-lookup"><span data-stu-id="b67f1-140">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b67f1-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="b67f1-141">Request</span></span>

<span data-ttu-id="b67f1-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b67f1-142">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationsUserDetail
```

#### <a name="response"></a><span data-ttu-id="b67f1-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="b67f1-143">Response</span></span>

<span data-ttu-id="b67f1-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b67f1-144">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="b67f1-145">Скачанный после перенаправления 302 CSV-файл будет иметь следующую схему.</span><span class="sxs-lookup"><span data-stu-id="b67f1-145">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Product Type,Last Activated Date,Windows,Mac,Windows 10 Mobile,iOS,Android
```
