---
title: Тип ресурса roleAssignment
description: Ресурс назначения роли. Назначения ролей объединяют определение роли с участниками и областями. Одной роли может соответствовать одно или несколько назначений. Это относится как к пользовательским, так и ко встроенным ролям.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 32527fad8db54f865f054f04400897e51638e5c2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554039"
---
# <a name="roleassignment-resource-type"></a><span data-ttu-id="21775-106">Тип ресурса roleAssignment</span><span class="sxs-lookup"><span data-stu-id="21775-106">roleAssignment resource type</span></span>

> <span data-ttu-id="21775-107">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="21775-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21775-108">Ресурс назначения роли.</span><span class="sxs-lookup"><span data-stu-id="21775-108">The Role Assignment resource.</span></span> <span data-ttu-id="21775-109">Назначения ролей объединяют определение роли с участниками и областями.</span><span class="sxs-lookup"><span data-stu-id="21775-109">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="21775-110">Одной роли может соответствовать одно или несколько назначений.</span><span class="sxs-lookup"><span data-stu-id="21775-110">There can be one or more role assignments per role.</span></span> <span data-ttu-id="21775-111">Это относится как к пользовательским, так и ко встроенным ролям.</span><span class="sxs-lookup"><span data-stu-id="21775-111">This applies to custom and built-in roles.</span></span>

## <a name="methods"></a><span data-ttu-id="21775-112">Методы</span><span class="sxs-lookup"><span data-stu-id="21775-112">Methods</span></span>
|<span data-ttu-id="21775-113">Метод</span><span class="sxs-lookup"><span data-stu-id="21775-113">Method</span></span>|<span data-ttu-id="21775-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="21775-114">Return Type</span></span>|<span data-ttu-id="21775-115">Описание</span><span class="sxs-lookup"><span data-stu-id="21775-115">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="21775-116">Список объектов roleAssignment</span><span class="sxs-lookup"><span data-stu-id="21775-116">List roleAssignments</span></span>](../api/intune-rbac-roleassignment-list.md)|<span data-ttu-id="21775-117">Коллекция объектов [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="21775-117">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="21775-118">Список свойств и связей объектов [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="21775-118">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>|
|[<span data-ttu-id="21775-119">Получение объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="21775-119">Get roleAssignment</span></span>](../api/intune-rbac-roleassignment-get.md)|<span data-ttu-id="21775-120">[roleAssignment](../resources/intune-rbac-roleassignment.md);</span><span class="sxs-lookup"><span data-stu-id="21775-120">[roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|<span data-ttu-id="21775-121">Чтение свойств и связей объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="21775-121">Read properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="21775-122">Создание объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="21775-122">Create roleAssignment</span></span>](../api/intune-rbac-roleassignment-create.md)|<span data-ttu-id="21775-123">[roleAssignment](../resources/intune-rbac-roleassignment.md);</span><span class="sxs-lookup"><span data-stu-id="21775-123">[roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|<span data-ttu-id="21775-124">Создание объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="21775-124">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="21775-125">Удаление объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="21775-125">Delete roleAssignment</span></span>](../api/intune-rbac-roleassignment-delete.md)|<span data-ttu-id="21775-126">Нет</span><span class="sxs-lookup"><span data-stu-id="21775-126">None</span></span>|<span data-ttu-id="21775-127">Удаляет объект [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="21775-127">Deletes a [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>|
|[<span data-ttu-id="21775-128">Обновление объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="21775-128">Update roleAssignment</span></span>](../api/intune-rbac-roleassignment-update.md)|[<span data-ttu-id="21775-129">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="21775-129">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="21775-130">Обновление свойств объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="21775-130">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="21775-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="21775-131">Properties</span></span>
|<span data-ttu-id="21775-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="21775-132">Property</span></span>|<span data-ttu-id="21775-133">Тип</span><span class="sxs-lookup"><span data-stu-id="21775-133">Type</span></span>|<span data-ttu-id="21775-134">Описание</span><span class="sxs-lookup"><span data-stu-id="21775-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21775-135">id</span><span class="sxs-lookup"><span data-stu-id="21775-135">id</span></span>|<span data-ttu-id="21775-136">Строка</span><span class="sxs-lookup"><span data-stu-id="21775-136">String</span></span>|<span data-ttu-id="21775-137">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="21775-137">Key of the entity.</span></span> <span data-ttu-id="21775-138">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="21775-138">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="21775-139">displayName</span><span class="sxs-lookup"><span data-stu-id="21775-139">displayName</span></span>|<span data-ttu-id="21775-140">String</span><span class="sxs-lookup"><span data-stu-id="21775-140">String</span></span>|<span data-ttu-id="21775-141">Отображаемое или понятное имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="21775-141">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="21775-142">description</span><span class="sxs-lookup"><span data-stu-id="21775-142">description</span></span>|<span data-ttu-id="21775-143">String</span><span class="sxs-lookup"><span data-stu-id="21775-143">String</span></span>|<span data-ttu-id="21775-144">Описание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="21775-144">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="21775-145">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="21775-145">resourceScopes</span></span>|<span data-ttu-id="21775-146">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="21775-146">String collection</span></span>|<span data-ttu-id="21775-147">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="21775-147">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="21775-148">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="21775-148">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="21775-149">Связи</span><span class="sxs-lookup"><span data-stu-id="21775-149">Relationships</span></span>
|<span data-ttu-id="21775-150">Отношение</span><span class="sxs-lookup"><span data-stu-id="21775-150">Relationship</span></span>|<span data-ttu-id="21775-151">Тип</span><span class="sxs-lookup"><span data-stu-id="21775-151">Type</span></span>|<span data-ttu-id="21775-152">Описание</span><span class="sxs-lookup"><span data-stu-id="21775-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21775-153">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="21775-153">roleDefinition</span></span>|[<span data-ttu-id="21775-154">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="21775-154">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="21775-155">Определение роли, частью которого является это назначение.</span><span class="sxs-lookup"><span data-stu-id="21775-155">Role definition this assignment is part of.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="21775-156">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="21775-156">JSON Representation</span></span>
<span data-ttu-id="21775-157">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="21775-157">Here is a JSON representation of the resource.</span></span>
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



