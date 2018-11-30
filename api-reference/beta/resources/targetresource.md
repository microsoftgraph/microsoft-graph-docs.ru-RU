---
title: Тип ресурса targetResource
description: Указывает коллекцию конечных типов ресурсов, связанные с действием аудита. Каждый тип целевого ресурса наследуют свойства, используйте следующий из данного ресурса.
ms.openlocfilehash: ba3bee7ce89f73ed97610d62676c22d14488ed9f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075229"
---
# <a name="targetresource-resource-type"></a><span data-ttu-id="45537-104">Тип ресурса targetResource</span><span class="sxs-lookup"><span data-stu-id="45537-104">targetResource resource type</span></span>
<span data-ttu-id="45537-105">Указывает коллекцию конечных типов ресурсов, связанные с действием аудита.</span><span class="sxs-lookup"><span data-stu-id="45537-105">Indicates a collection of  target resource types associated with the audit activity.</span></span> <span data-ttu-id="45537-106">Каждый тип целевого ресурса наследуют свойства, используйте следующий из данного ресурса.</span><span class="sxs-lookup"><span data-stu-id="45537-106">Each target resource type will inherit the properties outlined below from this resource.</span></span>


## <a name="properties"></a><span data-ttu-id="45537-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="45537-107">Properties</span></span>
| <span data-ttu-id="45537-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="45537-108">Property</span></span>     | <span data-ttu-id="45537-109">Тип</span><span class="sxs-lookup"><span data-stu-id="45537-109">Type</span></span>   |<span data-ttu-id="45537-110">Описание</span><span class="sxs-lookup"><span data-stu-id="45537-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="45537-111">displayName</span><span class="sxs-lookup"><span data-stu-id="45537-111">displayName</span></span>|<span data-ttu-id="45537-112">String</span><span class="sxs-lookup"><span data-stu-id="45537-112">String</span></span>|<span data-ttu-id="45537-113">Указывает отображаемое имя, описанные в разделе типы назначения ресурсов ниже ресурсов.</span><span class="sxs-lookup"><span data-stu-id="45537-113">Indicates the display name of the resources outlined under Target Resource Types below.</span></span>|
|<span data-ttu-id="45537-114">id</span><span class="sxs-lookup"><span data-stu-id="45537-114">id</span></span>|<span data-ttu-id="45537-115">String</span><span class="sxs-lookup"><span data-stu-id="45537-115">String</span></span>|<span data-ttu-id="45537-116">Указывает уникальный идентификатор ресурса (например: идентификатор пользователя, AppId, RoleId.).</span><span class="sxs-lookup"><span data-stu-id="45537-116">Indicates the Unique Id of the resource (For example: UserId, AppId, RoleId.).</span></span>|
|<span data-ttu-id="45537-117">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="45537-117">modifiedProperties</span></span>|<span data-ttu-id="45537-118">[modifiedProperty](modifiedproperty.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="45537-118">[modifiedProperty](modifiedproperty.md) collection</span></span>|<span data-ttu-id="45537-119">Указывает имя, старое значение и новое значение каждого атрибута, которые изменены.</span><span class="sxs-lookup"><span data-stu-id="45537-119">Indicates name, old value and new value of each attribute that changed.</span></span> <span data-ttu-id="45537-120">Этот параметр доступен для всех действий, «Обновить»</span><span class="sxs-lookup"><span data-stu-id="45537-120">This is applicable for any "Update" activities</span></span>|

### <a name="target-resource-types"></a><span data-ttu-id="45537-121">Типы назначения ресурсов</span><span class="sxs-lookup"><span data-stu-id="45537-121">Target Resource Types</span></span>

<span data-ttu-id="45537-122">Тип ресурса конечного зависит от базового ресурса:</span><span class="sxs-lookup"><span data-stu-id="45537-122">The target resource type varies according to the underlying resource:</span></span>

|<span data-ttu-id="45537-123">Имя ресурса</span><span class="sxs-lookup"><span data-stu-id="45537-123">Resource Name</span></span>| <span data-ttu-id="45537-124">Справочные материалы</span><span class="sxs-lookup"><span data-stu-id="45537-124">Reference</span></span>|
|-------------|----------|
<span data-ttu-id="45537-125">Устройство</span><span class="sxs-lookup"><span data-stu-id="45537-125">Device</span></span>|[<span data-ttu-id="45537-126">targetResourceDevice</span><span class="sxs-lookup"><span data-stu-id="45537-126">targetResourceDevice</span></span>](targetresourcedevice.md)
<span data-ttu-id="45537-127">Каталог</span><span class="sxs-lookup"><span data-stu-id="45537-127">Directory</span></span>|<span data-ttu-id="45537-128">[targetResourceDirectory] (targetresourcedirectory.md]</span><span class="sxs-lookup"><span data-stu-id="45537-128">[targetResourceDirectory](targetresourcedirectory.md]</span></span>
<span data-ttu-id="45537-129">Group</span><span class="sxs-lookup"><span data-stu-id="45537-129">Group</span></span>|[<span data-ttu-id="45537-130">targetResourceGroup</span><span class="sxs-lookup"><span data-stu-id="45537-130">targetResourceGroup</span></span>](targetresourcegroup.md)
<span data-ttu-id="45537-131">Политика</span><span class="sxs-lookup"><span data-stu-id="45537-131">Policy</span></span>|[<span data-ttu-id="45537-132">targetResourcePolicy</span><span class="sxs-lookup"><span data-stu-id="45537-132">targetResourcePolicy</span></span>](targetresourcepolicy.md)
<span data-ttu-id="45537-133">Role</span><span class="sxs-lookup"><span data-stu-id="45537-133">Role</span></span>|[<span data-ttu-id="45537-134">targetResourceRole</span><span class="sxs-lookup"><span data-stu-id="45537-134">targetResourceRole</span></span>](targetresourcerole.md)
<span data-ttu-id="45537-135">Участников-служб</span><span class="sxs-lookup"><span data-stu-id="45537-135">Service Principal</span></span>|[<span data-ttu-id="45537-136">targetResourceServicePrincipal</span><span class="sxs-lookup"><span data-stu-id="45537-136">targetResourceServicePrincipal</span></span>](targetresourceserviceprincipal.md)
<span data-ttu-id="45537-137">User</span><span class="sxs-lookup"><span data-stu-id="45537-137">User</span></span>|[<span data-ttu-id="45537-138">targetResourceUser</span><span class="sxs-lookup"><span data-stu-id="45537-138">targetResourceUser</span></span>](targetresourceuser.md)
<span data-ttu-id="45537-139">Other (другие)</span><span class="sxs-lookup"><span data-stu-id="45537-139">Other</span></span>|[<span data-ttu-id="45537-140">targetResourceOther</span><span class="sxs-lookup"><span data-stu-id="45537-140">targetResourceOther</span></span>](targetresourceother.md)

## <a name="json-representation"></a><span data-ttu-id="45537-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="45537-141">JSON representation</span></span>

<span data-ttu-id="45537-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="45537-142">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResource"
}-->

```json
{
  "displayName": "String",
  "id": "String",
  "modifiedProperties": [{"@odata.type": "microsoft.graph.modifiedProperty"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->