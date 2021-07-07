---
title: тип ресурса unifiedRolePermission
description: Разрешение роли каталога — это набор допустимых действий и условий ресурса.
localization_priority: Normal
author: sureshja
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 6fc799fec39eaa209ac8e74b02743cf84e76a51a
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316492"
---
# <a name="unifiedrolepermission-resource-type"></a><span data-ttu-id="88ccb-103">тип ресурса unifiedRolePermission</span><span class="sxs-lookup"><span data-stu-id="88ccb-103">unifiedRolePermission resource type</span></span>

<span data-ttu-id="88ccb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88ccb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88ccb-105">Представляет коллекцию допустимых действий ресурса и условия, которые должны быть выполнены для эффективного действия.</span><span class="sxs-lookup"><span data-stu-id="88ccb-105">Represents a collection of allowed resource actions and the conditions that must be met for the action to be effective.</span></span> <span data-ttu-id="88ccb-106">Действия ресурса — это задачи, которые можно выполнить на ресурсе.</span><span class="sxs-lookup"><span data-stu-id="88ccb-106">Resource actions are tasks that can be performed on a resource.</span></span> <span data-ttu-id="88ccb-107">Например, ресурс приложения поддерживает создание, обновление, удаление и сброс действий ресурса паролей.</span><span class="sxs-lookup"><span data-stu-id="88ccb-107">For example, the application resource supports create, update, delete, and reset password resource actions.</span></span>

## <a name="properties"></a><span data-ttu-id="88ccb-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="88ccb-108">Properties</span></span>

| <span data-ttu-id="88ccb-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="88ccb-109">Property</span></span>     | <span data-ttu-id="88ccb-110">Тип</span><span class="sxs-lookup"><span data-stu-id="88ccb-110">Type</span></span>        | <span data-ttu-id="88ccb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="88ccb-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="88ccb-112">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="88ccb-112">allowedResourceActions</span></span>|<span data-ttu-id="88ccb-113">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="88ccb-113">String collection</span></span>| <span data-ttu-id="88ccb-114">Набор задач, которые можно выполнить на ресурсе.</span><span class="sxs-lookup"><span data-stu-id="88ccb-114">Set of tasks that can be performed on a resource.</span></span> |
|<span data-ttu-id="88ccb-115">условие</span><span class="sxs-lookup"><span data-stu-id="88ccb-115">condition</span></span>|<span data-ttu-id="88ccb-116">String</span><span class="sxs-lookup"><span data-stu-id="88ccb-116">String</span></span>| <span data-ttu-id="88ccb-117">Необязательные ограничения, которые должны быть выполнены, чтобы разрешение было эффективным.</span><span class="sxs-lookup"><span data-stu-id="88ccb-117">Optional constraints that must be met for the permission to be effective.</span></span> |

### <a name="allowedresourceactions-property"></a><span data-ttu-id="88ccb-118">свойство allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="88ccb-118">allowedResourceActions property</span></span>

<span data-ttu-id="88ccb-119">Ниже приводится схема действий с ресурсами:</span><span class="sxs-lookup"><span data-stu-id="88ccb-119">The following is the schema for resource actions:</span></span> 

```
<Namespace>/<Entity>/<PropertySet>/<Action>  
```
<span data-ttu-id="88ccb-120">Пример: `microsoft.directory/applications/credentials/update`.</span><span class="sxs-lookup"><span data-stu-id="88ccb-120">For example: `microsoft.directory/applications/credentials/update`.</span></span>  

