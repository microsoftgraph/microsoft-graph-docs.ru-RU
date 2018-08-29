# <a name="restore-deleted-item"></a><span data-ttu-id="81c78-101">Восстановление удаленного элемента</span><span class="sxs-lookup"><span data-stu-id="81c78-101">Restore deleted item</span></span>

<span data-ttu-id="81c78-102">Восстановление недавно удаленного элемента из контейнера для [удаленных элементов](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="81c78-102">Restores a recently deleted item from [deleted items](../resources/directory.md).</span></span> 

<span data-ttu-id="81c78-103">В настоящее время хранение удаленных элементов поддерживается только для ресурсов [group](../resources/group.md) и [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="81c78-103">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="81c78-104">Вы можете полностью восстановить случайно удаленный элемент.</span><span class="sxs-lookup"><span data-stu-id="81c78-104">If an item was accidentally deleted, you can fully restore the item.</span></span>

<span data-ttu-id="81c78-105">Удаленный элемент можно восстановить в течение 30 дней.</span><span class="sxs-lookup"><span data-stu-id="81c78-105">A recently deleted item will remain available for up to 30 days.</span></span> <span data-ttu-id="81c78-106">Через 30 дней элемент удаляется без возможности восстановления.</span><span class="sxs-lookup"><span data-stu-id="81c78-106">After 30 days, the item is permanently deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="81c78-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="81c78-107">Permissions</span></span>
<span data-ttu-id="81c78-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="81c78-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

### <a name="for-users"></a><span data-ttu-id="81c78-110">Для пользователей:</span><span class="sxs-lookup"><span data-stu-id="81c78-110">For users:</span></span>

|<span data-ttu-id="81c78-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="81c78-111">Permission type</span></span>      | <span data-ttu-id="81c78-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="81c78-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="81c78-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="81c78-113">Delegated (work or school account)</span></span> | <span data-ttu-id="81c78-114">User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="81c78-114">User.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="81c78-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="81c78-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81c78-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81c78-116">Not supported.</span></span> |
|<span data-ttu-id="81c78-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="81c78-117">Application</span></span> | <span data-ttu-id="81c78-118">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81c78-118">User.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="81c78-119">Для групп:</span><span class="sxs-lookup"><span data-stu-id="81c78-119">For groups:</span></span>

|<span data-ttu-id="81c78-120">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="81c78-120">Permission type</span></span>      | <span data-ttu-id="81c78-121">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="81c78-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="81c78-122">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="81c78-122">Delegated (work or school account)</span></span> | <span data-ttu-id="81c78-123">Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="81c78-123">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="81c78-124">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="81c78-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81c78-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81c78-125">Not supported.</span></span>    |
|<span data-ttu-id="81c78-126">Для приложений</span><span class="sxs-lookup"><span data-stu-id="81c78-126">Application</span></span> | <span data-ttu-id="81c78-127">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81c78-127">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="81c78-128">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="81c78-128">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directory/deletedItems/{id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="81c78-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="81c78-129">Request headers</span></span>
| <span data-ttu-id="81c78-130">Имя</span><span class="sxs-lookup"><span data-stu-id="81c78-130">Name</span></span>       | <span data-ttu-id="81c78-131">Описание</span><span class="sxs-lookup"><span data-stu-id="81c78-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="81c78-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="81c78-132">Authorization</span></span>  | <span data-ttu-id="81c78-133">Bearer &lt;code&gt; *Обязательный*.</span><span class="sxs-lookup"><span data-stu-id="81c78-133">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="81c78-134">Accept</span><span class="sxs-lookup"><span data-stu-id="81c78-134">Accept</span></span> | <span data-ttu-id="81c78-135">application/json</span><span class="sxs-lookup"><span data-stu-id="81c78-135">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="81c78-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="81c78-136">Request body</span></span>
<span data-ttu-id="81c78-137">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="81c78-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81c78-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="81c78-138">Response</span></span>

<span data-ttu-id="81c78-139">В случае успеха этот метод возвращает код отклика `200 OK` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="81c78-139">If successful, this method returns `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81c78-140">Пример</span><span class="sxs-lookup"><span data-stu-id="81c78-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="81c78-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="81c78-141">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directory"
}-->
```http
POST https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}/restore
```
<span data-ttu-id="81c78-142">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="81c78-142">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="81c78-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="81c78-143">Response</span></span>
<span data-ttu-id="81c78-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="81c78-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#directoryObjects/$entity",
  "@odata.type":"#microsoft.graph.group",
  "id":"46cc6179-19d0-473e-97ad-6ff84347bbbb",
  "displayName":"SampleGroup",
  "groupTypes":["Unified"],
  "mail":"example@contoso.com",
  "mailEnabled":true,
  "mailNickname":"Example",
  "securityEnabled":false,
  "visibility":"Public"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create deletedItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->