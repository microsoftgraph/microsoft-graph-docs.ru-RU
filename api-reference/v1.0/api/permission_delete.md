# <a name="delete-permission"></a><span data-ttu-id="26be9-101">Удаление разрешения</span><span class="sxs-lookup"><span data-stu-id="26be9-101">Delete permission</span></span>

<span data-ttu-id="26be9-102">Отмена доступа к ресурсу [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="26be9-102">Remove access to a [DriveItem](../resources/driveitem.md).</span></span>

<span data-ttu-id="26be9-p101">Удалять можно только те разрешения, которые не были унаследованы. Свойство **inheritedFrom** должно иметь значение `null`.</span><span class="sxs-lookup"><span data-stu-id="26be9-p101">Only permissions that are not inherited can be deleted. The **inheritedFrom** property must be `null`.</span></span>

## <a name="permissions"></a><span data-ttu-id="26be9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="26be9-105">Permissions</span></span>
<span data-ttu-id="26be9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="26be9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="26be9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="26be9-108">Permission type</span></span>      | <span data-ttu-id="26be9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="26be9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="26be9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="26be9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="26be9-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26be9-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="26be9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="26be9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26be9-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26be9-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="26be9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="26be9-114">Application</span></span> | <span data-ttu-id="26be9-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26be9-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="26be9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="26be9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /me/drive/items/{item-id}/permissions/{perm-id}
DELETE /me/drive/root:/{path}:/permissions/{perm-id}
DELETE /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
DELETE /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
```

## <a name="request-headers"></a><span data-ttu-id="26be9-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="26be9-117">Request headers</span></span>

| <span data-ttu-id="26be9-118">Имя</span><span class="sxs-lookup"><span data-stu-id="26be9-118">Name</span></span>          | <span data-ttu-id="26be9-119">Тип</span><span class="sxs-lookup"><span data-stu-id="26be9-119">Type</span></span>   | <span data-ttu-id="26be9-120">Описание</span><span class="sxs-lookup"><span data-stu-id="26be9-120">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="26be9-121">if-match</span><span class="sxs-lookup"><span data-stu-id="26be9-121">if-match</span></span>      | <span data-ttu-id="26be9-122">string</span><span class="sxs-lookup"><span data-stu-id="26be9-122">string</span></span> | <span data-ttu-id="26be9-123">Если указан заголовок запроса, а предоставленный тег eTag (или cTag) не совпадает с текущим тегом элемента, то возвращается отклик `412 Precondition Failed`, а элемент не удаляется.</span><span class="sxs-lookup"><span data-stu-id="26be9-123">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="request-body"></a><span data-ttu-id="26be9-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="26be9-124">Request body</span></span>
<span data-ttu-id="26be9-125">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="26be9-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="26be9-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="26be9-126">Response</span></span>

<span data-ttu-id="26be9-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="26be9-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26be9-129">Пример</span><span class="sxs-lookup"><span data-stu-id="26be9-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="26be9-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="26be9-130">Request</span></span>

<span data-ttu-id="26be9-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="26be9-131">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_permission"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/drive/root/items/{item-id}/permissions/{perm-id}
```

##### <a name="response"></a><span data-ttu-id="26be9-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="26be9-132">Response</span></span>

<span data-ttu-id="26be9-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="26be9-133">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="remarks"></a><span data-ttu-id="26be9-134">Заметки</span><span class="sxs-lookup"><span data-stu-id="26be9-134">Remarks</span></span>

* <span data-ttu-id="26be9-135">[Диски](../resources/drive.md), у которых для свойства **driveType** задано значение `personal` (личное хранилище OneDrive), не могут создавать и изменять разрешения в корневом ресурсе DriveItem.</span><span class="sxs-lookup"><span data-stu-id="26be9-135">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive Personal) cannot create or modify permissions on the root DriveItem.</span></span> 

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete permission",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Delete permission"
}-->
