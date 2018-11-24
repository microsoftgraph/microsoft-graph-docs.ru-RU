# <a name="directoryrole-resource-type"></a><span data-ttu-id="25568-101">Тип ресурса directoryRole</span><span class="sxs-lookup"><span data-stu-id="25568-101">directoryRole resource type</span></span>

<span data-ttu-id="25568-102">Представляет роль directory Azure AD.</span><span class="sxs-lookup"><span data-stu-id="25568-102">Represents an Azure AD directory role.</span></span> <span data-ttu-id="25568-103">Каталог роли Azure AD также называются *ролями администратора*.</span><span class="sxs-lookup"><span data-stu-id="25568-103">Azure AD directory roles are also known as *administrator roles*.</span></span> <span data-ttu-id="25568-104">Дополнительные сведения о ролях каталогов (администратор) можно [Назначение ролей администратора в Azure AD](http://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/).</span><span class="sxs-lookup"><span data-stu-id="25568-104">For more information about directory (administrator) roles, see [Assigning administrator roles in Azure AD](http://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/).</span></span> <span data-ttu-id="25568-105">Microsoft Graph можно назначить роли каталог, чтобы предоставлять им разрешения целевой роли пользователей.</span><span class="sxs-lookup"><span data-stu-id="25568-105">With the Microsoft Graph, you can assign users to directory roles to grant them the permissions of the target role.</span></span> <span data-ttu-id="25568-106">Для чтения роли каталога или обновите его члены, необходимо активировать в клиентов.</span><span class="sxs-lookup"><span data-stu-id="25568-106">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="25568-107">Только роль directory Администраторы организации активируется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="25568-107">Only the Company Administrators directory role is activated by default.</span></span> <span data-ttu-id="25568-108">Активация других ролей доступны directory отправить запрос POST с Идентификатором [directoryRoleTemplate](directoryroletemplate.md) , лежащие в основе роли каталога.</span><span class="sxs-lookup"><span data-stu-id="25568-108">To activate other available directory roles you send a POST request with the ID of the [directoryRoleTemplate](directoryroletemplate.md) on which the directory role is based.</span></span> <span data-ttu-id="25568-109">Наследуется от [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="25568-109">Inherits from [directoryObject](directoryobject.md).</span></span>
<span data-ttu-id="25568-110">Этот ресурс поддерживает:</span><span class="sxs-lookup"><span data-stu-id="25568-110">This resource supports:</span></span>

- <span data-ttu-id="25568-111">отслеживание дополнений, удалений и обновлений с помощью [запроса изменений](../../../concepts/delta_query_overview.md) (функция [delta](../api/directoryrole_delta.md)).</span><span class="sxs-lookup"><span data-stu-id="25568-111">Using [delta query](../../../concepts/delta_query_overview.md) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryrole_delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="25568-112">Методы</span><span class="sxs-lookup"><span data-stu-id="25568-112">Methods</span></span>

| <span data-ttu-id="25568-113">Метод</span><span class="sxs-lookup"><span data-stu-id="25568-113">Method</span></span>       | <span data-ttu-id="25568-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="25568-114">Return Type</span></span>  |<span data-ttu-id="25568-115">Описание</span><span class="sxs-lookup"><span data-stu-id="25568-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="25568-116">Получение directoryRole</span><span class="sxs-lookup"><span data-stu-id="25568-116">Get directoryRole</span></span>](../api/directoryrole_get.md) | [<span data-ttu-id="25568-117">directoryRole</span><span class="sxs-lookup"><span data-stu-id="25568-117">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="25568-118">Считывание свойств и отношений объекта directoryRole.</span><span class="sxs-lookup"><span data-stu-id="25568-118">Read properties and relationships of directoryRole object.</span></span> |
|[<span data-ttu-id="25568-119">Перечисление объектов directoryRole</span><span class="sxs-lookup"><span data-stu-id="25568-119">List directoryRoles</span></span>](../api/directoryrole_list.md) | <span data-ttu-id="25568-120">Коллекция объектов [directoryRole](directoryrole.md)</span><span class="sxs-lookup"><span data-stu-id="25568-120">[directoryRole](directoryrole.md) collection</span></span> | <span data-ttu-id="25568-121">Перечисление ролей каталога, активированных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="25568-121">List the directory roles that are activated in the tenant.</span></span> |
|[<span data-ttu-id="25568-122">Добавление элемента</span><span class="sxs-lookup"><span data-stu-id="25568-122">Add member</span></span>](../api/directoryrole_post_members.md) |[<span data-ttu-id="25568-123">directoryObject</span><span class="sxs-lookup"><span data-stu-id="25568-123">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="25568-124">Добавление пользователя в роль каталога путем записи данных в свойство навигации members.</span><span class="sxs-lookup"><span data-stu-id="25568-124">Add a user to the directory role by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="25568-125">Список членов</span><span class="sxs-lookup"><span data-stu-id="25568-125">List members</span></span>](../api/directoryrole_list_members.md) |<span data-ttu-id="25568-126">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="25568-126">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="25568-127">Получение пользователей, которые относятся к членам роли каталога, из свойства навигации members.</span><span class="sxs-lookup"><span data-stu-id="25568-127">Get the users that are members of the directory role from the members navigation property.</span></span>|
|[<span data-ttu-id="25568-128">Удаление члена</span><span class="sxs-lookup"><span data-stu-id="25568-128">Remove a member</span></span>](../api/directoryrole_delete_member.md) |[<span data-ttu-id="25568-129">directoryObject</span><span class="sxs-lookup"><span data-stu-id="25568-129">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="25568-130">Удаление ресурса user из роли каталога.</span><span class="sxs-lookup"><span data-stu-id="25568-130">Remove a user from the directory role.</span></span>|
|[<span data-ttu-id="25568-131">Активация directoryRole</span><span class="sxs-lookup"><span data-stu-id="25568-131">Activate directoryRole</span></span>](../api/directoryrole_post_directoryroles.md) |[<span data-ttu-id="25568-132">directoryRole</span><span class="sxs-lookup"><span data-stu-id="25568-132">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="25568-133">Активация роли каталога.</span><span class="sxs-lookup"><span data-stu-id="25568-133">Activate a directory role.</span></span>|
|[<span data-ttu-id="25568-134">delta</span><span class="sxs-lookup"><span data-stu-id="25568-134">delta</span></span>](../api/directoryrole_delta.md)|<span data-ttu-id="25568-135">Коллекция объектов directoryRole</span><span class="sxs-lookup"><span data-stu-id="25568-135">directoryRole collection</span></span>| <span data-ttu-id="25568-136">Получите добавочные изменения для каталога ролей.</span><span class="sxs-lookup"><span data-stu-id="25568-136">Get incremental changes for directory roles.</span></span> |

## <a name="properties"></a><span data-ttu-id="25568-137">Свойства</span><span class="sxs-lookup"><span data-stu-id="25568-137">Properties</span></span>
| <span data-ttu-id="25568-138">Свойство</span><span class="sxs-lookup"><span data-stu-id="25568-138">Property</span></span>   | <span data-ttu-id="25568-139">Тип</span><span class="sxs-lookup"><span data-stu-id="25568-139">Type</span></span> | <span data-ttu-id="25568-140">Описание</span><span class="sxs-lookup"><span data-stu-id="25568-140">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="25568-141">описание</span><span class="sxs-lookup"><span data-stu-id="25568-141">description</span></span>|<span data-ttu-id="25568-142">String</span><span class="sxs-lookup"><span data-stu-id="25568-142">String</span></span>|<span data-ttu-id="25568-p102">Описание роли каталога. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25568-p102">The description for the directory role. Read-only.</span></span> |
|<span data-ttu-id="25568-145">displayName</span><span class="sxs-lookup"><span data-stu-id="25568-145">displayName</span></span>|<span data-ttu-id="25568-146">String</span><span class="sxs-lookup"><span data-stu-id="25568-146">String</span></span>|<span data-ttu-id="25568-p103">Отображаемое имя роли каталога. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25568-p103">The display name for the directory role. Read-only.</span></span> |
|<span data-ttu-id="25568-149">id</span><span class="sxs-lookup"><span data-stu-id="25568-149">id</span></span>|<span data-ttu-id="25568-150">String</span><span class="sxs-lookup"><span data-stu-id="25568-150">String</span></span>|<span data-ttu-id="25568-p104">Уникальный идентификатор роли каталога. Наследуется из [directoryObject](directoryobject.md). Ключ, значение null не допускается, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25568-p104">The unique identifier for the directory role. Inherited from [directoryObject](directoryobject.md). Key, Not nullable, Read-only.</span></span>|
|<span data-ttu-id="25568-154">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="25568-154">roleTemplateId</span></span>|<span data-ttu-id="25568-155">String</span><span class="sxs-lookup"><span data-stu-id="25568-155">String</span></span>| <span data-ttu-id="25568-p105">Свойство **id** ресурса [directoryRoleTemplate](directoryroletemplate.md), определяющего значения свойств для этой роли. При активации роли каталога на клиенте следует указать свойство с помощью операции POST. После активации роли каталога свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25568-p105">The **id** of the [directoryRoleTemplate](directoryroletemplate.md) that this role is based on. The property must be specified when activating a directory role in a tenant with a POST operation. After the directory role has been activated, the property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="25568-159">Связи</span><span class="sxs-lookup"><span data-stu-id="25568-159">Relationships</span></span>
| <span data-ttu-id="25568-160">Связь</span><span class="sxs-lookup"><span data-stu-id="25568-160">Relationship</span></span> | <span data-ttu-id="25568-161">Тип</span><span class="sxs-lookup"><span data-stu-id="25568-161">Type</span></span> |<span data-ttu-id="25568-162">Описание</span><span class="sxs-lookup"><span data-stu-id="25568-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="25568-163">members</span><span class="sxs-lookup"><span data-stu-id="25568-163">members</span></span>|<span data-ttu-id="25568-164">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="25568-164">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="25568-p106">Пользователи, которые относятся к членам этой роли каталога. Методы HTTP: GET, POST, DELETE. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="25568-p106">Users that are members of this directory role. HTTP Methods: GET, POST, DELETE. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="25568-169">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="25568-169">JSON representation</span></span>

<span data-ttu-id="25568-170">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="25568-170">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [
    "memberOf",
    "members",
    "ownedObjects",
    "owners"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.directoryRole",
  "@odata.annotations": [
    {
      "capabilities": {
        "toppable": false
      }
    }
  ]
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
  "roleTemplateId": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
