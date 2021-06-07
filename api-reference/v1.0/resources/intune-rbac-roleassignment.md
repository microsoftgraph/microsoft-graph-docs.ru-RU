---
title: Тип ресурса roleAssignment
description: Ресурс назначения роли. Назначения ролей объединяют определение роли с участниками и областями. Одной роли может соответствовать одно или несколько назначений. Это относится как к пользовательским, так и ко встроенным ролям.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: af1feaf16cbff0f915982a78a623647803efcd2f
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751197"
---
# <a name="roleassignment-resource-type"></a><span data-ttu-id="5a499-106">Тип ресурса roleAssignment</span><span class="sxs-lookup"><span data-stu-id="5a499-106">roleAssignment resource type</span></span>

<span data-ttu-id="5a499-107">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a499-107">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5a499-108">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5a499-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a499-109">Ресурс назначения роли.</span><span class="sxs-lookup"><span data-stu-id="5a499-109">The Role Assignment resource.</span></span> <span data-ttu-id="5a499-110">Назначения ролей объединяют определение роли с участниками и областями.</span><span class="sxs-lookup"><span data-stu-id="5a499-110">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="5a499-111">Одной роли может соответствовать одно или несколько назначений.</span><span class="sxs-lookup"><span data-stu-id="5a499-111">There can be one or more role assignments per role.</span></span> <span data-ttu-id="5a499-112">Это относится как к пользовательским, так и ко встроенным ролям.</span><span class="sxs-lookup"><span data-stu-id="5a499-112">This applies to custom and built-in roles.</span></span>

## <a name="methods"></a><span data-ttu-id="5a499-113">Методы</span><span class="sxs-lookup"><span data-stu-id="5a499-113">Methods</span></span>
|<span data-ttu-id="5a499-114">Метод</span><span class="sxs-lookup"><span data-stu-id="5a499-114">Method</span></span>|<span data-ttu-id="5a499-115">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5a499-115">Return Type</span></span>|<span data-ttu-id="5a499-116">Описание</span><span class="sxs-lookup"><span data-stu-id="5a499-116">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5a499-117">Список объектов roleAssignment</span><span class="sxs-lookup"><span data-stu-id="5a499-117">List roleAssignments</span></span>](../api/intune-rbac-roleassignment-list.md)|<span data-ttu-id="5a499-118">Коллекция объектов [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5a499-118">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="5a499-119">Список свойств и связей объектов [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5a499-119">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>|
|[<span data-ttu-id="5a499-120">Получение объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="5a499-120">Get roleAssignment</span></span>](../api/intune-rbac-roleassignment-get.md)|[<span data-ttu-id="5a499-121">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="5a499-121">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="5a499-122">Чтение свойств и связей объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5a499-122">Read properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="5a499-123">Создание объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="5a499-123">Create roleAssignment</span></span>](../api/intune-rbac-roleassignment-create.md)|[<span data-ttu-id="5a499-124">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="5a499-124">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="5a499-125">Создание объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5a499-125">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="5a499-126">Удаление объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="5a499-126">Delete roleAssignment</span></span>](../api/intune-rbac-roleassignment-delete.md)|<span data-ttu-id="5a499-127">Нет</span><span class="sxs-lookup"><span data-stu-id="5a499-127">None</span></span>|<span data-ttu-id="5a499-128">Удаляет объект [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5a499-128">Deletes a [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>|
|[<span data-ttu-id="5a499-129">Обновление объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="5a499-129">Update roleAssignment</span></span>](../api/intune-rbac-roleassignment-update.md)|[<span data-ttu-id="5a499-130">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="5a499-130">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="5a499-131">Обновление свойств объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5a499-131">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5a499-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="5a499-132">Properties</span></span>
|<span data-ttu-id="5a499-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="5a499-133">Property</span></span>|<span data-ttu-id="5a499-134">Тип</span><span class="sxs-lookup"><span data-stu-id="5a499-134">Type</span></span>|<span data-ttu-id="5a499-135">Описание</span><span class="sxs-lookup"><span data-stu-id="5a499-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a499-136">id</span><span class="sxs-lookup"><span data-stu-id="5a499-136">id</span></span>|<span data-ttu-id="5a499-137">String</span><span class="sxs-lookup"><span data-stu-id="5a499-137">String</span></span>|<span data-ttu-id="5a499-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5a499-138">Key of the entity.</span></span> <span data-ttu-id="5a499-139">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="5a499-139">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="5a499-140">displayName</span><span class="sxs-lookup"><span data-stu-id="5a499-140">displayName</span></span>|<span data-ttu-id="5a499-141">String</span><span class="sxs-lookup"><span data-stu-id="5a499-141">String</span></span>|<span data-ttu-id="5a499-142">Отображаемое или понятное имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="5a499-142">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="5a499-143">description</span><span class="sxs-lookup"><span data-stu-id="5a499-143">description</span></span>|<span data-ttu-id="5a499-144">String</span><span class="sxs-lookup"><span data-stu-id="5a499-144">String</span></span>|<span data-ttu-id="5a499-145">Описание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="5a499-145">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="5a499-146">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="5a499-146">resourceScopes</span></span>|<span data-ttu-id="5a499-147">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5a499-147">String collection</span></span>|<span data-ttu-id="5a499-148">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="5a499-148">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="5a499-149">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5a499-149">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5a499-150">Отношения</span><span class="sxs-lookup"><span data-stu-id="5a499-150">Relationships</span></span>
|<span data-ttu-id="5a499-151">Связь</span><span class="sxs-lookup"><span data-stu-id="5a499-151">Relationship</span></span>|<span data-ttu-id="5a499-152">Тип</span><span class="sxs-lookup"><span data-stu-id="5a499-152">Type</span></span>|<span data-ttu-id="5a499-153">Описание</span><span class="sxs-lookup"><span data-stu-id="5a499-153">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a499-154">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="5a499-154">roleDefinition</span></span>|[<span data-ttu-id="5a499-155">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="5a499-155">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="5a499-156">Определение роли, частью которого является это назначение.</span><span class="sxs-lookup"><span data-stu-id="5a499-156">Role definition this assignment is part of.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5a499-157">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5a499-157">JSON Representation</span></span>
<span data-ttu-id="5a499-158">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5a499-158">Here is a JSON representation of the resource.</span></span>
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




