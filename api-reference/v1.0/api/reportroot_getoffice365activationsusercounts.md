# <a name="reportroot-getoffice365activationsusercounts"></a><span data-ttu-id="2bae1-101">reportRoot: getOffice365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="2bae1-101">reportRoot: getOffice365ActivationsUserCounts</span></span>

<span data-ttu-id="2bae1-102">Узнайте, сколько пользователей есть и сколько из них активировали подписку на Office на компьютере или мобильном устройстве.</span><span class="sxs-lookup"><span data-stu-id="2bae1-102">Get the count of users that are enabled and those that have activated the Office subscription on desktop or devices.</span></span>

> <span data-ttu-id="2bae1-103">**Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: активации Microsoft Office](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span><span class="sxs-lookup"><span data-stu-id="2bae1-103">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).</span></span>

## <a name="permissions"></a><span data-ttu-id="2bae1-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2bae1-104">Permissions</span></span>

<span data-ttu-id="2bae1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2bae1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="2bae1-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2bae1-107">Permission type</span></span>                        | <span data-ttu-id="2bae1-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2bae1-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="2bae1-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2bae1-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="2bae1-110">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2bae1-110">Reports.Read.All</span></span>                         |
| <span data-ttu-id="2bae1-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2bae1-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2bae1-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2bae1-112">Not supported.</span></span>                           |
| <span data-ttu-id="2bae1-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2bae1-113">Application</span></span>                            | <span data-ttu-id="2bae1-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2bae1-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="2bae1-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2bae1-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserCounts
```

## <a name="request-headers"></a><span data-ttu-id="2bae1-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2bae1-116">Request headers</span></span>

| <span data-ttu-id="2bae1-117">Имя</span><span class="sxs-lookup"><span data-stu-id="2bae1-117">Name</span></span>          | <span data-ttu-id="2bae1-118">Описание</span><span class="sxs-lookup"><span data-stu-id="2bae1-118">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="2bae1-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2bae1-119">Authorization</span></span> | <span data-ttu-id="2bae1-p102">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2bae1-p102">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="2bae1-122">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="2bae1-122">If-None-Match</span></span> | <span data-ttu-id="2bae1-123">Если этот заголовок запроса включен, а указанный eTag совпадает с текущим тегом файла, то будет возвращен код отклика `304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="2bae1-123">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="2bae1-124">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="2bae1-124">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="2bae1-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="2bae1-125">Response</span></span>

<span data-ttu-id="2bae1-126">В случае успешного выполнения этот метод возвращает отклик `302 Found`, который перенаправляет на URL-адрес, для которого выполнена предварительная аутентификация, для скачивания отчета.</span><span class="sxs-lookup"><span data-stu-id="2bae1-126">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="2bae1-127">Этот URL-адрес можно найти в заголовке `Location` отклика.</span><span class="sxs-lookup"><span data-stu-id="2bae1-127">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="2bae1-128">URL-адреса для скачивания, для которых выполнена предварительная аутентификация, действительны в течение нескольких минут и не требуют заголовка `Authorization`.</span><span class="sxs-lookup"><span data-stu-id="2bae1-128">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="2bae1-129">CSV-файл содержит столбцы со следующими заголовками:</span><span class="sxs-lookup"><span data-stu-id="2bae1-129">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="2bae1-130">"Report Refresh Date" (Дата обновления отчета);</span><span class="sxs-lookup"><span data-stu-id="2bae1-130">Report Refresh Date</span></span>
- <span data-ttu-id="2bae1-131">"Product Type" (Тип продукта);</span><span class="sxs-lookup"><span data-stu-id="2bae1-131">Product Type</span></span>
- <span data-ttu-id="2bae1-132">"Assigned" (Назначенные);</span><span class="sxs-lookup"><span data-stu-id="2bae1-132">Assigned</span></span>
- <span data-ttu-id="2bae1-133">"Activated" (Активированные).</span><span class="sxs-lookup"><span data-stu-id="2bae1-133">Activated</span></span>

## <a name="example"></a><span data-ttu-id="2bae1-134">Пример</span><span class="sxs-lookup"><span data-stu-id="2bae1-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="2bae1-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="2bae1-135">Request</span></span>

<span data-ttu-id="2bae1-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2bae1-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationsUserCounts
```

#### <a name="response"></a><span data-ttu-id="2bae1-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="2bae1-137">Response</span></span>

<span data-ttu-id="2bae1-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2bae1-138">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="2bae1-139">У скачанного после перенаправления 302 CSV-файла будет приведенная ниже схема.</span><span class="sxs-lookup"><span data-stu-id="2bae1-139">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Product Type,Assigned,Activated
```
