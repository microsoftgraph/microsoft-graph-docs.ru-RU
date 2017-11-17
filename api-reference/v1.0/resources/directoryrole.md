# <a name="directoryrole-resource-type"></a><span data-ttu-id="1628c-101">Тип ресурса directoryRole</span><span class="sxs-lookup"><span data-stu-id="1628c-101">directoryRole resource type</span></span>

<span data-ttu-id="1628c-p101">Представляет роль каталога Azure AD. Роли каталога Azure AD также известны как *роли администратора*. Для получения дополнительных сведений о ролях каталога (администратора) см. статью [Назначение ролей администратора в Azure AD](http://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/). С помощью Microsoft Graph можно назначать пользователям роли каталога, чтобы предоставить им разрешения целевой роли. Чтобы можно было считать роль каталога или обновить ее членов, сначала следует активировать ее на клиенте. По умолчанию активируется только роль каталога администраторов организации. Чтобы активировать остальные доступные роли каталога, следует отправить запрос POST с идентификатором ресурса [directoryRoleTemplate](directoryroletemplate.md), определяющего значения свойств для роли каталога. Наследуется из [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="1628c-p101">Represents an Azure AD directory role. Azure AD directory roles are also known as *administrator roles*. For more information about directory (administrator) roles, see [Assigning administrator roles in Azure AD](http://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/). With the Microsoft Graph, you can assign users to directory roles to grant them the permissions of the target role. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators directory role is activated by default. To activate other available directory roles you send a POST request with the ID of the [directoryRoleTemplate](directoryroletemplate.md) on which the directory role is based. Inherits from [directoryObject](directoryobject.md).</span></span>

## <a name="methods"></a><span data-ttu-id="1628c-110">Методы</span><span class="sxs-lookup"><span data-stu-id="1628c-110">Methods</span></span>

| <span data-ttu-id="1628c-111">Метод</span><span class="sxs-lookup"><span data-stu-id="1628c-111">Method</span></span>       | <span data-ttu-id="1628c-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1628c-112">Return Type</span></span>  |<span data-ttu-id="1628c-113">Описание</span><span class="sxs-lookup"><span data-stu-id="1628c-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1628c-114">Получение directoryRole</span><span class="sxs-lookup"><span data-stu-id="1628c-114">Get directoryRole</span></span>](../api/directoryrole_get.md) | [<span data-ttu-id="1628c-115">directoryRole</span><span class="sxs-lookup"><span data-stu-id="1628c-115">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="1628c-116">Считывание свойств и отношений объекта directoryRole.</span><span class="sxs-lookup"><span data-stu-id="1628c-116">Read properties and relationships of directoryRole object.</span></span> |
|[<span data-ttu-id="1628c-117">Перечисление объектов directoryRole</span><span class="sxs-lookup"><span data-stu-id="1628c-117">List directoryRoles</span></span>](../api/directoryrole_list.md) | <span data-ttu-id="1628c-118">Коллекция объектов [directoryRole](directoryrole.md)</span><span class="sxs-lookup"><span data-stu-id="1628c-118">[directoryRole](directoryrole.md) collection</span></span> | <span data-ttu-id="1628c-119">Перечисление ролей каталога, активированных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="1628c-119">List the directory roles that are activated in the tenant.</span></span> |
|[<span data-ttu-id="1628c-120">Добавление элемента</span><span class="sxs-lookup"><span data-stu-id="1628c-120">Add member</span></span>](../api/directoryrole_post_members.md) |[<span data-ttu-id="1628c-121">directoryObject</span><span class="sxs-lookup"><span data-stu-id="1628c-121">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="1628c-122">Добавление пользователя в роль каталога путем записи данных в свойство навигации members.</span><span class="sxs-lookup"><span data-stu-id="1628c-122">Add a user to the directory role by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="1628c-123">Список членов</span><span class="sxs-lookup"><span data-stu-id="1628c-123">List members</span></span>](../api/directoryrole_list_members.md) |<span data-ttu-id="1628c-124">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="1628c-124">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="1628c-125">Получение пользователей, которые относятся к членам роли каталога, из свойства навигации members.</span><span class="sxs-lookup"><span data-stu-id="1628c-125">Get the users that are members of the directory role from the members navigation property.</span></span>|
|[<span data-ttu-id="1628c-126">Удаление члена</span><span class="sxs-lookup"><span data-stu-id="1628c-126">Remove a member</span></span>](../api/directoryrole_delete_member.md) |[<span data-ttu-id="1628c-127">directoryObject</span><span class="sxs-lookup"><span data-stu-id="1628c-127">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="1628c-128">Удаление ресурса user из роли каталога.</span><span class="sxs-lookup"><span data-stu-id="1628c-128">Remove a user from the directory role.</span></span>|
|[<span data-ttu-id="1628c-129">Активация directoryRole</span><span class="sxs-lookup"><span data-stu-id="1628c-129">Activate directoryRole</span></span>](../api/directoryrole_post_directoryroles.md) |[<span data-ttu-id="1628c-130">directoryRole</span><span class="sxs-lookup"><span data-stu-id="1628c-130">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="1628c-131">Активация роли каталога.</span><span class="sxs-lookup"><span data-stu-id="1628c-131">Activate a directory role.</span></span>|

## <a name="properties"></a><span data-ttu-id="1628c-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="1628c-132">Properties</span></span>
| <span data-ttu-id="1628c-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="1628c-133">Property</span></span>   | <span data-ttu-id="1628c-134">Тип</span><span class="sxs-lookup"><span data-stu-id="1628c-134">Type</span></span> | <span data-ttu-id="1628c-135">Описание</span><span class="sxs-lookup"><span data-stu-id="1628c-135">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="1628c-136">description</span><span class="sxs-lookup"><span data-stu-id="1628c-136">description</span></span>|<span data-ttu-id="1628c-137">String</span><span class="sxs-lookup"><span data-stu-id="1628c-137">String</span></span>|<span data-ttu-id="1628c-p102">Описание роли каталога. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1628c-p102">The description for the directory role. Read-only.</span></span> |
|<span data-ttu-id="1628c-140">displayName</span><span class="sxs-lookup"><span data-stu-id="1628c-140">displayName</span></span>|<span data-ttu-id="1628c-141">Строка</span><span class="sxs-lookup"><span data-stu-id="1628c-141">String</span></span>|<span data-ttu-id="1628c-p103">Отображаемое имя роли каталога. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1628c-p103">The display name for the directory role. Read-only.</span></span> |
|<span data-ttu-id="1628c-144">id</span><span class="sxs-lookup"><span data-stu-id="1628c-144">id</span></span>|<span data-ttu-id="1628c-145">String</span><span class="sxs-lookup"><span data-stu-id="1628c-145">String</span></span>|<span data-ttu-id="1628c-p104">Уникальный идентификатор роли каталога. Наследуется из [directoryObject](directoryobject.md). Ключ, значение null не допускается, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1628c-p104">The unique identifier for the directory role. Inherited from [directoryObject](directoryobject.md). Key, Not nullable, Read-only.</span></span>|
|<span data-ttu-id="1628c-149">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="1628c-149">roleTemplateId</span></span>|<span data-ttu-id="1628c-150">String</span><span class="sxs-lookup"><span data-stu-id="1628c-150">String</span></span>| <span data-ttu-id="1628c-p105">Свойство **id** ресурса [directoryRoleTemplate](directoryroletemplate.md), определяющего значения свойств для этой роли. При активации роли каталога на клиенте следует указать свойство с помощью операции POST. После активации роли каталога свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1628c-p105">The **id** of the [directoryRoleTemplate](directoryroletemplate.md) that this role is based on. The property must be specified when activating a directory role in a tenant with a POST operation. After the directory role has been activated, the property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="1628c-154">Связи</span><span class="sxs-lookup"><span data-stu-id="1628c-154">Relationships</span></span>
| <span data-ttu-id="1628c-155">Связь</span><span class="sxs-lookup"><span data-stu-id="1628c-155">Relationship</span></span> | <span data-ttu-id="1628c-156">Тип</span><span class="sxs-lookup"><span data-stu-id="1628c-156">Type</span></span> |<span data-ttu-id="1628c-157">Описание</span><span class="sxs-lookup"><span data-stu-id="1628c-157">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1628c-158">members</span><span class="sxs-lookup"><span data-stu-id="1628c-158">members</span></span>|<span data-ttu-id="1628c-159">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="1628c-159">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="1628c-p106">Пользователи, которые относятся к членам этой роли каталога. Методы HTTP: GET, POST, DELETE. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="1628c-p106">Users that are members of this directory role. HTTP Methods: GET, POST, DELETE. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1628c-164">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="1628c-164">JSON representation</span></span>

<span data-ttu-id="1628c-165">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1628c-165">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "memberOf",
    "members",
    "ownedObjects",
    "owners"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryRole"
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
