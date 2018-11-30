---
title: Тип ресурса roleAssignment
description: Ресурс назначения роли. Назначения ролей объединяют определение роли с участниками и областями. Одной роли может соответствовать одно или несколько назначений. Это относится как к настраиваемым, так и ко встроенным ролям.
ms.openlocfilehash: 8af3c9778fefd2485948a48f1621c9d9e034c6db
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026429"
---
# <a name="roleassignment-resource-type"></a><span data-ttu-id="a510d-106">Тип ресурса roleAssignment</span><span class="sxs-lookup"><span data-stu-id="a510d-106">roleAssignment resource type</span></span>

> <span data-ttu-id="a510d-107">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a510d-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a510d-108">Ресурс назначения роли.</span><span class="sxs-lookup"><span data-stu-id="a510d-108">The Role Assignment resource.</span></span> <span data-ttu-id="a510d-109">Назначения ролей объединяют определение роли с участниками и областями.</span><span class="sxs-lookup"><span data-stu-id="a510d-109">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="a510d-110">Одной роли может соответствовать одно или несколько назначений.</span><span class="sxs-lookup"><span data-stu-id="a510d-110">There can be one or more role assignments per role.</span></span> <span data-ttu-id="a510d-111">Это относится как к пользовательским, так и ко встроенным ролям.</span><span class="sxs-lookup"><span data-stu-id="a510d-111">This applies to custom and built-in roles.</span></span>
## <a name="methods"></a><span data-ttu-id="a510d-112">Методы</span><span class="sxs-lookup"><span data-stu-id="a510d-112">Methods</span></span>
|<span data-ttu-id="a510d-113">Метод</span><span class="sxs-lookup"><span data-stu-id="a510d-113">Method</span></span>|<span data-ttu-id="a510d-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a510d-114">Return Type</span></span>|<span data-ttu-id="a510d-115">Описание</span><span class="sxs-lookup"><span data-stu-id="a510d-115">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a510d-116">Список объектов roleAssignment</span><span class="sxs-lookup"><span data-stu-id="a510d-116">List roleAssignments</span></span>](../api/intune-rbac-roleassignment-list.md)|<span data-ttu-id="a510d-117">Коллекция объектов [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="a510d-117">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="a510d-118">Список свойств и связей объектов [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a510d-118">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>|
|[<span data-ttu-id="a510d-119">Получение объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="a510d-119">Get roleAssignment</span></span>](../api/intune-rbac-roleassignment-get.md)|[<span data-ttu-id="a510d-120">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="a510d-120">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="a510d-121">Чтение свойств и связей объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a510d-121">Read properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="a510d-122">Создание объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="a510d-122">Create roleAssignment</span></span>](../api/intune-rbac-roleassignment-create.md)|[<span data-ttu-id="a510d-123">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="a510d-123">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="a510d-124">Создание объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a510d-124">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="a510d-125">Удаление объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="a510d-125">Delete roleAssignment</span></span>](../api/intune-rbac-roleassignment-delete.md)|<span data-ttu-id="a510d-126">Нет</span><span class="sxs-lookup"><span data-stu-id="a510d-126">None</span></span>|<span data-ttu-id="a510d-127">Удаляет объект [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a510d-127">Deletes a [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>|
|[<span data-ttu-id="a510d-128">Обновление объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="a510d-128">Update roleAssignment</span></span>](../api/intune-rbac-roleassignment-update.md)|[<span data-ttu-id="a510d-129">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="a510d-129">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="a510d-130">Обновление свойств объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a510d-130">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a510d-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="a510d-131">Properties</span></span>
|<span data-ttu-id="a510d-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="a510d-132">Property</span></span>|<span data-ttu-id="a510d-133">Тип</span><span class="sxs-lookup"><span data-stu-id="a510d-133">Type</span></span>|<span data-ttu-id="a510d-134">Описание</span><span class="sxs-lookup"><span data-stu-id="a510d-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a510d-135">id</span><span class="sxs-lookup"><span data-stu-id="a510d-135">id</span></span>|<span data-ttu-id="a510d-136">String</span><span class="sxs-lookup"><span data-stu-id="a510d-136">String</span></span>|<span data-ttu-id="a510d-137">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a510d-137">Key of the entity.</span></span> <span data-ttu-id="a510d-138">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="a510d-138">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="a510d-139">displayName</span><span class="sxs-lookup"><span data-stu-id="a510d-139">displayName</span></span>|<span data-ttu-id="a510d-140">String</span><span class="sxs-lookup"><span data-stu-id="a510d-140">String</span></span>|<span data-ttu-id="a510d-141">Отображаемое или понятное имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="a510d-141">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="a510d-142">описание</span><span class="sxs-lookup"><span data-stu-id="a510d-142">description</span></span>|<span data-ttu-id="a510d-143">String</span><span class="sxs-lookup"><span data-stu-id="a510d-143">String</span></span>|<span data-ttu-id="a510d-144">Описание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="a510d-144">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="a510d-145">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="a510d-145">resourceScopes</span></span>|<span data-ttu-id="a510d-146">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a510d-146">String collection</span></span>|<span data-ttu-id="a510d-147">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="a510d-147">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="a510d-148">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a510d-148">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a510d-149">Связи</span><span class="sxs-lookup"><span data-stu-id="a510d-149">Relationships</span></span>
|<span data-ttu-id="a510d-150">Связь</span><span class="sxs-lookup"><span data-stu-id="a510d-150">Relationship</span></span>|<span data-ttu-id="a510d-151">Тип</span><span class="sxs-lookup"><span data-stu-id="a510d-151">Type</span></span>|<span data-ttu-id="a510d-152">Описание</span><span class="sxs-lookup"><span data-stu-id="a510d-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a510d-153">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="a510d-153">roleDefinition</span></span>|[<span data-ttu-id="a510d-154">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="a510d-154">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="a510d-155">Определение роли, частью которого является это назначение.</span><span class="sxs-lookup"><span data-stu-id="a510d-155">Role definition this assignment is part of.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a510d-156">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a510d-156">JSON Representation</span></span>
<span data-ttu-id="a510d-157">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a510d-157">Here is a JSON representation of the resource.</span></span>
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



