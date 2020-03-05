---
title: Тип ресурса roleAssignment
description: Ресурс назначения роли. Назначения ролей объединяют определение роли с участниками и областями. Одной роли может соответствовать одно или несколько назначений. Это относится как к пользовательским, так и ко встроенным ролям.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b398e008c7e3047754b67d55ac31c5235bb2d06d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447943"
---
# <a name="roleassignment-resource-type"></a><span data-ttu-id="e85b2-106">Тип ресурса roleAssignment</span><span class="sxs-lookup"><span data-stu-id="e85b2-106">roleAssignment resource type</span></span>

<span data-ttu-id="e85b2-107">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e85b2-107">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e85b2-108">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e85b2-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e85b2-109">Ресурс назначения роли.</span><span class="sxs-lookup"><span data-stu-id="e85b2-109">The Role Assignment resource.</span></span> <span data-ttu-id="e85b2-110">Назначения ролей объединяют определение роли с участниками и областями.</span><span class="sxs-lookup"><span data-stu-id="e85b2-110">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="e85b2-111">Одной роли может соответствовать одно или несколько назначений.</span><span class="sxs-lookup"><span data-stu-id="e85b2-111">There can be one or more role assignments per role.</span></span> <span data-ttu-id="e85b2-112">Это относится как к пользовательским, так и ко встроенным ролям.</span><span class="sxs-lookup"><span data-stu-id="e85b2-112">This applies to custom and built-in roles.</span></span>

## <a name="methods"></a><span data-ttu-id="e85b2-113">Методы</span><span class="sxs-lookup"><span data-stu-id="e85b2-113">Methods</span></span>
|<span data-ttu-id="e85b2-114">Метод</span><span class="sxs-lookup"><span data-stu-id="e85b2-114">Method</span></span>|<span data-ttu-id="e85b2-115">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e85b2-115">Return Type</span></span>|<span data-ttu-id="e85b2-116">Описание</span><span class="sxs-lookup"><span data-stu-id="e85b2-116">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e85b2-117">Список объектов roleAssignment</span><span class="sxs-lookup"><span data-stu-id="e85b2-117">List roleAssignments</span></span>](../api/intune-rbac-roleassignment-list.md)|<span data-ttu-id="e85b2-118">Коллекция объектов [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="e85b2-118">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="e85b2-119">Список свойств и связей объектов [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e85b2-119">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>|
|[<span data-ttu-id="e85b2-120">Получение объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="e85b2-120">Get roleAssignment</span></span>](../api/intune-rbac-roleassignment-get.md)|<span data-ttu-id="e85b2-121">[roleAssignment](../resources/intune-rbac-roleassignment.md);</span><span class="sxs-lookup"><span data-stu-id="e85b2-121">[roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|<span data-ttu-id="e85b2-122">Чтение свойств и связей объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e85b2-122">Read properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="e85b2-123">Создание объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="e85b2-123">Create roleAssignment</span></span>](../api/intune-rbac-roleassignment-create.md)|<span data-ttu-id="e85b2-124">[roleAssignment](../resources/intune-rbac-roleassignment.md);</span><span class="sxs-lookup"><span data-stu-id="e85b2-124">[roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|<span data-ttu-id="e85b2-125">Создание объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e85b2-125">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="e85b2-126">Удаление объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="e85b2-126">Delete roleAssignment</span></span>](../api/intune-rbac-roleassignment-delete.md)|<span data-ttu-id="e85b2-127">Нет</span><span class="sxs-lookup"><span data-stu-id="e85b2-127">None</span></span>|<span data-ttu-id="e85b2-128">Удаляет объект [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e85b2-128">Deletes a [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>|
|[<span data-ttu-id="e85b2-129">Обновление объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="e85b2-129">Update roleAssignment</span></span>](../api/intune-rbac-roleassignment-update.md)|[<span data-ttu-id="e85b2-130">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="e85b2-130">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="e85b2-131">Обновление свойств объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e85b2-131">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e85b2-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="e85b2-132">Properties</span></span>
|<span data-ttu-id="e85b2-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="e85b2-133">Property</span></span>|<span data-ttu-id="e85b2-134">Тип</span><span class="sxs-lookup"><span data-stu-id="e85b2-134">Type</span></span>|<span data-ttu-id="e85b2-135">Описание</span><span class="sxs-lookup"><span data-stu-id="e85b2-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e85b2-136">id</span><span class="sxs-lookup"><span data-stu-id="e85b2-136">id</span></span>|<span data-ttu-id="e85b2-137">String</span><span class="sxs-lookup"><span data-stu-id="e85b2-137">String</span></span>|<span data-ttu-id="e85b2-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e85b2-138">Key of the entity.</span></span> <span data-ttu-id="e85b2-139">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="e85b2-139">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="e85b2-140">displayName</span><span class="sxs-lookup"><span data-stu-id="e85b2-140">displayName</span></span>|<span data-ttu-id="e85b2-141">Строка</span><span class="sxs-lookup"><span data-stu-id="e85b2-141">String</span></span>|<span data-ttu-id="e85b2-142">Отображаемое или понятное имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="e85b2-142">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="e85b2-143">description</span><span class="sxs-lookup"><span data-stu-id="e85b2-143">description</span></span>|<span data-ttu-id="e85b2-144">String</span><span class="sxs-lookup"><span data-stu-id="e85b2-144">String</span></span>|<span data-ttu-id="e85b2-145">Описание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="e85b2-145">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="e85b2-146">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="e85b2-146">resourceScopes</span></span>|<span data-ttu-id="e85b2-147">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e85b2-147">String collection</span></span>|<span data-ttu-id="e85b2-148">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="e85b2-148">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="e85b2-149">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e85b2-149">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e85b2-150">Связи</span><span class="sxs-lookup"><span data-stu-id="e85b2-150">Relationships</span></span>
|<span data-ttu-id="e85b2-151">Связь</span><span class="sxs-lookup"><span data-stu-id="e85b2-151">Relationship</span></span>|<span data-ttu-id="e85b2-152">Тип</span><span class="sxs-lookup"><span data-stu-id="e85b2-152">Type</span></span>|<span data-ttu-id="e85b2-153">Описание</span><span class="sxs-lookup"><span data-stu-id="e85b2-153">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e85b2-154">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="e85b2-154">roleDefinition</span></span>|[<span data-ttu-id="e85b2-155">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="e85b2-155">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="e85b2-156">Определение роли, частью которого является это назначение.</span><span class="sxs-lookup"><span data-stu-id="e85b2-156">Role definition this assignment is part of.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e85b2-157">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e85b2-157">JSON Representation</span></span>
<span data-ttu-id="e85b2-158">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e85b2-158">Here is a JSON representation of the resource.</span></span>
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




