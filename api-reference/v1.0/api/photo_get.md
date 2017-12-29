# <a name="get-photo"></a><span data-ttu-id="652b1-101">Получение фотографии</span><span class="sxs-lookup"><span data-stu-id="652b1-101">Get photo</span></span>

<span data-ttu-id="652b1-102">Получение свойств и связей объекта фотографии.</span><span class="sxs-lookup"><span data-stu-id="652b1-102">Retrieve the properties and relationships of photo object.</span></span>
## <a name="permissions"></a><span data-ttu-id="652b1-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="652b1-103">Permissions</span></span>
<span data-ttu-id="652b1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="652b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="652b1-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="652b1-106">Permission type</span></span>      | <span data-ttu-id="652b1-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="652b1-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="652b1-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="652b1-108">Delegated (work or school account)</span></span> | <span data-ttu-id="652b1-109">Files.Read</span><span class="sxs-lookup"><span data-stu-id="652b1-109">Files.Read</span></span>    |
|<span data-ttu-id="652b1-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="652b1-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="652b1-111">Files.Read</span><span class="sxs-lookup"><span data-stu-id="652b1-111">Files.Read</span></span>    |
|<span data-ttu-id="652b1-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="652b1-112">Application</span></span> | <span data-ttu-id="652b1-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="652b1-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="652b1-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="652b1-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/photo
GET /groups/{id}/photo
GET /drive/root/createdByUser/photo
```
## <a name="optional-query-parameters"></a><span data-ttu-id="652b1-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="652b1-115">Optional query parameters</span></span>
<span data-ttu-id="652b1-116">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/ru-RU/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="652b1-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/ru-RU/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="652b1-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="652b1-117">Request headers</span></span>
| <span data-ttu-id="652b1-118">Имя</span><span class="sxs-lookup"><span data-stu-id="652b1-118">Name</span></span>       | <span data-ttu-id="652b1-119">Тип</span><span class="sxs-lookup"><span data-stu-id="652b1-119">Type</span></span> | <span data-ttu-id="652b1-120">Описание</span><span class="sxs-lookup"><span data-stu-id="652b1-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="652b1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="652b1-121">Authorization</span></span>  | <span data-ttu-id="652b1-122">string</span><span class="sxs-lookup"><span data-stu-id="652b1-122">string</span></span>  | <span data-ttu-id="652b1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="652b1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="652b1-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="652b1-125">Request body</span></span>
<span data-ttu-id="652b1-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="652b1-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="652b1-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="652b1-127">Response</span></span>

<span data-ttu-id="652b1-128">В случае успеха этот метод возвращает код отклика `200 OK` и объект [photo](../resources/photo.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="652b1-128">If successful, this method returns a `200 OK` response code and [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="652b1-129">Пример</span><span class="sxs-lookup"><span data-stu-id="652b1-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="652b1-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="652b1-130">Request</span></span>
<span data-ttu-id="652b1-131">Ниже приведен пример запроса на получение метаданных фотографий.</span><span class="sxs-lookup"><span data-stu-id="652b1-131">Here is an example of the request for the user's drives.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photo"
}-->
```http
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
```
##### <a name="response"></a><span data-ttu-id="652b1-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="652b1-132">Response</span></span>
<span data-ttu-id="652b1-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="652b1-133">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.profilePhoto"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 53

{
  "height": 99,
  "width": 99,
  "id": "id-value"
}
```
##### <a name="request"></a><span data-ttu-id="652b1-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="652b1-134">Request</span></span>
<span data-ttu-id="652b1-135">Ниже приведен пример запроса на получение байтов фотографий.</span><span class="sxs-lookup"><span data-stu-id="652b1-135">Here is an example of the request for the user's drives.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photo"
}-->
```http
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo/$value
```
##### <a name="response"></a><span data-ttu-id="652b1-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="652b1-136">Response</span></span>
<span data-ttu-id="652b1-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="652b1-137">Here is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "stream" } -->

```http
HTTP/1.1 200 OK
Cache-Control: private
Content-Type: image/jpeg
ETag: "A19A6498"
request-id: 16e1bff0-6d74-47d6-944c-61707916a74c
client-request-id: 16e1bff0-6d74-47d6-944c-61707916a74c
x-ms-ags-diagnostic: {"ServerInfo":{"DataCenter":"West US","Slice":"SliceA","Ring":"5","ScaleUnit":"003","Host":"AGSFE_IN_14","ADSiteName":"WST"}}
Access-Control-Allow-Origin: *
Access-Control-Expose-Headers: ETag, Location, Preference-Applied, Content-Range, request-id, client-request-id
Duration: 125.9389
Date: Wed, 13 Dec 2017 22:02:17 GMT
Content-Length: 250526

<binary image data>
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
