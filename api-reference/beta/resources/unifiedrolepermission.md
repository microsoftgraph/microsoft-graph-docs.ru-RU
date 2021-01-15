---
title: Тип ресурса unifiedRolePermission
description: Разрешение роли каталога — это коллекция разрешенных действий и условий ресурсов.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 45c59567e8926e8ae7fc2429939b2491a8237782
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874286"
---
# <a name="unifiedrolepermission-resource-type"></a><span data-ttu-id="895b6-103">Тип ресурса unifiedRolePermission</span><span class="sxs-lookup"><span data-stu-id="895b6-103">unifiedRolePermission resource type</span></span>

<span data-ttu-id="895b6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="895b6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="895b6-105">Представляет коллекцию разрешенных действий с ресурсами и условия, которые должны быть выполнены, чтобы действие было эффективным.</span><span class="sxs-lookup"><span data-stu-id="895b6-105">Represents a collection of allowed resource actions and the conditions that must be met for the action to be effective.</span></span> <span data-ttu-id="895b6-106">Действия с ресурсами — это задачи, которые могут быть перенаучены для ресурса.</span><span class="sxs-lookup"><span data-stu-id="895b6-106">Resource actions are tasks that can be perfomed on a resource.</span></span> <span data-ttu-id="895b6-107">Например, ресурс приложения поддерживает действия по созданию, обновлению, удалению и сбросу ресурсов паролей.</span><span class="sxs-lookup"><span data-stu-id="895b6-107">For example, the application resource supports create, update, delete, and reset password resource actions.</span></span>

## <a name="properties"></a><span data-ttu-id="895b6-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="895b6-108">Properties</span></span>

| <span data-ttu-id="895b6-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="895b6-109">Property</span></span>     | <span data-ttu-id="895b6-110">Тип</span><span class="sxs-lookup"><span data-stu-id="895b6-110">Type</span></span>        | <span data-ttu-id="895b6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="895b6-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="895b6-112">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="895b6-112">allowedResourceActions</span></span>|<span data-ttu-id="895b6-113">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="895b6-113">String collection</span></span>| <span data-ttu-id="895b6-114">Набор задач, которые можно выполнить с ресурсом.</span><span class="sxs-lookup"><span data-stu-id="895b6-114">Set of tasks that can be performed on a resource.</span></span> |
|<span data-ttu-id="895b6-115">condition</span><span class="sxs-lookup"><span data-stu-id="895b6-115">condition</span></span>|<span data-ttu-id="895b6-116">String</span><span class="sxs-lookup"><span data-stu-id="895b6-116">String</span></span>| <span data-ttu-id="895b6-117">Необязательные ограничения, которые должны быть выполнены, чтобы разрешение было эффективным.</span><span class="sxs-lookup"><span data-stu-id="895b6-117">Optional constraints that must be met for the permission to be effective.</span></span> |

### <a name="allowedresourceactions-property"></a><span data-ttu-id="895b6-118">Свойство allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="895b6-118">allowedResourceActions property</span></span>

<span data-ttu-id="895b6-119">Ниже приводится схема действий с ресурсами.</span><span class="sxs-lookup"><span data-stu-id="895b6-119">The following is the schema for resource actions:</span></span> 

```
<Namespace>/<Entity>/<PropertySet>/<Action>  
```
<span data-ttu-id="895b6-120">Пример: `microsoft.directory/applications/credentials/update`.</span><span class="sxs-lookup"><span data-stu-id="895b6-120">For example: `microsoft.directory/applications/credentials/update`.</span></span>  

