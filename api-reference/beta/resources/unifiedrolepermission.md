---
title: Тип ресурса Унифиедролепермиссион
description: Разрешение роли каталога — это коллекция разрешенных действий и условий для ресурсов.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f456927289a285a81eb088dd622b79f120df188f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43401667"
---
# <a name="unifiedrolepermission-resource-type"></a><span data-ttu-id="68679-103">Тип ресурса Унифиедролепермиссион</span><span class="sxs-lookup"><span data-stu-id="68679-103">unifiedRolePermission resource type</span></span>

<span data-ttu-id="68679-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68679-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68679-105">Представляет коллекцию разрешенных действий с ресурсами и условий, которые должны выполняться для вступления в силу действия.</span><span class="sxs-lookup"><span data-stu-id="68679-105">Represents a collection of allowed resource actions and the conditions that must be met for the action to be effective.</span></span> <span data-ttu-id="68679-106">Действия с ресурсами — это задачи, которые могут быть перфомед для ресурса.</span><span class="sxs-lookup"><span data-stu-id="68679-106">Resource actions are tasks that can be perfomed on a resource.</span></span> <span data-ttu-id="68679-107">Например, ресурс Application поддерживает действия с ресурсами "создание", "обновление", "удаление" и "Сброс пароля".</span><span class="sxs-lookup"><span data-stu-id="68679-107">For example, the application resource supports create, update, delete, and reset password resource actions.</span></span>

## <a name="properties"></a><span data-ttu-id="68679-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="68679-108">Properties</span></span>

| <span data-ttu-id="68679-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="68679-109">Property</span></span>     | <span data-ttu-id="68679-110">Тип</span><span class="sxs-lookup"><span data-stu-id="68679-110">Type</span></span>        | <span data-ttu-id="68679-111">Описание</span><span class="sxs-lookup"><span data-stu-id="68679-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="68679-112">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="68679-112">allowedResourceActions</span></span>|<span data-ttu-id="68679-113">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="68679-113">String collection</span></span>| <span data-ttu-id="68679-114">Набор задач, которые могут быть перфомед для ресурса.</span><span class="sxs-lookup"><span data-stu-id="68679-114">Set of tasks that can be perfomed on a resource.</span></span> |
|<span data-ttu-id="68679-115">установлен</span><span class="sxs-lookup"><span data-stu-id="68679-115">condition</span></span>|<span data-ttu-id="68679-116">String</span><span class="sxs-lookup"><span data-stu-id="68679-116">String</span></span>| <span data-ttu-id="68679-117">Необязательные ограничения, которые должны выполняться для эффективного разрешения.</span><span class="sxs-lookup"><span data-stu-id="68679-117">Optional constraints that must be met for the permission to be effective.</span></span> |

### <a name="allowedresourceactions-property"></a><span data-ttu-id="68679-118">Свойство Алловедресаурцеактионс</span><span class="sxs-lookup"><span data-stu-id="68679-118">allowedResourceActions property</span></span>

<span data-ttu-id="68679-119">Ниже приведена схема действий с ресурсами.</span><span class="sxs-lookup"><span data-stu-id="68679-119">The following is the schema for resource actions:</span></span> 

```
<Namespace>/<Entity>/<PropertySet>/<Action>  
```
<span data-ttu-id="68679-120">Пример: `microsoft.directory/applications/credentials/update`.</span><span class="sxs-lookup"><span data-stu-id="68679-120">For example: `microsoft.directory/applications/credentials/update`.</span></span>  

- <span data-ttu-id="68679-121">Namespace — службы, которые предоставляют задачу.</span><span class="sxs-lookup"><span data-stu-id="68679-121">Namespace - The services that exposes the task.</span></span> <span data-ttu-id="68679-122">Например, все задачи в Azure Active Directory используют пространство имен Microsoft. Directory.</span><span class="sxs-lookup"><span data-stu-id="68679-122">For example, all tasks in Azure Active Directory use the namespace microsoft.directory.</span></span>  
- <span data-ttu-id="68679-123">Объект Entity — логические функции или компоненты, предоставляемые службой в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="68679-123">Entity - The logical features or components exposed by the service in Microsoft Graph.</span></span> <span data-ttu-id="68679-124">Например, приложения, субъекты служб или группы.</span><span class="sxs-lookup"><span data-stu-id="68679-124">For example, applications, service principals, or groups.</span></span>
- <span data-ttu-id="68679-125">Набор свойств — конкретные свойства или аспекты объекта, для которого предоставляется доступ.</span><span class="sxs-lookup"><span data-stu-id="68679-125">PropertySet - The specific properties or aspects of the entity for which access is being granted.</span></span> <span data-ttu-id="68679-126">Например, `microsoft.directory/applications/authentication/read` предоставляет возможность чтения URL-адреса ответа, URL-адреса выхода и неявного свойства Flow для объекта **Application** в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="68679-126">For example, `microsoft.directory/applications/authentication/read` grants the ability to read the reply URL, logout URL, and implicit flow property on the **application** object in Azure AD.</span></span> <span data-ttu-id="68679-127">Ниже приведены зарезервированные имена для общих наборов свойств.</span><span class="sxs-lookup"><span data-stu-id="68679-127">The following are reserved names for common property sets:</span></span>  
  - <span data-ttu-id="68679-128">Аллпропертиес — задает все свойства объекта, включая привилегированные свойства.</span><span class="sxs-lookup"><span data-stu-id="68679-128">allProperties - Designates all properties of the entity, including privileged properties.</span></span> <span data-ttu-id="68679-129">Примеры включают `microsoft.directory/applications/allProperties/read` и `microsoft.directory/applications/allProperties/update`.</span><span class="sxs-lookup"><span data-stu-id="68679-129">Examples include `microsoft.directory/applications/allProperties/read` and `microsoft.directory/applications/allProperties/update`.</span></span>
  - <span data-ttu-id="68679-130">Basic — назначает общие свойства чтения, но исключает привилегированных.</span><span class="sxs-lookup"><span data-stu-id="68679-130">basic - Designates common read properties but excludes privileged ones.</span></span> <span data-ttu-id="68679-131">Например, `microsoft.directory/applications/basic/update` позволяет обновлять стандартные свойства, такие как отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="68679-131">For example, `microsoft.directory/applications/basic/update` includes the ability to update standard properties like display name.</span></span>
  - <span data-ttu-id="68679-132">Standard — назначает общие свойства обновления, но исключает привилегированных.</span><span class="sxs-lookup"><span data-stu-id="68679-132">standard - Designates common update properties but excludes privileged ones.</span></span> <span data-ttu-id="68679-133">Например, `microsoft.directory/applications/standard/read`.</span><span class="sxs-lookup"><span data-stu-id="68679-133">For example, `microsoft.directory/applications/standard/read`.</span></span>
