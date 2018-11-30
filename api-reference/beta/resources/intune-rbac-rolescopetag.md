---
title: Тип ресурса roleScopeTag
description: Тег области роли
ms.openlocfilehash: 9be1f1307243c18e10f8e6dfc3f302502cdb54a7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078094"
---
# <a name="rolescopetag-resource-type"></a><span data-ttu-id="3000a-103">Тип ресурса roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="3000a-103">roleScopeTag resource type</span></span>

> <span data-ttu-id="3000a-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3000a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3000a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3000a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3000a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3000a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3000a-107">Тег области роли</span><span class="sxs-lookup"><span data-stu-id="3000a-107">Role Scope Tag</span></span>
## <a name="methods"></a><span data-ttu-id="3000a-108">Методы</span><span class="sxs-lookup"><span data-stu-id="3000a-108">Methods</span></span>
|<span data-ttu-id="3000a-109">Метод</span><span class="sxs-lookup"><span data-stu-id="3000a-109">Method</span></span>|<span data-ttu-id="3000a-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3000a-110">Return Type</span></span>|<span data-ttu-id="3000a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3000a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3000a-112">Список roleScopeTags</span><span class="sxs-lookup"><span data-stu-id="3000a-112">List roleScopeTags</span></span>](../api/intune-rbac-rolescopetag-list.md)|<span data-ttu-id="3000a-113">[roleScopeTag](../resources/intune-rbac-rolescopetag.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="3000a-113">[roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection</span></span>|<span data-ttu-id="3000a-114">Свойства списка и связей объектов [roleScopeTag](../resources/intune-rbac-rolescopetag.md) .</span><span class="sxs-lookup"><span data-stu-id="3000a-114">List properties and relationships of the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) objects.</span></span>|
|[<span data-ttu-id="3000a-115">Получение roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="3000a-115">Get roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-get.md)|[<span data-ttu-id="3000a-116">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="3000a-116">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="3000a-117">Чтение свойства и связи объекта [roleScopeTag](../resources/intune-rbac-rolescopetag.md) .</span><span class="sxs-lookup"><span data-stu-id="3000a-117">Read properties and relationships of the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|
|[<span data-ttu-id="3000a-118">Создание roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="3000a-118">Create roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-create.md)|[<span data-ttu-id="3000a-119">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="3000a-119">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="3000a-120">Создание нового объекта [roleScopeTag](../resources/intune-rbac-rolescopetag.md) .</span><span class="sxs-lookup"><span data-stu-id="3000a-120">Create a new [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|
|[<span data-ttu-id="3000a-121">Удаление roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="3000a-121">Delete roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-delete.md)|<span data-ttu-id="3000a-122">Нет</span><span class="sxs-lookup"><span data-stu-id="3000a-122">None</span></span>|<span data-ttu-id="3000a-123">Удаляет [roleScopeTag](../resources/intune-rbac-rolescopetag.md).</span><span class="sxs-lookup"><span data-stu-id="3000a-123">Deletes a [roleScopeTag](../resources/intune-rbac-rolescopetag.md).</span></span>|
|[<span data-ttu-id="3000a-124">Обновление roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="3000a-124">Update roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-update.md)|[<span data-ttu-id="3000a-125">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="3000a-125">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="3000a-126">Обновление свойства объекта [roleScopeTag](../resources/intune-rbac-rolescopetag.md) .</span><span class="sxs-lookup"><span data-stu-id="3000a-126">Update the properties of a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3000a-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="3000a-127">Properties</span></span>
|<span data-ttu-id="3000a-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="3000a-128">Property</span></span>|<span data-ttu-id="3000a-129">Тип</span><span class="sxs-lookup"><span data-stu-id="3000a-129">Type</span></span>|<span data-ttu-id="3000a-130">Описание</span><span class="sxs-lookup"><span data-stu-id="3000a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3000a-131">id</span><span class="sxs-lookup"><span data-stu-id="3000a-131">id</span></span>|<span data-ttu-id="3000a-132">String</span><span class="sxs-lookup"><span data-stu-id="3000a-132">String</span></span>|<span data-ttu-id="3000a-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3000a-133">Key of the entity.</span></span> <span data-ttu-id="3000a-134">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="3000a-134">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="3000a-135">displayName</span><span class="sxs-lookup"><span data-stu-id="3000a-135">displayName</span></span>|<span data-ttu-id="3000a-136">String</span><span class="sxs-lookup"><span data-stu-id="3000a-136">String</span></span>|<span data-ttu-id="3000a-137">Отображение или понятное имя тега область роли.</span><span class="sxs-lookup"><span data-stu-id="3000a-137">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="3000a-138">описание</span><span class="sxs-lookup"><span data-stu-id="3000a-138">description</span></span>|<span data-ttu-id="3000a-139">String</span><span class="sxs-lookup"><span data-stu-id="3000a-139">String</span></span>|<span data-ttu-id="3000a-140">Описание тег область роли.</span><span class="sxs-lookup"><span data-stu-id="3000a-140">Description of the Role Scope Tag.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3000a-141">Связи</span><span class="sxs-lookup"><span data-stu-id="3000a-141">Relationships</span></span>
<span data-ttu-id="3000a-142">Нет</span><span class="sxs-lookup"><span data-stu-id="3000a-142">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3000a-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3000a-143">JSON Representation</span></span>
<span data-ttu-id="3000a-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3000a-144">Here is a JSON representation of the resource.</span></span>
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