- <span data-ttu-id="88ccb-121">Namespace — службы, которые раскрывают задачу.</span><span class="sxs-lookup"><span data-stu-id="88ccb-121">Namespace - The services that exposes the task.</span></span> <span data-ttu-id="88ccb-122">Например, все задачи в Azure Active Directory использовать пространство имен microsoft.directory.</span><span class="sxs-lookup"><span data-stu-id="88ccb-122">For example, all tasks in Azure Active Directory use the namespace microsoft.directory.</span></span>  
- <span data-ttu-id="88ccb-123">Entity — логические функции или компоненты, открытые службой в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="88ccb-123">Entity - The logical features or components exposed by the service in Microsoft Graph.</span></span> <span data-ttu-id="88ccb-124">Например, приложения, основные службы или группы.</span><span class="sxs-lookup"><span data-stu-id="88ccb-124">For example, applications, service principals, or groups.</span></span>
- <span data-ttu-id="88ccb-125">PropertySet — конкретные свойства или аспекты объекта, для которого предоставляется доступ.</span><span class="sxs-lookup"><span data-stu-id="88ccb-125">PropertySet - The specific properties or aspects of the entity for which access is being granted.</span></span> <span data-ttu-id="88ccb-126">Например, предоставляется возможность чтения URL-адреса ответа, URL-адреса входа и неявного потока на объекте приложения `microsoft.directory/applications/authentication/read` в Azure  AD.</span><span class="sxs-lookup"><span data-stu-id="88ccb-126">For example, `microsoft.directory/applications/authentication/read` grants the ability to read the reply URL, logout URL, and implicit flow property on the **application** object in Azure AD.</span></span> <span data-ttu-id="88ccb-127">Для общих наборов свойств зарезервированы следующие имена:</span><span class="sxs-lookup"><span data-stu-id="88ccb-127">The following are reserved names for common property sets:</span></span>  
  - <span data-ttu-id="88ccb-128">allProperties — назначает все свойства объекта, включая привилегированные свойства.</span><span class="sxs-lookup"><span data-stu-id="88ccb-128">allProperties - Designates all properties of the entity, including privileged properties.</span></span> <span data-ttu-id="88ccb-129">Примеры включают `microsoft.directory/applications/allProperties/read` и `microsoft.directory/applications/allProperties/update` .</span><span class="sxs-lookup"><span data-stu-id="88ccb-129">Examples include `microsoft.directory/applications/allProperties/read` and `microsoft.directory/applications/allProperties/update`.</span></span>
  - <span data-ttu-id="88ccb-130">basic — назначает общие свойства чтения, но исключает привилегированные свойства.</span><span class="sxs-lookup"><span data-stu-id="88ccb-130">basic - Designates common read properties but excludes privileged ones.</span></span> <span data-ttu-id="88ccb-131">Например, включает возможность обновления стандартных свойств, `microsoft.directory/applications/basic/update` таких как имя отображения.</span><span class="sxs-lookup"><span data-stu-id="88ccb-131">For example, `microsoft.directory/applications/basic/update` includes the ability to update standard properties like display name.</span></span>
  - <span data-ttu-id="88ccb-132">стандартный . Назначает общие свойства обновления, но исключает привилегированные.</span><span class="sxs-lookup"><span data-stu-id="88ccb-132">standard - Designates common update properties but excludes privileged ones.</span></span> <span data-ttu-id="88ccb-133">Например, `microsoft.directory/applications/standard/read`.</span><span class="sxs-lookup"><span data-stu-id="88ccb-133">For example, `microsoft.directory/applications/standard/read`.</span></span>
- <span data-ttu-id="88ccb-134">Действия — операции, которые будут предоставлены.</span><span class="sxs-lookup"><span data-stu-id="88ccb-134">Actions - The operations being granted.</span></span> <span data-ttu-id="88ccb-135">В большинстве обстоятельств разрешения должны быть выражены с точки зрения CRUD или allTasks.</span><span class="sxs-lookup"><span data-stu-id="88ccb-135">In most circumstances, permissions should be expressed in terms of CRUD or allTasks.</span></span> <span data-ttu-id="88ccb-136">Действия включают:</span><span class="sxs-lookup"><span data-stu-id="88ccb-136">Actions include:</span></span>
  - <span data-ttu-id="88ccb-137">Create — возможность создания нового экземпляра объекта.</span><span class="sxs-lookup"><span data-stu-id="88ccb-137">Create - The ability to create a new instance of the entity.</span></span>
  - <span data-ttu-id="88ccb-138">Чтение . Возможность чтения заданного набора свойств (включая allProperties).</span><span class="sxs-lookup"><span data-stu-id="88ccb-138">Read - The ability to read a given property set (including allProperties).</span></span>
  - <span data-ttu-id="88ccb-139">Обновление . Возможность обновления данного набора свойств (включая allProperties).</span><span class="sxs-lookup"><span data-stu-id="88ccb-139">Update - The ability to update a given property set (including allProperties).</span></span>
  - <span data-ttu-id="88ccb-140">Удаление — возможность удаления данного объекта.</span><span class="sxs-lookup"><span data-stu-id="88ccb-140">Delete - The ability to delete a given entity.</span></span>
  - <span data-ttu-id="88ccb-141">AllTasks — представляет все операции CRUD (создание, чтение, обновление и удаление).</span><span class="sxs-lookup"><span data-stu-id="88ccb-141">AllTasks - Represents all CRUD operations (create, read, update, and delete).</span></span> 