- <span data-ttu-id="68679-134">Actions — операции, которые вы предоставляете.</span><span class="sxs-lookup"><span data-stu-id="68679-134">Actions - The operations being granted.</span></span> <span data-ttu-id="68679-135">В большинстве случаев разрешения следует выражать в терминах CRUD или Аллтаскс.</span><span class="sxs-lookup"><span data-stu-id="68679-135">In most circumstances, permissions should be expressed in terms of CRUD or allTasks.</span></span> <span data-ttu-id="68679-136">Сюда входят следующие действия:</span><span class="sxs-lookup"><span data-stu-id="68679-136">Actions include:</span></span>
  - <span data-ttu-id="68679-137">Create — возможность создания нового экземпляра объекта.</span><span class="sxs-lookup"><span data-stu-id="68679-137">Create - The ability to create a new instance of the entity.</span></span>
  - <span data-ttu-id="68679-138">Read — возможность считывания данного набора свойств (включая Аллпропертиес).</span><span class="sxs-lookup"><span data-stu-id="68679-138">Read - The ability to read a given property set (including allProperties).</span></span>
  - <span data-ttu-id="68679-139">Update — возможность обновления набора свойств (включая Аллпропертиес).</span><span class="sxs-lookup"><span data-stu-id="68679-139">Update - The ability to update a given property set (including allProperties).</span></span>
  - <span data-ttu-id="68679-140">Delete — возможность удаления данной сущности.</span><span class="sxs-lookup"><span data-stu-id="68679-140">Delete - The ability to delete a given entity.</span></span>
  - <span data-ttu-id="68679-141">Аллтаскс — представляет все операции CRUD (создание, чтение, обновление и удаление).</span><span class="sxs-lookup"><span data-stu-id="68679-141">AllTasks - Represents all CRUD operations (create, read, update, and delete).</span></span> 

### <a name="condition-property"></a><span data-ttu-id="68679-142">свойство Condition</span><span class="sxs-lookup"><span data-stu-id="68679-142">condition property</span></span>
<span data-ttu-id="68679-143">Условия определяют ограничения, которые должны выполняться.</span><span class="sxs-lookup"><span data-stu-id="68679-143">Conditions define constraints that must be met.</span></span> <span data-ttu-id="68679-144">Например, требование, которое участник является владельцем целевого объекта.</span><span class="sxs-lookup"><span data-stu-id="68679-144">For example, a requirement that the principal be an "owner" of the target.</span></span> <span data-ttu-id="68679-145">Ниже приведены поддерживаемые условия.</span><span class="sxs-lookup"><span data-stu-id="68679-145">The following are the supported conditions:</span></span>

- <span data-ttu-id="68679-146">Само: "@Subject. objectId = = @Resource. objectId"</span><span class="sxs-lookup"><span data-stu-id="68679-146">Self: "@Subject.objectId == @Resource.objectId"</span></span>
- <span data-ttu-id="68679-147">Owner: "@Subject. objectId Any_of @Resource. Owners"</span><span class="sxs-lookup"><span data-stu-id="68679-147">Owner: "@Subject.objectId Any_of @Resource.owners"</span></span>

<span data-ttu-id="68679-148">Ниже приведен пример разрешения роли с условием.</span><span class="sxs-lookup"><span data-stu-id="68679-148">The following is an example of a role permission with a condition.</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="68679-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="68679-149">JSON representation</span></span>

<span data-ttu-id="68679-150">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="68679-150">The following is a JSON representation of the resource.</span></span>

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
## <a name="see-also"></a><span data-ttu-id="68679-151">См. также</span><span class="sxs-lookup"><span data-stu-id="68679-151">See also</span></span>

- <span data-ttu-id="68679-152">[Разрешения роли администратора в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles) — сведения о разрешениях для встроенных ролей каталогов.</span><span class="sxs-lookup"><span data-stu-id="68679-152">[Administrator role permissions in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles) - For information about permissions for built-in directory roles.</span></span>
- <span data-ttu-id="68679-153">[Подтипы регистрации приложений и разрешения в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/roles-custom-available-permissions) — сведения о разрешениях, доступных для пользовательских ролей каталога.</span><span class="sxs-lookup"><span data-stu-id="68679-153">[Application registration subtypes and permissions in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/roles-custom-available-permissions) -  For information about permissions that are available for custom directory roles.</span></span> 

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unifiedRolePermission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
