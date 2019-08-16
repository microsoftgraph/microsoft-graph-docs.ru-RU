---
title: Тип ресурса Унифиедролепермиссион
description: Разрешение роли каталога — это коллекция разрешенных действий и условий для ресурсов.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d15e2709c429be3c6400b59db5174093892d3009
ms.sourcegitcommit: 567d0420243765b4088bc8029306a517f92926fd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/16/2019
ms.locfileid: "36437862"
---
# <a name="unifiedrolepermission-resource-type"></a><span data-ttu-id="67107-103">Тип ресурса Унифиедролепермиссион</span><span class="sxs-lookup"><span data-stu-id="67107-103">unifiedRolePermission resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67107-104">Представляет коллекцию разрешенных действий с ресурсами и условий, которые должны выполняться для вступления в силу действия.</span><span class="sxs-lookup"><span data-stu-id="67107-104">Represents a collection of allowed resource actions and the conditions that must be met for the action to be effective.</span></span> <span data-ttu-id="67107-105">Действия с ресурсами — это задачи, которые могут быть перфомед для ресурса.</span><span class="sxs-lookup"><span data-stu-id="67107-105">Resource actions are tasks that can be perfomed on a resource.</span></span> <span data-ttu-id="67107-106">Например, ресурс Application поддерживает действия с ресурсами "создание", "обновление", "удаление" и "Сброс пароля".</span><span class="sxs-lookup"><span data-stu-id="67107-106">For example, the application resource supports create, update, delete, and reset password resource actions.</span></span>

## <a name="properties"></a><span data-ttu-id="67107-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="67107-107">Properties</span></span>

| <span data-ttu-id="67107-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="67107-108">Property</span></span>     | <span data-ttu-id="67107-109">Тип</span><span class="sxs-lookup"><span data-stu-id="67107-109">Type</span></span>        | <span data-ttu-id="67107-110">Описание</span><span class="sxs-lookup"><span data-stu-id="67107-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="67107-111">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="67107-111">allowedResourceActions</span></span>|<span data-ttu-id="67107-112">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="67107-112">String collection</span></span>| <span data-ttu-id="67107-113">Набор задач, которые могут быть перфомед для ресурса.</span><span class="sxs-lookup"><span data-stu-id="67107-113">Set of tasks that can be perfomed on a resource.</span></span> |
|<span data-ttu-id="67107-114">установлен</span><span class="sxs-lookup"><span data-stu-id="67107-114">condition</span></span>|<span data-ttu-id="67107-115">String</span><span class="sxs-lookup"><span data-stu-id="67107-115">String</span></span>| <span data-ttu-id="67107-116">Необязательные ограничения, которые должны выполняться для эффективного разрешения.</span><span class="sxs-lookup"><span data-stu-id="67107-116">Optional constraints that must be met for the permission to be effective.</span></span> |

### <a name="allowedresourceactions-property"></a><span data-ttu-id="67107-117">Свойство Алловедресаурцеактионс</span><span class="sxs-lookup"><span data-stu-id="67107-117">allowedResourceActions property</span></span>

<span data-ttu-id="67107-118">Ниже приведена схема действий с ресурсами.</span><span class="sxs-lookup"><span data-stu-id="67107-118">The following is the schema for resource actions:</span></span> 

```
<Namespace>/<Entity>/<PropertySet>/<Action>  
```
<span data-ttu-id="67107-119">Пример: `microsoft.directory/applications/credentials/update`.</span><span class="sxs-lookup"><span data-stu-id="67107-119">For example: `microsoft.directory/applications/credentials/update`.</span></span>  

