# <a name="get-directory-objects-from-a-list-of-ids"></a><span data-ttu-id="183f4-101">Получение объектов каталога из списка идентификаторов</span><span class="sxs-lookup"><span data-stu-id="183f4-101">Get directory objects from a list of ids</span></span>

<span data-ttu-id="183f4-p101">Возвращает объекты каталогов, указанные в списке идентификаторов.  ПРИМЕЧАНИЕ. Возвращаемые объекты каталогов представляют собой полные объекты, содержащие **все** свойства. Параметр запроса `$select` недоступен для этой операции.</span><span class="sxs-lookup"><span data-stu-id="183f4-p101">Returns the directory objects specified in a list of ids.  NOTE: The directory objects returned are the full objects containing **all** their properties. The `$select` query option is not available for this operation.</span></span>

<span data-ttu-id="183f4-105">Ниже перечислены некоторые распространенные случаи использования этой функции.</span><span class="sxs-lookup"><span data-stu-id="183f4-105">Some common uses for this function are to:</span></span>

* <span data-ttu-id="183f4-106">Разрешение идентификаторов, возвращаемых как часть коллекций идентификаторов функциями, например [getMemberObjects](directoryobject_getmemberobjects.md) или [getMemberGroups](directoryobject_getmembergroups.md), в базовые объекты каталогов.</span><span class="sxs-lookup"><span data-stu-id="183f4-106">Resolve ids returned by functions (that return collections of ids) such as [getMemberObjects](directoryobject_getmemberobjects.md) or [getMemberGroups](directoryobject_getmembergroups.md)  to their backing directory objects.</span></span>
* <span data-ttu-id="183f4-107">Разрешение идентификаторов, которые приложение хранит во внешнем хранилище, в базовые объекты каталогов.</span><span class="sxs-lookup"><span data-stu-id="183f4-107">Resolve ids persisted in an external store by the application to their backing directory objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="183f4-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="183f4-108">Permissions</span></span>

<span data-ttu-id="183f4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="183f4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="183f4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="183f4-111">Permission type</span></span>      | <span data-ttu-id="183f4-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="183f4-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="183f4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="183f4-113">Delegated (work or school account)</span></span> | <span data-ttu-id="183f4-114">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="183f4-114">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="183f4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="183f4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="183f4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="183f4-116">Not supported.</span></span>    |
|<span data-ttu-id="183f4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="183f4-117">Application</span></span> | <span data-ttu-id="183f4-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="183f4-118">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="183f4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="183f4-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getByIds
```

## <a name="request-headers"></a><span data-ttu-id="183f4-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="183f4-120">Request headers</span></span>

| <span data-ttu-id="183f4-121">Имя</span><span class="sxs-lookup"><span data-stu-id="183f4-121">Name</span></span>       | <span data-ttu-id="183f4-122">Тип</span><span class="sxs-lookup"><span data-stu-id="183f4-122">Type</span></span> | <span data-ttu-id="183f4-123">Описание</span><span class="sxs-lookup"><span data-stu-id="183f4-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="183f4-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="183f4-124">Authorization</span></span>  | <span data-ttu-id="183f4-125">строка</span><span class="sxs-lookup"><span data-stu-id="183f4-125">string</span></span>  | <span data-ttu-id="183f4-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="183f4-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="183f4-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="183f4-128">Content-Type</span></span>  | <span data-ttu-id="183f4-129">строка</span><span class="sxs-lookup"><span data-stu-id="183f4-129">string</span></span> | <span data-ttu-id="183f4-130">application/json</span><span class="sxs-lookup"><span data-stu-id="183f4-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="183f4-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="183f4-131">Request body</span></span>

<span data-ttu-id="183f4-132">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="183f4-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="183f4-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="183f4-133">Parameter</span></span>   | <span data-ttu-id="183f4-134">Тип</span><span class="sxs-lookup"><span data-stu-id="183f4-134">Type</span></span> |<span data-ttu-id="183f4-135">Описание</span><span class="sxs-lookup"><span data-stu-id="183f4-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="183f4-136">ids</span><span class="sxs-lookup"><span data-stu-id="183f4-136">ids</span></span>|<span data-ttu-id="183f4-137">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="183f4-137">String collection</span></span>| <span data-ttu-id="183f4-p104">Коллекция идентификаторов, для которой необходимо возвратить объекты. Вы можете указать до 1000 идентификаторов.</span><span class="sxs-lookup"><span data-stu-id="183f4-p104">A collection of ids for which to return objects. You can specify up to 1000 ids.</span></span> |
|<span data-ttu-id="183f4-140">types</span><span class="sxs-lookup"><span data-stu-id="183f4-140">types</span></span>|<span data-ttu-id="183f4-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="183f4-141">String collection</span></span>| <span data-ttu-id="183f4-142">Коллекция типов ресурсов, определяющая набор коллекций ресурсов для поиска.</span><span class="sxs-lookup"><span data-stu-id="183f4-142">A collection of resource types that specifies the set of resource collections to search.</span></span> <span data-ttu-id="183f4-143">Если не указана, то коллекция по умолчанию — [directoryObject](../resources/directoryobject.md), которая содержит все типы ресурсов, определенные в справочнике.</span><span class="sxs-lookup"><span data-stu-id="183f4-143">If not specified, the default is [directoryObject](../resources/directoryobject.md), which contains all of the resource types defined in the directory.</span></span> <span data-ttu-id="183f4-144">Любой объект, производный от `directoryObject` может быть указан в коллекции, например, [user (пользователь)](../resources/user.md), [group (группа)](../resources/group.md), [device (устройство)](../resources/device.md)и т. д.</span><span class="sxs-lookup"><span data-stu-id="183f4-144">Any object that derives from `directoryObject` may be specified in the collection; for example: [user](../resources/user.md), [group](../resources/group.md), [device](../resources/device.md), and so on.</span></span> <span data-ttu-id="183f4-145">Для значений не важен регистр символов.</span><span class="sxs-lookup"><span data-stu-id="183f4-145">The values are not case-sensitive.</span></span>|

## <a name="response"></a><span data-ttu-id="183f4-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="183f4-146">Response</span></span>

<span data-ttu-id="183f4-147">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="183f4-147">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="183f4-148">Пример</span><span class="sxs-lookup"><span data-stu-id="183f4-148">Example</span></span>

##### <a name="request"></a><span data-ttu-id="183f4-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="183f4-149">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryobject_getById"
}-->

```http
POST https://graph.microsoft.com/v1.0/directoryObjects/getByIds
Content-type: application/json

{
    "ids":["84b80893874940a3-97b7-68513b600544","5d6059b6368d-45f8-91e18e07d485f1d0"],
    "types":["user"]
}
```

##### <a name="response"></a><span data-ttu-id="183f4-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="183f4-150">Response</span></span>

<span data-ttu-id="183f4-p106">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="183f4-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryObjects",
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
