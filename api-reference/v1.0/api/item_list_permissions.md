# <a name="list-permissions-on-a-driveitem"></a><span data-ttu-id="8a012-101">Создание списка разрешений для доступа к ресурсу DriveItem</span><span class="sxs-lookup"><span data-stu-id="8a012-101">List permissions on a DriveItem</span></span>

<span data-ttu-id="8a012-102">Создание списка действующих разрешений для доступа к ресурсу [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="8a012-102">List the effective permissions of on a [DriveItem](../resources/driveitem.md).</span></span>

<span data-ttu-id="8a012-p101">Связи между **разрешениями** ресурса DriveItem невозможно развернуть как часть запроса на [получение DriveItem](item_get.md) или коллекции DriveItems. Необходимо открыть доступ непосредственно к свойству разрешений.</span><span class="sxs-lookup"><span data-stu-id="8a012-p101">The **permissions** relationship of DriveItem cannot be expanded as part of a call to [get DriveItem](item_get.md) or a collection of DriveItems. You must access the permissions property directly.</span></span>

## <a name="access-to-permissions"></a><span data-ttu-id="8a012-105">Доступ к разрешениям</span><span class="sxs-lookup"><span data-stu-id="8a012-105">Access to Permissions</span></span>

<span data-ttu-id="8a012-106">Коллекция разрешений включает потенциально конфиденциальные данные и может быть недоступна для каждого абонента.</span><span class="sxs-lookup"><span data-stu-id="8a012-106">The permissions collection includes potentially sensitive information and may not be available for every caller.</span></span>

* <span data-ttu-id="8a012-p102">Все разрешения будут возвращены владельцу элемента. Включает совладельцев.</span><span class="sxs-lookup"><span data-stu-id="8a012-p102">For the owner of the item, all permissions will be returned. This includes co-owners.</span></span>
* <span data-ttu-id="8a012-109">Абоненту, который не является владельцем, возвращаются только применяемые к нему разрешения.</span><span class="sxs-lookup"><span data-stu-id="8a012-109">For a non-owner caller, only the permissions that apply to the caller are returned.</span></span>
* <span data-ttu-id="8a012-110">Свойства разрешений, которые содержат секреты (например, `shareId` и `webUrl`), возвращаются только для вызывающих, которые могут создать разрешение.</span><span class="sxs-lookup"><span data-stu-id="8a012-110">Permission properties that contain secrets (e.g. `shareId` and `webUrl`) are only returned for callers that are able to create the Permission.</span></span>

## <a name="permissions"></a><span data-ttu-id="8a012-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8a012-111">Permissions</span></span>
<span data-ttu-id="8a012-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8a012-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8a012-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8a012-114">Permission type</span></span>      | <span data-ttu-id="8a012-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8a012-115">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="8a012-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8a012-116">Delegated (work or school account)</span></span> | <span data-ttu-id="8a012-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a012-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    | 
|<span data-ttu-id="8a012-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8a012-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a012-119">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a012-119">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    | 
|<span data-ttu-id="8a012-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8a012-120">Application</span></span> | <span data-ttu-id="8a012-121">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a012-121">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="8a012-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8a012-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{item-id}/permissions
GET /me/drive/root:/{path}:/permissions
GET /drives/{drive-id}/items/{item-id}/permissions
GET /groups/{group-id}/drive/items/{item-id}/permissions
```

## <a name="request-headers"></a><span data-ttu-id="8a012-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8a012-123">Request headers</span></span>

| <span data-ttu-id="8a012-124">Имя</span><span class="sxs-lookup"><span data-stu-id="8a012-124">Name</span></span>          | <span data-ttu-id="8a012-125">Тип</span><span class="sxs-lookup"><span data-stu-id="8a012-125">Type</span></span>   | <span data-ttu-id="8a012-126">Описание</span><span class="sxs-lookup"><span data-stu-id="8a012-126">Description</span></span>                                                                                                                                     |
|:--------------|:-------|:------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="8a012-127">if-none-match</span><span class="sxs-lookup"><span data-stu-id="8a012-127">if-none-match</span></span> | <span data-ttu-id="8a012-128">string</span><span class="sxs-lookup"><span data-stu-id="8a012-128">string</span></span> | <span data-ttu-id="8a012-129">Если указан заголовок запроса, а предоставленный тег etag совпадает с текущим тегом etag элемента, то возвращается отклик `HTTP 304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="8a012-129">If this request header is included and the etag provided matches the current etag on the item, an `HTTP 304 Not Modified` response is returned.</span></span> |


## <a name="optional-query-parameters"></a><span data-ttu-id="8a012-130">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8a012-130">Optional query parameters</span></span>
<span data-ttu-id="8a012-131">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8a012-131">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-body"></a><span data-ttu-id="8a012-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8a012-132">Request body</span></span>
<span data-ttu-id="8a012-133">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8a012-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8a012-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a012-134">Response</span></span>

<span data-ttu-id="8a012-135">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию ресурсов [Permission](../resources/permission.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8a012-135">If successful, this method returns a `200 OK` response code and collection of [Permission](../resources/permission.md) resources in the response body.</span></span>

<span data-ttu-id="8a012-136">Действующие разрешения элемента могут поступать из двух источников:</span><span class="sxs-lookup"><span data-stu-id="8a012-136">Effective permissions of an item can come from two sources:</span></span>

* <span data-ttu-id="8a012-137">разрешения, которые были применены непосредственно к самому элементу;</span><span class="sxs-lookup"><span data-stu-id="8a012-137">Permissions applied directly on the item itself</span></span>
* <span data-ttu-id="8a012-138">разрешения, унаследованные от предшествующих элементов.</span><span class="sxs-lookup"><span data-stu-id="8a012-138">Permissions inherited from the item's ancestors</span></span>

<span data-ttu-id="8a012-p104">Абоненты могут распознать унаследованное разрешение, проверив свойство **inheritedFrom**. Это свойство — ресурс [**itemReference**](../resources/itemreference.md), отсылающий к предшествующему элементу, от которого унаследовано разрешение.</span><span class="sxs-lookup"><span data-stu-id="8a012-p104">Callers can differentiate if the permission is inherited or not by checking the **inheritedFrom** property. This property is an [**itemReference**](../resources/itemreference.md) resource referencing the ancestor that the permission is inherited from.</span></span>

## <a name="example"></a><span data-ttu-id="8a012-141">Пример</span><span class="sxs-lookup"><span data-stu-id="8a012-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8a012-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="8a012-142">Request</span></span>
<span data-ttu-id="8a012-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8a012-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_permissions"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/permissions
```


##### <a name="response"></a><span data-ttu-id="8a012-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a012-144">Response</span></span>
<span data-ttu-id="8a012-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8a012-145">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "1",
      "roles": ["write"],
      "link": {
        "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
        "type": "edit"
      }
    },
    {
      "id": "2",
      "roles": ["write"],
      "grantedTo": {
        "user": {
          "id": "5D33DD65C6932946",
          "displayName": "John Doe"
        }
      },
      "inheritedFrom": {
        "driveId": "1234567890ABD",
        "id": "1234567890ABC!123",
        "path": "/drive/root:/Documents" }
    },
    {
      "id": "3",
      "roles": ["write"],
      "link": {
        "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
        "type": "edit",
        "application": {
          "id": "12345",
          "displayName": "TimeTravelPlus"
        }
      }
    }
  ]
}
```

<span data-ttu-id="8a012-146">Дополнительные сведения о том, как получить единый ресурс разрешения см. в статье [Получение разрешения](permission_get.md).</span><span class="sxs-lookup"><span data-stu-id="8a012-146">See [Get permission](permission_get.md) for more details on retrieving a single permission resource.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List permissions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/List permissions"
}-->