- <span data-ttu-id="67107-120">Namespace — службы, которые предоставляют задачу.</span><span class="sxs-lookup"><span data-stu-id="67107-120">Namespace - The services that exposes the task.</span></span> <span data-ttu-id="67107-121">Например, все задачи в Azure Active Directory используют пространство имен Microsoft. Directory.</span><span class="sxs-lookup"><span data-stu-id="67107-121">For example, all tasks in Azure Active Directory use the namespace microsoft.directory.</span></span>  
- <span data-ttu-id="67107-122">Объект Entity — логические функции или компоненты, предоставляемые службой в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="67107-122">Entity - The logical features or components exposed by the service in Microsoft Graph.</span></span> <span data-ttu-id="67107-123">Например, приложения, субъекты служб или группы.</span><span class="sxs-lookup"><span data-stu-id="67107-123">For example, applications, service principals, or groups.</span></span>
- <span data-ttu-id="67107-124">Набор свойств — конкретные свойства или аспекты объекта, для которого предоставляется доступ.</span><span class="sxs-lookup"><span data-stu-id="67107-124">PropertySet - The specific properties or aspects of the entity for which access is being granted.</span></span> <span data-ttu-id="67107-125">Например, `microsoft.directory/applications/authentication/read` предоставляет возможность чтения URL-адреса ответа, URL-адреса выхода и неявного свойства Flow для объекта **Application** в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="67107-125">For example, `microsoft.directory/applications/authentication/read` grants the ability to read the reply URL, logout URL, and implicit flow property on the **application** object in Azure AD.</span></span> <span data-ttu-id="67107-126">Ниже приведены зарезервированные имена для общих наборов свойств.</span><span class="sxs-lookup"><span data-stu-id="67107-126">The following are reserved names for common property sets:</span></span>  
  - <span data-ttu-id="67107-127">Аллпропертиес — задает все свойства объекта, включая привилегированные свойства.</span><span class="sxs-lookup"><span data-stu-id="67107-127">allProperties - Designates all properties of the entity, including privileged properties.</span></span> <span data-ttu-id="67107-128">Примеры включают `microsoft.directory/applications/allProperties/read` и `microsoft.directory/applications/allProperties/update`.</span><span class="sxs-lookup"><span data-stu-id="67107-128">Examples include `microsoft.directory/applications/allProperties/read` and `microsoft.directory/applications/allProperties/update`.</span></span>
  - <span data-ttu-id="67107-129">Basic — назначает общие свойства чтения, но исключает привилегированных.</span><span class="sxs-lookup"><span data-stu-id="67107-129">basic - Designates common read properties but excludes privileged ones.</span></span> <span data-ttu-id="67107-130">Например, `microsoft.directory/applications/basic/update` позволяет обновлять стандартные свойства, такие как отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="67107-130">For example, `microsoft.directory/applications/basic/update` includes the ability to update standard properties like display name.</span></span>
  - <span data-ttu-id="67107-131">Standard — назначает общие свойства обновления, но исключает привилегированных.</span><span class="sxs-lookup"><span data-stu-id="67107-131">standard - Designates common update properties but excludes privileged ones.</span></span> <span data-ttu-id="67107-132">Например, `microsoft.directory/applications/standard/read`.</span><span class="sxs-lookup"><span data-stu-id="67107-132">For example, `microsoft.directory/applications/standard/read`.</span></span>
