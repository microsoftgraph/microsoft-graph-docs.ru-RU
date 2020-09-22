---
title: Тип ресурса managedAppPolicy
description: Ресурс ManagedAppPolicy представляет базовый тип политик для определенных платформ.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b502364cdcc461601b8790955bb93710be336e24
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48030276"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="e16ae-103">Тип ресурса managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="e16ae-103">managedAppPolicy resource type</span></span>

<span data-ttu-id="e16ae-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e16ae-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e16ae-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e16ae-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e16ae-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e16ae-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e16ae-107">Ресурс ManagedAppPolicy представляет базовый тип политик для определенных платформ.</span><span class="sxs-lookup"><span data-stu-id="e16ae-107">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>

## <a name="methods"></a><span data-ttu-id="e16ae-108">Методы</span><span class="sxs-lookup"><span data-stu-id="e16ae-108">Methods</span></span>
|<span data-ttu-id="e16ae-109">Метод</span><span class="sxs-lookup"><span data-stu-id="e16ae-109">Method</span></span>|<span data-ttu-id="e16ae-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e16ae-110">Return Type</span></span>|<span data-ttu-id="e16ae-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e16ae-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e16ae-112">Список объектов managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="e16ae-112">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="e16ae-113">Коллекция [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e16ae-113">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="e16ae-114">Список свойств и связей объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e16ae-114">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="e16ae-115">Получение объекта managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="e16ae-115">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="e16ae-116">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="e16ae-116">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="e16ae-117">Чтение свойств и связей объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e16ae-117">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="e16ae-118">Действие targetApps</span><span class="sxs-lookup"><span data-stu-id="e16ae-118">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="e16ae-119">Нет</span><span class="sxs-lookup"><span data-stu-id="e16ae-119">None</span></span>|<span data-ttu-id="e16ae-120">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e16ae-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="e16ae-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="e16ae-121">Properties</span></span>
|<span data-ttu-id="e16ae-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="e16ae-122">Property</span></span>|<span data-ttu-id="e16ae-123">Тип</span><span class="sxs-lookup"><span data-stu-id="e16ae-123">Type</span></span>|<span data-ttu-id="e16ae-124">Описание</span><span class="sxs-lookup"><span data-stu-id="e16ae-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e16ae-125">displayName</span><span class="sxs-lookup"><span data-stu-id="e16ae-125">displayName</span></span>|<span data-ttu-id="e16ae-126">String</span><span class="sxs-lookup"><span data-stu-id="e16ae-126">String</span></span>|<span data-ttu-id="e16ae-127">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="e16ae-127">Policy display name.</span></span>|
|<span data-ttu-id="e16ae-128">description</span><span class="sxs-lookup"><span data-stu-id="e16ae-128">description</span></span>|<span data-ttu-id="e16ae-129">String</span><span class="sxs-lookup"><span data-stu-id="e16ae-129">String</span></span>|<span data-ttu-id="e16ae-130">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="e16ae-130">The policy's description.</span></span>|
|<span data-ttu-id="e16ae-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e16ae-131">createdDateTime</span></span>|<span data-ttu-id="e16ae-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e16ae-132">DateTimeOffset</span></span>|<span data-ttu-id="e16ae-133">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="e16ae-133">The date and time the policy was created.</span></span>|
|<span data-ttu-id="e16ae-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e16ae-134">lastModifiedDateTime</span></span>|<span data-ttu-id="e16ae-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e16ae-135">DateTimeOffset</span></span>|<span data-ttu-id="e16ae-136">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="e16ae-136">Last time the policy was modified.</span></span>|
|<span data-ttu-id="e16ae-137">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e16ae-137">roleScopeTagIds</span></span>|<span data-ttu-id="e16ae-138">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e16ae-138">String collection</span></span>|<span data-ttu-id="e16ae-139">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="e16ae-139">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="e16ae-140">id</span><span class="sxs-lookup"><span data-stu-id="e16ae-140">id</span></span>|<span data-ttu-id="e16ae-141">String</span><span class="sxs-lookup"><span data-stu-id="e16ae-141">String</span></span>|<span data-ttu-id="e16ae-142">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e16ae-142">Key of the entity.</span></span>|
|<span data-ttu-id="e16ae-143">version</span><span class="sxs-lookup"><span data-stu-id="e16ae-143">version</span></span>|<span data-ttu-id="e16ae-144">String</span><span class="sxs-lookup"><span data-stu-id="e16ae-144">String</span></span>|<span data-ttu-id="e16ae-145">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="e16ae-145">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e16ae-146">Отношения</span><span class="sxs-lookup"><span data-stu-id="e16ae-146">Relationships</span></span>
<span data-ttu-id="e16ae-147">Нет</span><span class="sxs-lookup"><span data-stu-id="e16ae-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e16ae-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e16ae-148">JSON Representation</span></span>
<span data-ttu-id="e16ae-149">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e16ae-149">Here is a JSON representation of the resource.</span></span>
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






