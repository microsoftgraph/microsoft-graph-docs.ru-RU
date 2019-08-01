---
title: Тип ресурса roleAssignment
description: Ресурс назначения роли. Назначения ролей объединяют определение роли с участниками и областями. Одной роли может соответствовать одно или несколько назначений. Это относится как к пользовательским, так и ко встроенным ролям.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 542cd188653465f2482e4a5fe837eeb811fe3bd6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037130"
---
# <a name="roleassignment-resource-type"></a><span data-ttu-id="2aeee-106">Тип ресурса roleAssignment</span><span class="sxs-lookup"><span data-stu-id="2aeee-106">roleAssignment resource type</span></span>

> <span data-ttu-id="2aeee-107">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2aeee-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2aeee-108">Ресурс назначения роли.</span><span class="sxs-lookup"><span data-stu-id="2aeee-108">The Role Assignment resource.</span></span> <span data-ttu-id="2aeee-109">Назначения ролей объединяют определение роли с участниками и областями.</span><span class="sxs-lookup"><span data-stu-id="2aeee-109">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="2aeee-110">Одной роли может соответствовать одно или несколько назначений.</span><span class="sxs-lookup"><span data-stu-id="2aeee-110">There can be one or more role assignments per role.</span></span> <span data-ttu-id="2aeee-111">Это относится как к пользовательским, так и ко встроенным ролям.</span><span class="sxs-lookup"><span data-stu-id="2aeee-111">This applies to custom and built-in roles.</span></span>

## <a name="methods"></a><span data-ttu-id="2aeee-112">Методы</span><span class="sxs-lookup"><span data-stu-id="2aeee-112">Methods</span></span>
|<span data-ttu-id="2aeee-113">Метод</span><span class="sxs-lookup"><span data-stu-id="2aeee-113">Method</span></span>|<span data-ttu-id="2aeee-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2aeee-114">Return Type</span></span>|<span data-ttu-id="2aeee-115">Описание</span><span class="sxs-lookup"><span data-stu-id="2aeee-115">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2aeee-116">Список объектов roleAssignment</span><span class="sxs-lookup"><span data-stu-id="2aeee-116">List roleAssignments</span></span>](../api/intune-rbac-roleassignment-list.md)|<span data-ttu-id="2aeee-117">Коллекция объектов [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="2aeee-117">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="2aeee-118">Список свойств и связей объектов [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2aeee-118">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>|
|[<span data-ttu-id="2aeee-119">Получение объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="2aeee-119">Get roleAssignment</span></span>](../api/intune-rbac-roleassignment-get.md)|<span data-ttu-id="2aeee-120">[roleAssignment](../resources/intune-rbac-roleassignment.md);</span><span class="sxs-lookup"><span data-stu-id="2aeee-120">[roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|<span data-ttu-id="2aeee-121">Чтение свойств и связей объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2aeee-121">Read properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="2aeee-122">Создание объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="2aeee-122">Create roleAssignment</span></span>](../api/intune-rbac-roleassignment-create.md)|<span data-ttu-id="2aeee-123">[roleAssignment](../resources/intune-rbac-roleassignment.md);</span><span class="sxs-lookup"><span data-stu-id="2aeee-123">[roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|<span data-ttu-id="2aeee-124">Создание объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2aeee-124">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="2aeee-125">Удаление объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="2aeee-125">Delete roleAssignment</span></span>](../api/intune-rbac-roleassignment-delete.md)|<span data-ttu-id="2aeee-126">Нет</span><span class="sxs-lookup"><span data-stu-id="2aeee-126">None</span></span>|<span data-ttu-id="2aeee-127">Удаляет объект [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2aeee-127">Deletes a [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>|
|[<span data-ttu-id="2aeee-128">Обновление объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="2aeee-128">Update roleAssignment</span></span>](../api/intune-rbac-roleassignment-update.md)|[<span data-ttu-id="2aeee-129">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="2aeee-129">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="2aeee-130">Обновление свойств объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2aeee-130">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2aeee-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="2aeee-131">Properties</span></span>
|<span data-ttu-id="2aeee-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="2aeee-132">Property</span></span>|<span data-ttu-id="2aeee-133">Тип</span><span class="sxs-lookup"><span data-stu-id="2aeee-133">Type</span></span>|<span data-ttu-id="2aeee-134">Описание</span><span class="sxs-lookup"><span data-stu-id="2aeee-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2aeee-135">id</span><span class="sxs-lookup"><span data-stu-id="2aeee-135">id</span></span>|<span data-ttu-id="2aeee-136">String</span><span class="sxs-lookup"><span data-stu-id="2aeee-136">String</span></span>|<span data-ttu-id="2aeee-137">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2aeee-137">Key of the entity.</span></span> <span data-ttu-id="2aeee-138">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="2aeee-138">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="2aeee-139">displayName</span><span class="sxs-lookup"><span data-stu-id="2aeee-139">displayName</span></span>|<span data-ttu-id="2aeee-140">Строка</span><span class="sxs-lookup"><span data-stu-id="2aeee-140">String</span></span>|<span data-ttu-id="2aeee-141">Отображаемое или понятное имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="2aeee-141">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="2aeee-142">description</span><span class="sxs-lookup"><span data-stu-id="2aeee-142">description</span></span>|<span data-ttu-id="2aeee-143">String</span><span class="sxs-lookup"><span data-stu-id="2aeee-143">String</span></span>|<span data-ttu-id="2aeee-144">Описание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="2aeee-144">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="2aeee-145">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="2aeee-145">resourceScopes</span></span>|<span data-ttu-id="2aeee-146">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="2aeee-146">String collection</span></span>|<span data-ttu-id="2aeee-147">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="2aeee-147">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="2aeee-148">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="2aeee-148">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2aeee-149">Отношения</span><span class="sxs-lookup"><span data-stu-id="2aeee-149">Relationships</span></span>
|<span data-ttu-id="2aeee-150">Отношение</span><span class="sxs-lookup"><span data-stu-id="2aeee-150">Relationship</span></span>|<span data-ttu-id="2aeee-151">Тип</span><span class="sxs-lookup"><span data-stu-id="2aeee-151">Type</span></span>|<span data-ttu-id="2aeee-152">Описание</span><span class="sxs-lookup"><span data-stu-id="2aeee-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2aeee-153">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="2aeee-153">roleDefinition</span></span>|[<span data-ttu-id="2aeee-154">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="2aeee-154">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="2aeee-155">Определение роли, частью которого является это назначение.</span><span class="sxs-lookup"><span data-stu-id="2aeee-155">Role definition this assignment is part of.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2aeee-156">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2aeee-156">JSON Representation</span></span>
<span data-ttu-id="2aeee-157">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2aeee-157">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "resourceScopes": [
    "String"
  ]
}
```



