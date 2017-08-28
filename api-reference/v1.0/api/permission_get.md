# <a name="get-permission"></a><span data-ttu-id="e43a9-101">Получение разрешения</span><span class="sxs-lookup"><span data-stu-id="e43a9-101">Get permission</span></span>

<span data-ttu-id="e43a9-102">Получение свойств и связей объекта разрешений.</span><span class="sxs-lookup"><span data-stu-id="e43a9-102">Retrieve the properties and relationships of permission object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e43a9-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e43a9-103">Permissions</span></span>
<span data-ttu-id="e43a9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e43a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e43a9-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e43a9-106">Permission type</span></span>      | <span data-ttu-id="e43a9-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e43a9-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e43a9-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e43a9-108">Delegated (work or school account)</span></span> | <span data-ttu-id="e43a9-109">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e43a9-109">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="e43a9-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e43a9-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e43a9-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e43a9-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="e43a9-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e43a9-112">Application</span></span> | <span data-ttu-id="e43a9-113">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e43a9-113">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e43a9-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e43a9-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{item-id}/permissions/{perm-id}
GET /me/drive/root:/{path}:/permissions/{perm-id}
GET /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
GET /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e43a9-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e43a9-115">Optional query parameters</span></span>
<span data-ttu-id="e43a9-116">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e43a9-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-body"></a><span data-ttu-id="e43a9-117">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e43a9-117">Request body</span></span>
<span data-ttu-id="e43a9-118">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e43a9-118">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e43a9-119">Отклик</span><span class="sxs-lookup"><span data-stu-id="e43a9-119">Response</span></span>

<span data-ttu-id="e43a9-120">В случае успеха этот метод возвращает код отклика `200 OK` и ресурс [Permission](../resources/permission.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e43a9-120">If successful, this method returns a `200 OK` response code and [Permission](../resources/permission.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e43a9-121">Пример</span><span class="sxs-lookup"><span data-stu-id="e43a9-121">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e43a9-122">Запрос</span><span class="sxs-lookup"><span data-stu-id="e43a9-122">Request</span></span>

<span data-ttu-id="e43a9-123">Ниже приведен пример запроса на доступ к разрешению для корневой папки.</span><span class="sxs-lookup"><span data-stu-id="e43a9-123">Here is an example of the request to access a permission on the root folder.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_permission"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/permissions/{perm-id}
```
##### <a name="response"></a><span data-ttu-id="e43a9-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="e43a9-124">Response</span></span>
<span data-ttu-id="e43a9-125">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e43a9-125">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 762

{
  "grantedTo": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "efee1b77-fb3b-4f65-99d6-274c11914d12"
    }
  },
  "id": "1",
  "roles": [ "write" ]
}
```

## <a name="remarks"></a><span data-ttu-id="e43a9-126">Заметки</span><span class="sxs-lookup"><span data-stu-id="e43a9-126">Remarks</span></span>

<span data-ttu-id="e43a9-127">Ресурс [Permission](../resources/permission.md) использует _аспекты_ для предоставления сведений о типе разрешения, представленного ресурсом.</span><span class="sxs-lookup"><span data-stu-id="e43a9-127">The [Permission](../resources/permission.md) resource uses _facets_ to provide information about the kind of permission represented by the resource.</span></span>

<span data-ttu-id="e43a9-p102">Разрешения с аспектом [**link**](../resources/sharinglink.md) представляют ссылки для предоставления общего доступа, созданные для элемента. Такие ссылки содержат уникальный токен, предоставляющий доступ к элементу для любого пользователя, воспользовавшегося ссылкой.</span><span class="sxs-lookup"><span data-stu-id="e43a9-p102">Permissions with a [**link**](../resources/sharinglink.md) facet represent sharing links created on the item. Sharing links contain a unique token that provides access to the item for anyone with the link.</span></span>

<span data-ttu-id="e43a9-130">Разрешения с аспектом [**invitation**](../resources/sharinginvitation.md) представляют разрешения, добавленные при приглашении определенных пользователей или групп поработать с файлом.</span><span class="sxs-lookup"><span data-stu-id="e43a9-130">Permissions with a [**invitation**](../resources/sharinginvitation.md) facet represent permissions added by inviting specific users or groups to have access to the file.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get permission",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Get permission"
}-->
