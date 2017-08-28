# <a name="update-permission"></a><span data-ttu-id="dac74-101">Обновление разрешения</span><span class="sxs-lookup"><span data-stu-id="dac74-101">Update permission</span></span>

<span data-ttu-id="dac74-102">Обновление свойств разрешения путем обновления ресурса.</span><span class="sxs-lookup"><span data-stu-id="dac74-102">Update the properties of a permission by patching the resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="dac74-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dac74-103">Permissions</span></span>

<span data-ttu-id="dac74-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="dac74-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="dac74-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dac74-106">Permission type</span></span>      | <span data-ttu-id="dac74-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dac74-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dac74-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dac74-108">Delegated (work or school account)</span></span> | <span data-ttu-id="dac74-109">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dac74-109">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="dac74-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dac74-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dac74-111">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dac74-111">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="dac74-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dac74-112">Application</span></span> | <span data-ttu-id="dac74-113">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dac74-113">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dac74-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dac74-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{item-id}/permissions/{perm-id}
PATCH /me/drive/root:/{path}:/permissions/{perm-id}
PATCH /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
PATCH /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="request-headers"></a><span data-ttu-id="dac74-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dac74-115">Request headers</span></span>

| <span data-ttu-id="dac74-116">Имя</span><span class="sxs-lookup"><span data-stu-id="dac74-116">Name</span></span>          | <span data-ttu-id="dac74-117">Тип</span><span class="sxs-lookup"><span data-stu-id="dac74-117">Type</span></span>   | <span data-ttu-id="dac74-118">Описание</span><span class="sxs-lookup"><span data-stu-id="dac74-118">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="dac74-119">if-match</span><span class="sxs-lookup"><span data-stu-id="dac74-119">if-match</span></span>      | <span data-ttu-id="dac74-120">string</span><span class="sxs-lookup"><span data-stu-id="dac74-120">string</span></span> | <span data-ttu-id="dac74-121">Если указан заголовок запроса, а предоставленный тег eTag (или cTag) не совпадает с текущим тегом элемента, то возвращается отклик `412 Precondition Failed`, а элемент не удаляется.</span><span class="sxs-lookup"><span data-stu-id="dac74-121">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dac74-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dac74-122">Request body</span></span>
<span data-ttu-id="dac74-p102">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="dac74-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="dac74-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="dac74-126">Property</span></span>     | <span data-ttu-id="dac74-127">Тип</span><span class="sxs-lookup"><span data-stu-id="dac74-127">Type</span></span>   | <span data-ttu-id="dac74-128">Описание</span><span class="sxs-lookup"><span data-stu-id="dac74-128">Description</span></span>                   |
|:-------------|:-------|:------------------------------|
| <span data-ttu-id="dac74-129">**roles**</span><span class="sxs-lookup"><span data-stu-id="dac74-129">**roles**</span></span>    | <span data-ttu-id="dac74-130">String</span><span class="sxs-lookup"><span data-stu-id="dac74-130">String</span></span> | <span data-ttu-id="dac74-131">Массив типов разрешений.</span><span class="sxs-lookup"><span data-stu-id="dac74-131">An array of permission types.</span></span> |

## <a name="response"></a><span data-ttu-id="dac74-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="dac74-132">Response</span></span>

<span data-ttu-id="dac74-133">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [permission](../resources/permission.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dac74-133">If successful, this method returns a `200 OK` response code and updated [permission](../resources/permission.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dac74-134">Пример</span><span class="sxs-lookup"><span data-stu-id="dac74-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="dac74-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="dac74-135">Request</span></span>

<span data-ttu-id="dac74-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dac74-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_permission"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/permissions/{perm-id}
Content-type: application/json

{
  "roles": [ "read" ]
}
```
##### <a name="response"></a><span data-ttu-id="dac74-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="dac74-137">Response</span></span>

<span data-ttu-id="dac74-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="dac74-138">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "grantedTo": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "efee1b77-fb3b-4f65-99d6-274c11914d12"
    }
  },
  "id": "1",
  "roles": [ "read" ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update permission",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Update permission"
}-->
