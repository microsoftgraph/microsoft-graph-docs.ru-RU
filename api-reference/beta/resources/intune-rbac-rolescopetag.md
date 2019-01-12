---
title: Тип ресурса roleScopeTag
description: Тег области роли
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 609d4202069f6e4258c9824a65b72ab769c365b2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981856"
---
# <a name="rolescopetag-resource-type"></a><span data-ttu-id="28623-103">Тип ресурса roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="28623-103">roleScopeTag resource type</span></span>

> <span data-ttu-id="28623-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="28623-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="28623-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28623-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="28623-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="28623-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="28623-107">Тег области роли</span><span class="sxs-lookup"><span data-stu-id="28623-107">Role Scope Tag</span></span>
## <a name="methods"></a><span data-ttu-id="28623-108">Методы</span><span class="sxs-lookup"><span data-stu-id="28623-108">Methods</span></span>
|<span data-ttu-id="28623-109">Метод</span><span class="sxs-lookup"><span data-stu-id="28623-109">Method</span></span>|<span data-ttu-id="28623-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="28623-110">Return Type</span></span>|<span data-ttu-id="28623-111">Описание</span><span class="sxs-lookup"><span data-stu-id="28623-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="28623-112">Список roleScopeTags</span><span class="sxs-lookup"><span data-stu-id="28623-112">List roleScopeTags</span></span>](../api/intune-rbac-rolescopetag-list.md)|<span data-ttu-id="28623-113">[roleScopeTag](../resources/intune-rbac-rolescopetag.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="28623-113">[roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection</span></span>|<span data-ttu-id="28623-114">Свойства списка и связей объектов [roleScopeTag](../resources/intune-rbac-rolescopetag.md) .</span><span class="sxs-lookup"><span data-stu-id="28623-114">List properties and relationships of the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) objects.</span></span>|
|[<span data-ttu-id="28623-115">Получение roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="28623-115">Get roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-get.md)|[<span data-ttu-id="28623-116">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="28623-116">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="28623-117">Чтение свойства и связи объекта [roleScopeTag](../resources/intune-rbac-rolescopetag.md) .</span><span class="sxs-lookup"><span data-stu-id="28623-117">Read properties and relationships of the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|
|[<span data-ttu-id="28623-118">Создание roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="28623-118">Create roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-create.md)|[<span data-ttu-id="28623-119">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="28623-119">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="28623-120">Создание нового объекта [roleScopeTag](../resources/intune-rbac-rolescopetag.md) .</span><span class="sxs-lookup"><span data-stu-id="28623-120">Create a new [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|
|[<span data-ttu-id="28623-121">Удаление roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="28623-121">Delete roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-delete.md)|<span data-ttu-id="28623-122">Нет</span><span class="sxs-lookup"><span data-stu-id="28623-122">None</span></span>|<span data-ttu-id="28623-123">Удаляет [roleScopeTag](../resources/intune-rbac-rolescopetag.md).</span><span class="sxs-lookup"><span data-stu-id="28623-123">Deletes a [roleScopeTag](../resources/intune-rbac-rolescopetag.md).</span></span>|
|[<span data-ttu-id="28623-124">Обновление roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="28623-124">Update roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-update.md)|[<span data-ttu-id="28623-125">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="28623-125">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="28623-126">Обновление свойства объекта [roleScopeTag](../resources/intune-rbac-rolescopetag.md) .</span><span class="sxs-lookup"><span data-stu-id="28623-126">Update the properties of a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="28623-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="28623-127">Properties</span></span>
|<span data-ttu-id="28623-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="28623-128">Property</span></span>|<span data-ttu-id="28623-129">Тип</span><span class="sxs-lookup"><span data-stu-id="28623-129">Type</span></span>|<span data-ttu-id="28623-130">Описание</span><span class="sxs-lookup"><span data-stu-id="28623-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28623-131">id</span><span class="sxs-lookup"><span data-stu-id="28623-131">id</span></span>|<span data-ttu-id="28623-132">String</span><span class="sxs-lookup"><span data-stu-id="28623-132">String</span></span>|<span data-ttu-id="28623-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="28623-133">Key of the entity.</span></span> <span data-ttu-id="28623-134">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="28623-134">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="28623-135">displayName</span><span class="sxs-lookup"><span data-stu-id="28623-135">displayName</span></span>|<span data-ttu-id="28623-136">String</span><span class="sxs-lookup"><span data-stu-id="28623-136">String</span></span>|<span data-ttu-id="28623-137">Отображение или понятное имя тега область роли.</span><span class="sxs-lookup"><span data-stu-id="28623-137">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="28623-138">описание</span><span class="sxs-lookup"><span data-stu-id="28623-138">description</span></span>|<span data-ttu-id="28623-139">String</span><span class="sxs-lookup"><span data-stu-id="28623-139">String</span></span>|<span data-ttu-id="28623-140">Описание тег область роли.</span><span class="sxs-lookup"><span data-stu-id="28623-140">Description of the Role Scope Tag.</span></span>|

## <a name="relationships"></a><span data-ttu-id="28623-141">Связи</span><span class="sxs-lookup"><span data-stu-id="28623-141">Relationships</span></span>
<span data-ttu-id="28623-142">Нет</span><span class="sxs-lookup"><span data-stu-id="28623-142">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="28623-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="28623-143">JSON Representation</span></span>
<span data-ttu-id="28623-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="28623-144">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleScopeTag"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```





