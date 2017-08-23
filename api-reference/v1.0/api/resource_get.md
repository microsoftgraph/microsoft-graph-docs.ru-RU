# <a name="get-resource"></a><span data-ttu-id="228a3-101">Получение ресурса</span><span class="sxs-lookup"><span data-stu-id="228a3-101">Get resource</span></span>

<span data-ttu-id="228a3-102">Получение двоичных данных объекта [resource](../resources/resource.md) файла или изображения.</span><span class="sxs-lookup"><span data-stu-id="228a3-102">Retrieve the binary data of a file or image [resource](../resources/resource.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="228a3-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="228a3-103">Permissions</span></span>
<span data-ttu-id="228a3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="228a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="228a3-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="228a3-106">Permission type</span></span>      | <span data-ttu-id="228a3-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="228a3-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="228a3-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="228a3-108">Delegated (work or school account)</span></span> | <span data-ttu-id="228a3-109">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="228a3-109">Notes.Read, Notes.ReadWrite, Notes.Read.All, or Notes.ReadWrite.All</span></span>    | 
|<span data-ttu-id="228a3-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="228a3-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="228a3-111">Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="228a3-111">Notes.Read, Notes.ReadWrite</span></span>    | 
|<span data-ttu-id="228a3-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="228a3-112">Application</span></span> | <span data-ttu-id="228a3-113">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="228a3-113">Notes.Read, Notes.ReadWrite, Notes.Read.All, or Notes.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="228a3-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="228a3-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/resources/{id}/content
GET /users/{id | userPrincipalName}/onenote/resources/{id}/content
GET /groups/{id}/onenote/resources/{id}/content
GET /sites/{id}/onenote/resources/{id}/content
```

## <a name="request-headers"></a><span data-ttu-id="228a3-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="228a3-115">Request headers</span></span>
| <span data-ttu-id="228a3-116">Имя</span><span class="sxs-lookup"><span data-stu-id="228a3-116">Name</span></span>       | <span data-ttu-id="228a3-117">Тип</span><span class="sxs-lookup"><span data-stu-id="228a3-117">Type</span></span> | <span data-ttu-id="228a3-118">Описание</span><span class="sxs-lookup"><span data-stu-id="228a3-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="228a3-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="228a3-119">Authorization</span></span>  | <span data-ttu-id="228a3-120">string</span><span class="sxs-lookup"><span data-stu-id="228a3-120">string</span></span>  | <span data-ttu-id="228a3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="228a3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="228a3-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="228a3-123">Request body</span></span>
<span data-ttu-id="228a3-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="228a3-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="228a3-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="228a3-125">Response</span></span>

<span data-ttu-id="228a3-126">При успешном выполнении это метод возвращает код отклика `200 OK` и двоичные данные изображения или файла в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="228a3-126">If successful, this method returns a `200 OK` response code and the image or file binary data in the response body.</span></span>

<span data-ttu-id="228a3-127">Примечание. Изображения не будут отображаться непосредственно в браузере, так как для их получения необходима авторизация (как и для остальной части содержимого страницы).</span><span class="sxs-lookup"><span data-stu-id="228a3-127">Note: Images won't render directly in a browser because they require authorization to retrieve them, like the rest of the page content.</span></span>
## <a name="example"></a><span data-ttu-id="228a3-128">Пример</span><span class="sxs-lookup"><span data-stu-id="228a3-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="228a3-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="228a3-129">Request</span></span>
<span data-ttu-id="228a3-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="228a3-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_resource"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/resources/{id}/content
```
##### <a name="response"></a><span data-ttu-id="228a3-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="228a3-131">Response</span></span>
<span data-ttu-id="228a3-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="228a3-132">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->
```http
HTTP/1.1 200 OK

...binary data...
```
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.onenoteResource"
} -->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
