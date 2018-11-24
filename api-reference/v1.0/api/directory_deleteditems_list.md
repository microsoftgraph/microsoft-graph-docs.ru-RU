# <a name="list-deleted-items"></a><span data-ttu-id="7d225-101">Перечисление удаленных элементов</span><span class="sxs-lookup"><span data-stu-id="7d225-101">List deleted items</span></span>

<span data-ttu-id="7d225-102">Получение списка недавно [удаленных элементов](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="7d225-102">Retrieve a list of recently deleted items from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="7d225-103">В настоящее время хранение удаленных элементов поддерживается только для ресурсов [group](../resources/group.md) и [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="7d225-103">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="7d225-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7d225-104">Permissions</span></span>
<span data-ttu-id="7d225-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7d225-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

### <a name="for-users"></a><span data-ttu-id="7d225-107">Для пользователей:</span><span class="sxs-lookup"><span data-stu-id="7d225-107">For users:</span></span>

|<span data-ttu-id="7d225-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7d225-108">Permission type</span></span>      | <span data-ttu-id="7d225-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7d225-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d225-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7d225-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7d225-111">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7d225-111">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="7d225-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7d225-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d225-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d225-113">Not supported.</span></span> |
|<span data-ttu-id="7d225-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7d225-114">Application</span></span> | <span data-ttu-id="7d225-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d225-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="7d225-116">Для групп:</span><span class="sxs-lookup"><span data-stu-id="7d225-116">For groups:</span></span>

|<span data-ttu-id="7d225-117">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7d225-117">Permission type</span></span>      | <span data-ttu-id="7d225-118">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7d225-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d225-119">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7d225-119">Delegated (work or school account)</span></span> | <span data-ttu-id="7d225-120">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7d225-120">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="7d225-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7d225-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d225-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d225-122">Not supported.</span></span>    |
|<span data-ttu-id="7d225-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7d225-123">Application</span></span> | <span data-ttu-id="7d225-124">Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="7d225-124">Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d225-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7d225-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http 
GET /directory/deletedItems/microsoft.graph.group
GET /directory/deletedItems/microsoft.graph.user
```

<span data-ttu-id="7d225-126">В настоящее время этот API поддерживает получение групп (microsoft.graph.group) и пользователей (microsoft.graph.user) из удаленных элементов.</span><span class="sxs-lookup"><span data-stu-id="7d225-126">This API currently supports retrieving object types of groups (microsoft.graph.group) or users (microsoft.graph.user) from deleted items.</span></span> <span data-ttu-id="7d225-127">Тип является обязательной частью URI.</span><span class="sxs-lookup"><span data-stu-id="7d225-127">The type is specified as a required part of the URI.</span></span> <span data-ttu-id="7d225-128">Вызов GET/каталог/deletedItems без типа не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d225-128">Calling GET /directory/deletedItems without a type is not supported.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="7d225-129">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7d225-129">Optional query parameters</span></span>
<span data-ttu-id="7d225-130">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="7d225-130">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7d225-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7d225-131">Request headers</span></span>
| <span data-ttu-id="7d225-132">Имя</span><span class="sxs-lookup"><span data-stu-id="7d225-132">Name</span></span>      |<span data-ttu-id="7d225-133">Описание</span><span class="sxs-lookup"><span data-stu-id="7d225-133">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7d225-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d225-134">Authorization</span></span>  | <span data-ttu-id="7d225-135">Bearer &lt;code&gt; *Обязательный*.</span><span class="sxs-lookup"><span data-stu-id="7d225-135">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="7d225-136">Accept</span><span class="sxs-lookup"><span data-stu-id="7d225-136">Accept</span></span>  | <span data-ttu-id="7d225-137">application/json</span><span class="sxs-lookup"><span data-stu-id="7d225-137">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="7d225-138">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7d225-138">Request body</span></span>
<span data-ttu-id="7d225-139">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7d225-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7d225-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d225-140">Response</span></span>

<span data-ttu-id="7d225-141">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7d225-141">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7d225-142">Пример</span><span class="sxs-lookup"><span data-stu-id="7d225-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7d225-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="7d225-143">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_deleteditems"
}-->
```http
GET https://graph.microsoft.com/v1.0/directory/deletedItems/microsoft.graph.group
```
##### <a name="response"></a><span data-ttu-id="7d225-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d225-144">Response</span></span>
<span data-ttu-id="7d225-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7d225-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "value": [
    {
      "id":"46cc6179-19d0-473e-97ad-6ff84347bbbb",
      "displayName":"SampleGroup",
      "groupTypes":["Unified"],
      "mail":"example@contoso.com",
      "mailEnabled":true,
      "mailNickname":"Example",
      "securityEnabled":false,
      "visibility":"Public"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List deleteditems",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->