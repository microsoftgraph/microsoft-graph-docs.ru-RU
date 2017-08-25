# <a name="get-directory-objects-from-a-list-of-ids"></a><span data-ttu-id="9b63f-101">Получение объектов каталога из списка идентификаторов</span><span class="sxs-lookup"><span data-stu-id="9b63f-101">Get directory objects from a list of ids</span></span>

<span data-ttu-id="9b63f-p101">Возвращает объекты каталогов, указанные в списке идентификаторов.  ПРИМЕЧАНИЕ. Возвращаемые объекты каталогов представляют собой полные объекты, содержащие **все** свойства. Параметр запроса `$select` недоступен для этой операции.</span><span class="sxs-lookup"><span data-stu-id="9b63f-p101">Returns the directory objects specified in a list of ids.  NOTE: The directory objects returned are the full objects containing **all** their properties. The `$select` query option is not available for this operation.</span></span>

<span data-ttu-id="9b63f-105">Ниже перечислены некоторые распространенные случаи использования этой функции.</span><span class="sxs-lookup"><span data-stu-id="9b63f-105">Some common uses for this function are to:</span></span>

* <span data-ttu-id="9b63f-106">Разрешение идентификаторов, возвращаемых как часть коллекций идентификаторов функциями, например [getMemberObjects](directoryobject_getmemberobjects.md) или [getMemberGroups](directoryobject_getmembergroups.md), в базовые объекты каталогов.</span><span class="sxs-lookup"><span data-stu-id="9b63f-106">Resolve ids returned by functions (that return collections of ids) such as [getMemberObjects](directoryobject_getmemberobjects.md) or [getMemberGroups](directoryobject_getmembergroups.md)  to their backing directory objects.</span></span>
* <span data-ttu-id="9b63f-107">Разрешение идентификаторов, которые приложение хранит во внешнем хранилище, в базовые объекты каталогов.</span><span class="sxs-lookup"><span data-stu-id="9b63f-107">Resolve ids persisted in an external store by the application to their backing directory objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="9b63f-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9b63f-108">Permissions</span></span>

<span data-ttu-id="9b63f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9b63f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="9b63f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9b63f-111">Permission type</span></span>      | <span data-ttu-id="9b63f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9b63f-112">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="9b63f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9b63f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="9b63f-114">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9b63f-114">Directory.Read.All, Directory.AccessAsUser.All</span></span>    | 
|<span data-ttu-id="9b63f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9b63f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b63f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b63f-116">Not supported.</span></span>    | 
|<span data-ttu-id="9b63f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9b63f-117">Application</span></span> | <span data-ttu-id="9b63f-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="9b63f-118">Directory.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="9b63f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9b63f-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getById
```

## <a name="request-headers"></a><span data-ttu-id="9b63f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9b63f-120">Request headers</span></span>

| <span data-ttu-id="9b63f-121">Имя</span><span class="sxs-lookup"><span data-stu-id="9b63f-121">Name</span></span>       | <span data-ttu-id="9b63f-122">Тип</span><span class="sxs-lookup"><span data-stu-id="9b63f-122">Type</span></span> | <span data-ttu-id="9b63f-123">Описание</span><span class="sxs-lookup"><span data-stu-id="9b63f-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9b63f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b63f-124">Authorization</span></span>  | <span data-ttu-id="9b63f-125">string</span><span class="sxs-lookup"><span data-stu-id="9b63f-125">string</span></span>  | <span data-ttu-id="9b63f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9b63f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9b63f-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9b63f-128">Content-Type</span></span>  | <span data-ttu-id="9b63f-129">application/json</span><span class="sxs-lookup"><span data-stu-id="9b63f-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9b63f-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9b63f-130">Request body</span></span>

<span data-ttu-id="9b63f-131">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="9b63f-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9b63f-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="9b63f-132">Parameter</span></span>   | <span data-ttu-id="9b63f-133">Тип</span><span class="sxs-lookup"><span data-stu-id="9b63f-133">Type</span></span> |<span data-ttu-id="9b63f-134">Описание</span><span class="sxs-lookup"><span data-stu-id="9b63f-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9b63f-135">ids</span><span class="sxs-lookup"><span data-stu-id="9b63f-135">ids</span></span>|<span data-ttu-id="9b63f-136">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9b63f-136">String collection</span></span>| <span data-ttu-id="9b63f-p104">Коллекция идентификаторов, для которой необходимо возвратить объекты. Вы можете указать до 1000 идентификаторов.</span><span class="sxs-lookup"><span data-stu-id="9b63f-p104">A collection of ids for which to return objects. You can specify up to 1000 ids.</span></span> |
|<span data-ttu-id="9b63f-139">types</span><span class="sxs-lookup"><span data-stu-id="9b63f-139">types</span></span>|<span data-ttu-id="9b63f-140">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9b63f-140">String collection</span></span>| <span data-ttu-id="9b63f-p105">Коллекция типов ресурсов, указывающая набор коллекций ресурсов, в котором необходимо выполнить поиск. Если аргумент не указан, по умолчанию используется объект [directoryObject](../resources/directoryobject.md), который содержит все типы ресурсов, определенные в каталоге. В коллекции можно указать любой объект, производный от `directoryObject`. Пример: [user](../resources/user.md), [group](../resources/group.md), [device](../resources/device.md). В значениях не учитывается регистр символов.</span><span class="sxs-lookup"><span data-stu-id="9b63f-p105">A collection of resource types that specifies the set of resource collections to search. If not specified, the default is [directoryObject](../resources/directoryobject.md), which contains all of the resource types defined in the directory. Any object that derives from `directoryObject` may be specified in the collection; for example: [user](../resources/user.md), [group](../resources/group.md), [device](../resources/device.md), and so on. The values are not case sensitive.</span></span>|

## <a name="response"></a><span data-ttu-id="9b63f-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b63f-145">Response</span></span>

<span data-ttu-id="9b63f-146">В случае успеха этот метод возвращает код отклика `200, OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9b63f-146">If successful, this method returns `200, OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b63f-147">Пример</span><span class="sxs-lookup"><span data-stu-id="9b63f-147">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9b63f-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="9b63f-148">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryobject_getById"
}-->

```http
POST https://graph.microsoft.com/v1.0/directoryObjects/getByIds
Content-type: application/json

{
    "ids":["84b80893-8749-40a3-97b7-68513b600544","5d6059b6-368d-45f8-91e1-8e07d485f1d0"],
    "types":["user"]
}
```

##### <a name="response"></a><span data-ttu-id="9b63f-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b63f-149">Response</span></span>

<span data-ttu-id="9b63f-p106">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9b63f-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#directoryObjects",
    "value": [
      {
        "@odata.type": "#microsoft.graph.user",
        "id": "84b80893-8749-40a3-97b7-68513b600544",
        "accountEnabled": true,
        "displayName": "Trevor Jones"
      },
      {
        "@odata.type": "#microsoft.graph.user",
        "id": "84b80893-8749-40a3-97b7-68513b600544",
        "accountEnabled": true,
        "displayName": "Billy Smith"
      }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getById",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