### <a name="condition-property"></a><span data-ttu-id="88ccb-142">свойство condition</span><span class="sxs-lookup"><span data-stu-id="88ccb-142">condition property</span></span>
<span data-ttu-id="88ccb-143">Условия определяют ограничения, которые должны быть выполнены.</span><span class="sxs-lookup"><span data-stu-id="88ccb-143">Conditions define constraints that must be met.</span></span> <span data-ttu-id="88ccb-144">Например, требование о том, чтобы директор был "владельцем" целевой группы.</span><span class="sxs-lookup"><span data-stu-id="88ccb-144">For example, a requirement that the principal be an "owner" of the target.</span></span> <span data-ttu-id="88ccb-145">Ниже следующую поддержку условий:</span><span class="sxs-lookup"><span data-stu-id="88ccb-145">The following are the supported conditions:</span></span>

- <span data-ttu-id="88ccb-146">Self: "$ResourceIsSelf"</span><span class="sxs-lookup"><span data-stu-id="88ccb-146">Self: "$ResourceIsSelf"</span></span>
- <span data-ttu-id="88ccb-147">Владелец: "$SubjectIsOwner"</span><span class="sxs-lookup"><span data-stu-id="88ccb-147">Owner: "$SubjectIsOwner"</span></span>

<span data-ttu-id="88ccb-148">Ниже приводится пример разрешения на роль с условием.</span><span class="sxs-lookup"><span data-stu-id="88ccb-148">The following is an example of a role permission with a condition.</span></span>

```json
"rolePermissions": [
        {
            "allowedResourceActions": [
                "microsoft.directory/applications/basic/update",
                "microsoft.directory/applications/credentials/update"
            ],
            "condition":  "$SubjectIsOwner"
        }
    ]

```

## <a name="json-representation"></a><span data-ttu-id="88ccb-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="88ccb-149">JSON representation</span></span>

<span data-ttu-id="88ccb-150">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="88ccb-150">The following is a JSON representation of the resource.</span></span>

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
## <a name="see-also"></a><span data-ttu-id="88ccb-151">См. также</span><span class="sxs-lookup"><span data-stu-id="88ccb-151">See also</span></span>

- <span data-ttu-id="88ccb-152">[Разрешения на роль](/azure/active-directory/users-groups-roles/directory-assign-admin-roles) администратора в Azure Active Directory - Сведения о разрешениях для встроенных ролей каталога.</span><span class="sxs-lookup"><span data-stu-id="88ccb-152">[Administrator role permissions in Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles) - For information about permissions for built-in directory roles.</span></span>
- <span data-ttu-id="88ccb-153">[Подтипы](/azure/active-directory/users-groups-roles/roles-custom-available-permissions) и разрешения регистрации приложений в Azure Active Directory - Сведения о разрешениях, доступных для пользовательских ролей каталога.</span><span class="sxs-lookup"><span data-stu-id="88ccb-153">[Application registration subtypes and permissions in Azure Active Directory](/azure/active-directory/users-groups-roles/roles-custom-available-permissions) -  For information about permissions that are available for custom directory roles.</span></span> 

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unifiedRolePermission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