- <span data-ttu-id="895b6-121">Пространство имен — службы, которые предоставляет задачу.</span><span class="sxs-lookup"><span data-stu-id="895b6-121">Namespace - The services that exposes the task.</span></span> <span data-ttu-id="895b6-122">Например, все задачи в Azure Active Directory используют пространство имен microsoft.directory.</span><span class="sxs-lookup"><span data-stu-id="895b6-122">For example, all tasks in Azure Active Directory use the namespace microsoft.directory.</span></span>  
- <span data-ttu-id="895b6-123">Сущность — логические функции или компоненты, которые компоненты компоненты, компоненты, которые компоненты службы в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="895b6-123">Entity - The logical features or components exposed by the service in Microsoft Graph.</span></span> <span data-ttu-id="895b6-124">Например, приложения, основные службы или группы.</span><span class="sxs-lookup"><span data-stu-id="895b6-124">For example, applications, service principals, or groups.</span></span>
- <span data-ttu-id="895b6-125">PropertySet — конкретные свойства или аспекты сущности, для которой предоставляется доступ.</span><span class="sxs-lookup"><span data-stu-id="895b6-125">PropertySet - The specific properties or aspects of the entity for which access is being granted.</span></span> <span data-ttu-id="895b6-126">Например, предоставляет возможность чтения URL-адреса ответа, URL-адреса для входа и неявного свойства потока в объекте приложения `microsoft.directory/applications/authentication/read` в Azure  AD.</span><span class="sxs-lookup"><span data-stu-id="895b6-126">For example, `microsoft.directory/applications/authentication/read` grants the ability to read the reply URL, logout URL, and implicit flow property on the **application** object in Azure AD.</span></span> <span data-ttu-id="895b6-127">Для общих наборов свойств зарезервированы следующие имена:</span><span class="sxs-lookup"><span data-stu-id="895b6-127">The following are reserved names for common property sets:</span></span>  
  - <span data-ttu-id="895b6-128">allProperties — назначает все свойства сущности, включая привилегированные свойства.</span><span class="sxs-lookup"><span data-stu-id="895b6-128">allProperties - Designates all properties of the entity, including privileged properties.</span></span> <span data-ttu-id="895b6-129">Примеры: `microsoft.directory/applications/allProperties/read` и `microsoft.directory/applications/allProperties/update` .</span><span class="sxs-lookup"><span data-stu-id="895b6-129">Examples include `microsoft.directory/applications/allProperties/read` and `microsoft.directory/applications/allProperties/update`.</span></span>
  - <span data-ttu-id="895b6-130">basic — назначает общие свойства чтения, но исключает привилегированные свойства.</span><span class="sxs-lookup"><span data-stu-id="895b6-130">basic - Designates common read properties but excludes privileged ones.</span></span> <span data-ttu-id="895b6-131">Например, включает возможность обновления стандартных свойств, таких как `microsoft.directory/applications/basic/update` отображаемая имя.</span><span class="sxs-lookup"><span data-stu-id="895b6-131">For example, `microsoft.directory/applications/basic/update` includes the ability to update standard properties like display name.</span></span>
  - <span data-ttu-id="895b6-132">standard — назначает общие свойства обновления, но исключает привилегированные свойства.</span><span class="sxs-lookup"><span data-stu-id="895b6-132">standard - Designates common update properties but excludes privileged ones.</span></span> <span data-ttu-id="895b6-133">Например, `microsoft.directory/applications/standard/read`.</span><span class="sxs-lookup"><span data-stu-id="895b6-133">For example, `microsoft.directory/applications/standard/read`.</span></span>
