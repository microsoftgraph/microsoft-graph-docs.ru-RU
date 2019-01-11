---
title: Тип ресурса roleAssignment
description: Ресурс назначения роли. Назначения ролей объединяют определение роли с участниками и областями. Одной роли может соответствовать одно или несколько назначений. Это относится как к настраиваемым, так и ко встроенным ролям.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e8506b87975b69f90cf561e776e557bb472f1ffd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846153"
---
# <a name="roleassignment-resource-type"></a><span data-ttu-id="dc4c1-106">Тип ресурса roleAssignment</span><span class="sxs-lookup"><span data-stu-id="dc4c1-106">roleAssignment resource type</span></span>

> <span data-ttu-id="dc4c1-107">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="dc4c1-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dc4c1-108">Ресурс назначения роли.</span><span class="sxs-lookup"><span data-stu-id="dc4c1-108">The Role Assignment resource.</span></span> <span data-ttu-id="dc4c1-109">Назначения ролей объединяют определение роли с участниками и областями.</span><span class="sxs-lookup"><span data-stu-id="dc4c1-109">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="dc4c1-110">Одной роли может соответствовать одно или несколько назначений.</span><span class="sxs-lookup"><span data-stu-id="dc4c1-110">There can be one or more role assignments per role.</span></span> <span data-ttu-id="dc4c1-111">Это относится как к пользовательским, так и ко встроенным ролям.</span><span class="sxs-lookup"><span data-stu-id="dc4c1-111">This applies to custom and built-in roles.</span></span>
## <a name="methods"></a><span data-ttu-id="dc4c1-112">Методы</span><span class="sxs-lookup"><span data-stu-id="dc4c1-112">Methods</span></span>
|<span data-ttu-id="dc4c1-113">Метод</span><span class="sxs-lookup"><span data-stu-id="dc4c1-113">Method</span></span>|<span data-ttu-id="dc4c1-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="dc4c1-114">Return Type</span></span>|<span data-ttu-id="dc4c1-115">Описание</span><span class="sxs-lookup"><span data-stu-id="dc4c1-115">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="dc4c1-116">Список объектов roleAssignment</span><span class="sxs-lookup"><span data-stu-id="dc4c1-116">List roleAssignments</span></span>](../api/intune-rbac-roleassignment-list.md)|<span data-ttu-id="dc4c1-117">Коллекция объектов [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="dc4c1-117">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="dc4c1-118">Список свойств и связей объектов [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="dc4c1-118">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>|
|[<span data-ttu-id="dc4c1-119">Получение объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="dc4c1-119">Get roleAssignment</span></span>](../api/intune-rbac-roleassignment-get.md)|[<span data-ttu-id="dc4c1-120">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="dc4c1-120">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="dc4c1-121">Чтение свойств и связей объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="dc4c1-121">Read properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="dc4c1-122">Создание объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="dc4c1-122">Create roleAssignment</span></span>](../api/intune-rbac-roleassignment-create.md)|[<span data-ttu-id="dc4c1-123">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="dc4c1-123">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="dc4c1-124">Создание объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="dc4c1-124">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="dc4c1-125">Удаление объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="dc4c1-125">Delete roleAssignment</span></span>](../api/intune-rbac-roleassignment-delete.md)|<span data-ttu-id="dc4c1-126">Нет</span><span class="sxs-lookup"><span data-stu-id="dc4c1-126">None</span></span>|<span data-ttu-id="dc4c1-127">Удаляет объект [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="dc4c1-127">Deletes a [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>|
|[<span data-ttu-id="dc4c1-128">Обновление объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="dc4c1-128">Update roleAssignment</span></span>](../api/intune-rbac-roleassignment-update.md)|[<span data-ttu-id="dc4c1-129">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="dc4c1-129">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="dc4c1-130">Обновление свойств объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="dc4c1-130">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="dc4c1-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="dc4c1-131">Properties</span></span>
|<span data-ttu-id="dc4c1-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="dc4c1-132">Property</span></span>|<span data-ttu-id="dc4c1-133">Тип</span><span class="sxs-lookup"><span data-stu-id="dc4c1-133">Type</span></span>|<span data-ttu-id="dc4c1-134">Описание</span><span class="sxs-lookup"><span data-stu-id="dc4c1-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc4c1-135">id</span><span class="sxs-lookup"><span data-stu-id="dc4c1-135">id</span></span>|<span data-ttu-id="dc4c1-136">Строка</span><span class="sxs-lookup"><span data-stu-id="dc4c1-136">String</span></span>|<span data-ttu-id="dc4c1-137">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="dc4c1-137">Key of the entity.</span></span> <span data-ttu-id="dc4c1-138">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="dc4c1-138">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="dc4c1-139">displayName</span><span class="sxs-lookup"><span data-stu-id="dc4c1-139">displayName</span></span>|<span data-ttu-id="dc4c1-140">String</span><span class="sxs-lookup"><span data-stu-id="dc4c1-140">String</span></span>|<span data-ttu-id="dc4c1-141">Отображаемое или понятное имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="dc4c1-141">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="dc4c1-142">описание</span><span class="sxs-lookup"><span data-stu-id="dc4c1-142">description</span></span>|<span data-ttu-id="dc4c1-143">String</span><span class="sxs-lookup"><span data-stu-id="dc4c1-143">String</span></span>|<span data-ttu-id="dc4c1-144">Описание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="dc4c1-144">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="dc4c1-145">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="dc4c1-145">resourceScopes</span></span>|<span data-ttu-id="dc4c1-146">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="dc4c1-146">String collection</span></span>|<span data-ttu-id="dc4c1-147">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="dc4c1-147">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="dc4c1-148">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="dc4c1-148">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dc4c1-149">Связи</span><span class="sxs-lookup"><span data-stu-id="dc4c1-149">Relationships</span></span>
|<span data-ttu-id="dc4c1-150">Связь</span><span class="sxs-lookup"><span data-stu-id="dc4c1-150">Relationship</span></span>|<span data-ttu-id="dc4c1-151">Тип</span><span class="sxs-lookup"><span data-stu-id="dc4c1-151">Type</span></span>|<span data-ttu-id="dc4c1-152">Описание</span><span class="sxs-lookup"><span data-stu-id="dc4c1-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc4c1-153">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="dc4c1-153">roleDefinition</span></span>|[<span data-ttu-id="dc4c1-154">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="dc4c1-154">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="dc4c1-155">Определение роли, частью которого является это назначение.</span><span class="sxs-lookup"><span data-stu-id="dc4c1-155">Role definition this assignment is part of.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dc4c1-156">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dc4c1-156">JSON Representation</span></span>
<span data-ttu-id="dc4c1-157">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dc4c1-157">Here is a JSON representation of the resource.</span></span>
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



