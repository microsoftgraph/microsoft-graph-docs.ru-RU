---
title: Тип ресурса roleScopeTag
description: Тег области роли
author: tfitzmac
ms.openlocfilehash: 49059ceddcd043f39f51c563c85ba8986b6fc61b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354770"
---
# <a name="rolescopetag-resource-type"></a><span data-ttu-id="18ab7-103">Тип ресурса roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="18ab7-103">roleScopeTag resource type</span></span>

> <span data-ttu-id="18ab7-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="18ab7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="18ab7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18ab7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="18ab7-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="18ab7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="18ab7-107">Тег области роли</span><span class="sxs-lookup"><span data-stu-id="18ab7-107">Role Scope Tag</span></span>
## <a name="methods"></a><span data-ttu-id="18ab7-108">Методы</span><span class="sxs-lookup"><span data-stu-id="18ab7-108">Methods</span></span>
|<span data-ttu-id="18ab7-109">Метод</span><span class="sxs-lookup"><span data-stu-id="18ab7-109">Method</span></span>|<span data-ttu-id="18ab7-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="18ab7-110">Return Type</span></span>|<span data-ttu-id="18ab7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="18ab7-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="18ab7-112">Список roleScopeTags</span><span class="sxs-lookup"><span data-stu-id="18ab7-112">List roleScopeTags</span></span>](../api/intune-rbac-rolescopetag-list.md)|<span data-ttu-id="18ab7-113">[roleScopeTag](../resources/intune-rbac-rolescopetag.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="18ab7-113">[roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection</span></span>|<span data-ttu-id="18ab7-114">Свойства списка и связей объектов [roleScopeTag](../resources/intune-rbac-rolescopetag.md) .</span><span class="sxs-lookup"><span data-stu-id="18ab7-114">List properties and relationships of the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) objects.</span></span>|
|[<span data-ttu-id="18ab7-115">Получение roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="18ab7-115">Get roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-get.md)|[<span data-ttu-id="18ab7-116">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="18ab7-116">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="18ab7-117">Чтение свойства и связи объекта [roleScopeTag](../resources/intune-rbac-rolescopetag.md) .</span><span class="sxs-lookup"><span data-stu-id="18ab7-117">Read properties and relationships of the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|
|[<span data-ttu-id="18ab7-118">Создание roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="18ab7-118">Create roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-create.md)|[<span data-ttu-id="18ab7-119">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="18ab7-119">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="18ab7-120">Создание нового объекта [roleScopeTag](../resources/intune-rbac-rolescopetag.md) .</span><span class="sxs-lookup"><span data-stu-id="18ab7-120">Create a new [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|
|[<span data-ttu-id="18ab7-121">Удаление roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="18ab7-121">Delete roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-delete.md)|<span data-ttu-id="18ab7-122">Нет</span><span class="sxs-lookup"><span data-stu-id="18ab7-122">None</span></span>|<span data-ttu-id="18ab7-123">Удаляет [roleScopeTag](../resources/intune-rbac-rolescopetag.md).</span><span class="sxs-lookup"><span data-stu-id="18ab7-123">Deletes a [roleScopeTag](../resources/intune-rbac-rolescopetag.md).</span></span>|
|[<span data-ttu-id="18ab7-124">Обновление roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="18ab7-124">Update roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-update.md)|[<span data-ttu-id="18ab7-125">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="18ab7-125">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="18ab7-126">Обновление свойства объекта [roleScopeTag](../resources/intune-rbac-rolescopetag.md) .</span><span class="sxs-lookup"><span data-stu-id="18ab7-126">Update the properties of a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="18ab7-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="18ab7-127">Properties</span></span>
|<span data-ttu-id="18ab7-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="18ab7-128">Property</span></span>|<span data-ttu-id="18ab7-129">Тип</span><span class="sxs-lookup"><span data-stu-id="18ab7-129">Type</span></span>|<span data-ttu-id="18ab7-130">Описание</span><span class="sxs-lookup"><span data-stu-id="18ab7-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18ab7-131">id</span><span class="sxs-lookup"><span data-stu-id="18ab7-131">id</span></span>|<span data-ttu-id="18ab7-132">Строка</span><span class="sxs-lookup"><span data-stu-id="18ab7-132">String</span></span>|<span data-ttu-id="18ab7-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="18ab7-133">Key of the entity.</span></span> <span data-ttu-id="18ab7-134">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="18ab7-134">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="18ab7-135">displayName</span><span class="sxs-lookup"><span data-stu-id="18ab7-135">displayName</span></span>|<span data-ttu-id="18ab7-136">Строка</span><span class="sxs-lookup"><span data-stu-id="18ab7-136">String</span></span>|<span data-ttu-id="18ab7-137">Отображение или понятное имя тега область роли.</span><span class="sxs-lookup"><span data-stu-id="18ab7-137">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="18ab7-138">описание</span><span class="sxs-lookup"><span data-stu-id="18ab7-138">description</span></span>|<span data-ttu-id="18ab7-139">Строка</span><span class="sxs-lookup"><span data-stu-id="18ab7-139">String</span></span>|<span data-ttu-id="18ab7-140">Описание тег область роли.</span><span class="sxs-lookup"><span data-stu-id="18ab7-140">Description of the Role Scope Tag.</span></span>|

## <a name="relationships"></a><span data-ttu-id="18ab7-141">Связи</span><span class="sxs-lookup"><span data-stu-id="18ab7-141">Relationships</span></span>
<span data-ttu-id="18ab7-142">Нет</span><span class="sxs-lookup"><span data-stu-id="18ab7-142">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="18ab7-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="18ab7-143">JSON Representation</span></span>
<span data-ttu-id="18ab7-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="18ab7-144">Here is a JSON representation of the resource.</span></span>
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