- <span data-ttu-id="895b6-134">Действия — предоставленные операции.</span><span class="sxs-lookup"><span data-stu-id="895b6-134">Actions - The operations being granted.</span></span> <span data-ttu-id="895b6-135">В большинстве ситуаций разрешения должны быть выражены с точки зрения CRUD или allTasks.</span><span class="sxs-lookup"><span data-stu-id="895b6-135">In most circumstances, permissions should be expressed in terms of CRUD or allTasks.</span></span> <span data-ttu-id="895b6-136">К действиям относятся:</span><span class="sxs-lookup"><span data-stu-id="895b6-136">Actions include:</span></span>
  - <span data-ttu-id="895b6-137">Create — возможность создания нового экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="895b6-137">Create - The ability to create a new instance of the entity.</span></span>
  - <span data-ttu-id="895b6-138">Чтение — возможность чтения заданного набора свойств (включая allProperties).</span><span class="sxs-lookup"><span data-stu-id="895b6-138">Read - The ability to read a given property set (including allProperties).</span></span>
  - <span data-ttu-id="895b6-139">Update — возможность обновления заданного набора свойств (включая allProperties).</span><span class="sxs-lookup"><span data-stu-id="895b6-139">Update - The ability to update a given property set (including allProperties).</span></span>
  - <span data-ttu-id="895b6-140">Delete — возможность удаления заданного объекта.</span><span class="sxs-lookup"><span data-stu-id="895b6-140">Delete - The ability to delete a given entity.</span></span>
  - <span data-ttu-id="895b6-141">AllTasks — представляет все операции CRUD (создание, чтение, обновление и удаление).</span><span class="sxs-lookup"><span data-stu-id="895b6-141">AllTasks - Represents all CRUD operations (create, read, update, and delete).</span></span> 

### <a name="condition-property"></a><span data-ttu-id="895b6-142">свойство condition</span><span class="sxs-lookup"><span data-stu-id="895b6-142">condition property</span></span>
<span data-ttu-id="895b6-143">Условия определяют ограничения, которые должны быть выполнены.</span><span class="sxs-lookup"><span data-stu-id="895b6-143">Conditions define constraints that must be met.</span></span> <span data-ttu-id="895b6-144">Например, требование, что основной объект является "владельцем" целевого сайта.</span><span class="sxs-lookup"><span data-stu-id="895b6-144">For example, a requirement that the principal be an "owner" of the target.</span></span> <span data-ttu-id="895b6-145">Поддерживаются следующие условия:</span><span class="sxs-lookup"><span data-stu-id="895b6-145">The following are the supported conditions:</span></span>

- <span data-ttu-id="895b6-146">Self: "@Subject.objectId == @Resource.objectId"</span><span class="sxs-lookup"><span data-stu-id="895b6-146">Self: "@Subject.objectId == @Resource.objectId"</span></span>
- <span data-ttu-id="895b6-147">Владелец: "@Subject.objectId Any_of @Resource.owners"</span><span class="sxs-lookup"><span data-stu-id="895b6-147">Owner: "@Subject.objectId Any_of @Resource.owners"</span></span>

<span data-ttu-id="895b6-148">Ниже приводится пример разрешения роли с условием.</span><span class="sxs-lookup"><span data-stu-id="895b6-148">The following is an example of a role permission with a condition.</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="895b6-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="895b6-149">JSON representation</span></span>

<span data-ttu-id="895b6-150">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="895b6-150">The following is a JSON representation of the resource.</span></span>

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
## <a name="see-also"></a><span data-ttu-id="895b6-151">См. также</span><span class="sxs-lookup"><span data-stu-id="895b6-151">See also</span></span>

- <span data-ttu-id="895b6-152">[Разрешения роли администратора в Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles) — сведения о разрешениях для встроенных ролей каталога.</span><span class="sxs-lookup"><span data-stu-id="895b6-152">[Administrator role permissions in Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles) - For information about permissions for built-in directory roles.</span></span>
- <span data-ttu-id="895b6-153">[Подтипы и](/azure/active-directory/users-groups-roles/roles-custom-available-permissions) разрешения регистрации приложений в Azure Active Directory — сведения о разрешениях, доступных для настраиваемой роли каталога.</span><span class="sxs-lookup"><span data-stu-id="895b6-153">[Application registration subtypes and permissions in Azure Active Directory](/azure/active-directory/users-groups-roles/roles-custom-available-permissions) -  For information about permissions that are available for custom directory roles.</span></span> 

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unifiedRolePermission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->