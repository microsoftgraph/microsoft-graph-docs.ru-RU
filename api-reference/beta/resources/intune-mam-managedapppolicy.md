---
title: Тип ресурса managedAppPolicy
description: Ресурс ManagedAppPolicy представляет базовый тип политик для определенных платформ.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e96da6ab943e22b7e779f969abec3c87201df750
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524324"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="6c333-103">Тип ресурса managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="6c333-103">managedAppPolicy resource type</span></span>

<span data-ttu-id="6c333-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6c333-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6c333-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c333-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c333-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6c333-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c333-107">Ресурс ManagedAppPolicy представляет базовый тип политик для определенных платформ.</span><span class="sxs-lookup"><span data-stu-id="6c333-107">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>

## <a name="methods"></a><span data-ttu-id="6c333-108">Методы</span><span class="sxs-lookup"><span data-stu-id="6c333-108">Methods</span></span>
|<span data-ttu-id="6c333-109">Метод</span><span class="sxs-lookup"><span data-stu-id="6c333-109">Method</span></span>|<span data-ttu-id="6c333-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6c333-110">Return Type</span></span>|<span data-ttu-id="6c333-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6c333-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6c333-112">Список объектов managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="6c333-112">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="6c333-113">Коллекция [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6c333-113">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="6c333-114">Список свойств и связей объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6c333-114">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="6c333-115">Получение объекта managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="6c333-115">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="6c333-116">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="6c333-116">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="6c333-117">Чтение свойств и связей объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6c333-117">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="6c333-118">Действие targetApps</span><span class="sxs-lookup"><span data-stu-id="6c333-118">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="6c333-119">Нет</span><span class="sxs-lookup"><span data-stu-id="6c333-119">None</span></span>|<span data-ttu-id="6c333-120">Н/Д</span><span class="sxs-lookup"><span data-stu-id="6c333-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="6c333-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="6c333-121">Properties</span></span>
|<span data-ttu-id="6c333-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="6c333-122">Property</span></span>|<span data-ttu-id="6c333-123">Тип</span><span class="sxs-lookup"><span data-stu-id="6c333-123">Type</span></span>|<span data-ttu-id="6c333-124">Описание</span><span class="sxs-lookup"><span data-stu-id="6c333-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c333-125">displayName</span><span class="sxs-lookup"><span data-stu-id="6c333-125">displayName</span></span>|<span data-ttu-id="6c333-126">Строка</span><span class="sxs-lookup"><span data-stu-id="6c333-126">String</span></span>|<span data-ttu-id="6c333-127">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="6c333-127">Policy display name.</span></span>|
|<span data-ttu-id="6c333-128">description</span><span class="sxs-lookup"><span data-stu-id="6c333-128">description</span></span>|<span data-ttu-id="6c333-129">String</span><span class="sxs-lookup"><span data-stu-id="6c333-129">String</span></span>|<span data-ttu-id="6c333-130">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="6c333-130">The policy's description.</span></span>|
|<span data-ttu-id="6c333-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6c333-131">createdDateTime</span></span>|<span data-ttu-id="6c333-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c333-132">DateTimeOffset</span></span>|<span data-ttu-id="6c333-133">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="6c333-133">The date and time the policy was created.</span></span>|
|<span data-ttu-id="6c333-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6c333-134">lastModifiedDateTime</span></span>|<span data-ttu-id="6c333-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c333-135">DateTimeOffset</span></span>|<span data-ttu-id="6c333-136">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="6c333-136">Last time the policy was modified.</span></span>|
|<span data-ttu-id="6c333-137">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6c333-137">roleScopeTagIds</span></span>|<span data-ttu-id="6c333-138">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6c333-138">String collection</span></span>|<span data-ttu-id="6c333-139">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="6c333-139">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="6c333-140">id</span><span class="sxs-lookup"><span data-stu-id="6c333-140">id</span></span>|<span data-ttu-id="6c333-141">String</span><span class="sxs-lookup"><span data-stu-id="6c333-141">String</span></span>|<span data-ttu-id="6c333-142">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6c333-142">Key of the entity.</span></span>|
|<span data-ttu-id="6c333-143">version</span><span class="sxs-lookup"><span data-stu-id="6c333-143">version</span></span>|<span data-ttu-id="6c333-144">String</span><span class="sxs-lookup"><span data-stu-id="6c333-144">String</span></span>|<span data-ttu-id="6c333-145">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="6c333-145">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6c333-146">Связи</span><span class="sxs-lookup"><span data-stu-id="6c333-146">Relationships</span></span>
<span data-ttu-id="6c333-147">Нет</span><span class="sxs-lookup"><span data-stu-id="6c333-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6c333-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6c333-148">JSON Representation</span></span>
<span data-ttu-id="6c333-149">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6c333-149">Here is a JSON representation of the resource.</span></span>
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



