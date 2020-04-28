---
title: Тип ресурса managedAppPolicy
description: Ресурс ManagedAppPolicy представляет базовый тип политик для определенных платформ.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ed9d53d683b8808ec92741d62958c0ce96fc6a55
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43372378"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="8eff0-103">Тип ресурса managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="8eff0-103">managedAppPolicy resource type</span></span>

<span data-ttu-id="8eff0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8eff0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8eff0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8eff0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8eff0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8eff0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8eff0-107">Ресурс ManagedAppPolicy представляет базовый тип политик для определенных платформ.</span><span class="sxs-lookup"><span data-stu-id="8eff0-107">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>

## <a name="methods"></a><span data-ttu-id="8eff0-108">Методы</span><span class="sxs-lookup"><span data-stu-id="8eff0-108">Methods</span></span>
|<span data-ttu-id="8eff0-109">Метод</span><span class="sxs-lookup"><span data-stu-id="8eff0-109">Method</span></span>|<span data-ttu-id="8eff0-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8eff0-110">Return Type</span></span>|<span data-ttu-id="8eff0-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8eff0-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8eff0-112">Список объектов managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="8eff0-112">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="8eff0-113">Коллекция [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8eff0-113">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="8eff0-114">Список свойств и связей объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8eff0-114">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="8eff0-115">Получение объекта managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="8eff0-115">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="8eff0-116">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="8eff0-116">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="8eff0-117">Чтение свойств и связей объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="8eff0-117">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="8eff0-118">Действие targetApps</span><span class="sxs-lookup"><span data-stu-id="8eff0-118">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="8eff0-119">Нет</span><span class="sxs-lookup"><span data-stu-id="8eff0-119">None</span></span>|<span data-ttu-id="8eff0-120">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8eff0-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="8eff0-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="8eff0-121">Properties</span></span>
|<span data-ttu-id="8eff0-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="8eff0-122">Property</span></span>|<span data-ttu-id="8eff0-123">Тип</span><span class="sxs-lookup"><span data-stu-id="8eff0-123">Type</span></span>|<span data-ttu-id="8eff0-124">Описание</span><span class="sxs-lookup"><span data-stu-id="8eff0-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8eff0-125">displayName</span><span class="sxs-lookup"><span data-stu-id="8eff0-125">displayName</span></span>|<span data-ttu-id="8eff0-126">Строка</span><span class="sxs-lookup"><span data-stu-id="8eff0-126">String</span></span>|<span data-ttu-id="8eff0-127">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="8eff0-127">Policy display name.</span></span>|
|<span data-ttu-id="8eff0-128">description</span><span class="sxs-lookup"><span data-stu-id="8eff0-128">description</span></span>|<span data-ttu-id="8eff0-129">String</span><span class="sxs-lookup"><span data-stu-id="8eff0-129">String</span></span>|<span data-ttu-id="8eff0-130">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="8eff0-130">The policy's description.</span></span>|
|<span data-ttu-id="8eff0-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8eff0-131">createdDateTime</span></span>|<span data-ttu-id="8eff0-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8eff0-132">DateTimeOffset</span></span>|<span data-ttu-id="8eff0-133">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="8eff0-133">The date and time the policy was created.</span></span>|
|<span data-ttu-id="8eff0-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8eff0-134">lastModifiedDateTime</span></span>|<span data-ttu-id="8eff0-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8eff0-135">DateTimeOffset</span></span>|<span data-ttu-id="8eff0-136">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="8eff0-136">Last time the policy was modified.</span></span>|
|<span data-ttu-id="8eff0-137">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8eff0-137">roleScopeTagIds</span></span>|<span data-ttu-id="8eff0-138">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="8eff0-138">String collection</span></span>|<span data-ttu-id="8eff0-139">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="8eff0-139">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="8eff0-140">id</span><span class="sxs-lookup"><span data-stu-id="8eff0-140">id</span></span>|<span data-ttu-id="8eff0-141">String</span><span class="sxs-lookup"><span data-stu-id="8eff0-141">String</span></span>|<span data-ttu-id="8eff0-142">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8eff0-142">Key of the entity.</span></span>|
|<span data-ttu-id="8eff0-143">version</span><span class="sxs-lookup"><span data-stu-id="8eff0-143">version</span></span>|<span data-ttu-id="8eff0-144">String</span><span class="sxs-lookup"><span data-stu-id="8eff0-144">String</span></span>|<span data-ttu-id="8eff0-145">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="8eff0-145">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8eff0-146">Связи</span><span class="sxs-lookup"><span data-stu-id="8eff0-146">Relationships</span></span>
<span data-ttu-id="8eff0-147">Нет</span><span class="sxs-lookup"><span data-stu-id="8eff0-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8eff0-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8eff0-148">JSON Representation</span></span>
<span data-ttu-id="8eff0-149">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8eff0-149">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppPolicy",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "id": "String (identifier)",
  "version": "String"
}
```



