---
title: Тип ресурса roleAssignment
description: Ресурс назначения роли. Назначения ролей объединяют определение роли с участниками и областями. Одной роли может соответствовать одно или несколько назначений. Это относится как к пользовательским, так и ко встроенным ролям.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a2c7713731d75b0f20b2923fb9b9e5e492c7d643
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37360596"
---
# <a name="roleassignment-resource-type"></a><span data-ttu-id="3b1b1-106">Тип ресурса roleAssignment</span><span class="sxs-lookup"><span data-stu-id="3b1b1-106">roleAssignment resource type</span></span>

> <span data-ttu-id="3b1b1-107">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3b1b1-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b1b1-108">Ресурс назначения роли.</span><span class="sxs-lookup"><span data-stu-id="3b1b1-108">The Role Assignment resource.</span></span> <span data-ttu-id="3b1b1-109">Назначения ролей объединяют определение роли с участниками и областями.</span><span class="sxs-lookup"><span data-stu-id="3b1b1-109">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="3b1b1-110">Одной роли может соответствовать одно или несколько назначений.</span><span class="sxs-lookup"><span data-stu-id="3b1b1-110">There can be one or more role assignments per role.</span></span> <span data-ttu-id="3b1b1-111">Это относится как к пользовательским, так и ко встроенным ролям.</span><span class="sxs-lookup"><span data-stu-id="3b1b1-111">This applies to custom and built-in roles.</span></span>

## <a name="methods"></a><span data-ttu-id="3b1b1-112">Методы</span><span class="sxs-lookup"><span data-stu-id="3b1b1-112">Methods</span></span>
|<span data-ttu-id="3b1b1-113">Метод</span><span class="sxs-lookup"><span data-stu-id="3b1b1-113">Method</span></span>|<span data-ttu-id="3b1b1-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3b1b1-114">Return Type</span></span>|<span data-ttu-id="3b1b1-115">Описание</span><span class="sxs-lookup"><span data-stu-id="3b1b1-115">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3b1b1-116">Список объектов roleAssignment</span><span class="sxs-lookup"><span data-stu-id="3b1b1-116">List roleAssignments</span></span>](../api/intune-rbac-roleassignment-list.md)|<span data-ttu-id="3b1b1-117">Коллекция объектов [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="3b1b1-117">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="3b1b1-118">Список свойств и связей объектов [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="3b1b1-118">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>|
|[<span data-ttu-id="3b1b1-119">Получение объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="3b1b1-119">Get roleAssignment</span></span>](../api/intune-rbac-roleassignment-get.md)|<span data-ttu-id="3b1b1-120">[roleAssignment](../resources/intune-rbac-roleassignment.md);</span><span class="sxs-lookup"><span data-stu-id="3b1b1-120">[roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|<span data-ttu-id="3b1b1-121">Чтение свойств и связей объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="3b1b1-121">Read properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="3b1b1-122">Создание объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="3b1b1-122">Create roleAssignment</span></span>](../api/intune-rbac-roleassignment-create.md)|<span data-ttu-id="3b1b1-123">[roleAssignment](../resources/intune-rbac-roleassignment.md);</span><span class="sxs-lookup"><span data-stu-id="3b1b1-123">[roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|<span data-ttu-id="3b1b1-124">Создание объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="3b1b1-124">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="3b1b1-125">Удаление объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="3b1b1-125">Delete roleAssignment</span></span>](../api/intune-rbac-roleassignment-delete.md)|<span data-ttu-id="3b1b1-126">Нет</span><span class="sxs-lookup"><span data-stu-id="3b1b1-126">None</span></span>|<span data-ttu-id="3b1b1-127">Удаляет объект [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="3b1b1-127">Deletes a [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>|
|[<span data-ttu-id="3b1b1-128">Обновление объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="3b1b1-128">Update roleAssignment</span></span>](../api/intune-rbac-roleassignment-update.md)|[<span data-ttu-id="3b1b1-129">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="3b1b1-129">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="3b1b1-130">Обновление свойств объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="3b1b1-130">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3b1b1-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="3b1b1-131">Properties</span></span>
|<span data-ttu-id="3b1b1-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="3b1b1-132">Property</span></span>|<span data-ttu-id="3b1b1-133">Тип</span><span class="sxs-lookup"><span data-stu-id="3b1b1-133">Type</span></span>|<span data-ttu-id="3b1b1-134">Описание</span><span class="sxs-lookup"><span data-stu-id="3b1b1-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b1b1-135">id</span><span class="sxs-lookup"><span data-stu-id="3b1b1-135">id</span></span>|<span data-ttu-id="3b1b1-136">String</span><span class="sxs-lookup"><span data-stu-id="3b1b1-136">String</span></span>|<span data-ttu-id="3b1b1-137">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3b1b1-137">Key of the entity.</span></span> <span data-ttu-id="3b1b1-138">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="3b1b1-138">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="3b1b1-139">displayName</span><span class="sxs-lookup"><span data-stu-id="3b1b1-139">displayName</span></span>|<span data-ttu-id="3b1b1-140">Строка</span><span class="sxs-lookup"><span data-stu-id="3b1b1-140">String</span></span>|<span data-ttu-id="3b1b1-141">Отображаемое или понятное имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="3b1b1-141">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="3b1b1-142">description</span><span class="sxs-lookup"><span data-stu-id="3b1b1-142">description</span></span>|<span data-ttu-id="3b1b1-143">String</span><span class="sxs-lookup"><span data-stu-id="3b1b1-143">String</span></span>|<span data-ttu-id="3b1b1-144">Описание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="3b1b1-144">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="3b1b1-145">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="3b1b1-145">resourceScopes</span></span>|<span data-ttu-id="3b1b1-146">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3b1b1-146">String collection</span></span>|<span data-ttu-id="3b1b1-147">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="3b1b1-147">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="3b1b1-148">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3b1b1-148">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3b1b1-149">Связи</span><span class="sxs-lookup"><span data-stu-id="3b1b1-149">Relationships</span></span>
|<span data-ttu-id="3b1b1-150">Связь</span><span class="sxs-lookup"><span data-stu-id="3b1b1-150">Relationship</span></span>|<span data-ttu-id="3b1b1-151">Тип</span><span class="sxs-lookup"><span data-stu-id="3b1b1-151">Type</span></span>|<span data-ttu-id="3b1b1-152">Описание</span><span class="sxs-lookup"><span data-stu-id="3b1b1-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b1b1-153">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="3b1b1-153">roleDefinition</span></span>|[<span data-ttu-id="3b1b1-154">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="3b1b1-154">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="3b1b1-155">Определение роли, частью которого является это назначение.</span><span class="sxs-lookup"><span data-stu-id="3b1b1-155">Role definition this assignment is part of.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3b1b1-156">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3b1b1-156">JSON Representation</span></span>
<span data-ttu-id="3b1b1-157">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3b1b1-157">Here is a JSON representation of the resource.</span></span>
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