- <span data-ttu-id="67107-133">Actions — операции, которые вы предоставляете.</span><span class="sxs-lookup"><span data-stu-id="67107-133">Actions - The operations being granted.</span></span> <span data-ttu-id="67107-134">В большинстве случаев разрешения следует выражать в терминах CRUD или Аллтаскс.</span><span class="sxs-lookup"><span data-stu-id="67107-134">In most circumstances, permissions should be expressed in terms of CRUD or allTasks.</span></span> <span data-ttu-id="67107-135">Сюда входят следующие действия:</span><span class="sxs-lookup"><span data-stu-id="67107-135">Actions include:</span></span>
  - <span data-ttu-id="67107-136">Create — возможность создания нового экземпляра объекта.</span><span class="sxs-lookup"><span data-stu-id="67107-136">Create - The ability to create a new instance of the entity.</span></span>
  - <span data-ttu-id="67107-137">Read — возможность считывания данного набора свойств (включая Аллпропертиес).</span><span class="sxs-lookup"><span data-stu-id="67107-137">Read - The ability to read a given property set (including allProperties).</span></span>
  - <span data-ttu-id="67107-138">Update — возможность обновления набора свойств (включая Аллпропертиес).</span><span class="sxs-lookup"><span data-stu-id="67107-138">Update - The ability to update a given property set (including allProperties).</span></span>
  - <span data-ttu-id="67107-139">Delete — возможность удаления данной сущности.</span><span class="sxs-lookup"><span data-stu-id="67107-139">Delete - The ability to delete a given entity.</span></span>
  - <span data-ttu-id="67107-140">Аллтаскс — представляет все операции CRUD (создание, чтение, обновление и удаление).</span><span class="sxs-lookup"><span data-stu-id="67107-140">AllTasks - Represents all CRUD operations (create, read, update, and delete).</span></span> 

### <a name="condition-property"></a><span data-ttu-id="67107-141">свойство Condition</span><span class="sxs-lookup"><span data-stu-id="67107-141">condition property</span></span>
<span data-ttu-id="67107-142">Условия определяют ограничения, которые должны выполняться.</span><span class="sxs-lookup"><span data-stu-id="67107-142">Conditions define constraints that must be met.</span></span> <span data-ttu-id="67107-143">Например, требование, которое участник является владельцем целевого объекта.</span><span class="sxs-lookup"><span data-stu-id="67107-143">For example, a requirement that the principal be an "owner" of the target.</span></span> <span data-ttu-id="67107-144">Ниже приведены поддерживаемые условия.</span><span class="sxs-lookup"><span data-stu-id="67107-144">The following are the supported conditions:</span></span>

- <span data-ttu-id="67107-145">Само: "@Subject. objectId = = @Resource. objectId"</span><span class="sxs-lookup"><span data-stu-id="67107-145">Self: "@Subject.objectId == @Resource.objectId"</span></span>
- <span data-ttu-id="67107-146">Owner: "@Subject. objectId Any_of @Resource. Owners"</span><span class="sxs-lookup"><span data-stu-id="67107-146">Owner: "@Subject.objectId Any_of @Resource.owners"</span></span>

<span data-ttu-id="67107-147">Ниже приведен пример разрешения роли с условием.</span><span class="sxs-lookup"><span data-stu-id="67107-147">The following is an example of a role permission with a condition.</span></span>

```json
"rolePermissions": [
        {
            "allowedResourceActions": [
                "microsoft.directory/applications/basic/update",
                "microsoft.directory/applications/credentials/update"
            ],
            "condition":  "@Subject.objectId Any_of @Resource.owners"
        }
    ]

```

## <a name="json-representation"></a><span data-ttu-id="67107-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="67107-148">JSON representation</span></span>

<span data-ttu-id="67107-149">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="67107-149">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unifiedRolePermission",
  "baseType": null
}-->

```json
{
  "allowedResourceActions": ["String"],
  "condition": "String"
}
```
## <a name="see-also"></a><span data-ttu-id="67107-150">См. также</span><span class="sxs-lookup"><span data-stu-id="67107-150">See also</span></span>

- <span data-ttu-id="67107-151">[Разрешения роли администратора в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles) — сведения о разрешениях для встроенных ролей каталогов.</span><span class="sxs-lookup"><span data-stu-id="67107-151">[Administrator role permissions in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles) - For information about permissions for built-in directory roles.</span></span>
- <span data-ttu-id="67107-152">[Подтипы регистрации приложений и разрешения в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/roles-custom-available-permissions) — сведения о разрешениях, доступных для пользовательских ролей каталога.</span><span class="sxs-lookup"><span data-stu-id="67107-152">[Application registration subtypes and permissions in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/roles-custom-available-permissions) -  For information about permissions that are available for custom directory roles.</span></span> 

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unifiedRolePermission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
