---
title: Тип ресурса managedAppPolicy
description: Ресурс ManagedAppPolicy представляет базовый тип политик для определенных платформ.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 140e9541cf6719c5348e6ed06e713f5c3e0757b3
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48726355"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="0f3ac-103">Тип ресурса managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="0f3ac-103">managedAppPolicy resource type</span></span>

<span data-ttu-id="0f3ac-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f3ac-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0f3ac-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f3ac-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0f3ac-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0f3ac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f3ac-107">Ресурс ManagedAppPolicy представляет базовый тип политик для определенных платформ.</span><span class="sxs-lookup"><span data-stu-id="0f3ac-107">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>

## <a name="methods"></a><span data-ttu-id="0f3ac-108">Методы</span><span class="sxs-lookup"><span data-stu-id="0f3ac-108">Methods</span></span>
|<span data-ttu-id="0f3ac-109">Метод</span><span class="sxs-lookup"><span data-stu-id="0f3ac-109">Method</span></span>|<span data-ttu-id="0f3ac-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0f3ac-110">Return Type</span></span>|<span data-ttu-id="0f3ac-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0f3ac-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0f3ac-112">Список объектов managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="0f3ac-112">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="0f3ac-113">Коллекция [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0f3ac-113">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="0f3ac-114">Список свойств и связей объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0f3ac-114">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="0f3ac-115">Получение объекта managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="0f3ac-115">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="0f3ac-116">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="0f3ac-116">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="0f3ac-117">Чтение свойств и связей объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0f3ac-117">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="0f3ac-118">Действие targetApps</span><span class="sxs-lookup"><span data-stu-id="0f3ac-118">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="0f3ac-119">Нет</span><span class="sxs-lookup"><span data-stu-id="0f3ac-119">None</span></span>|<span data-ttu-id="0f3ac-120">Н/Д</span><span class="sxs-lookup"><span data-stu-id="0f3ac-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="0f3ac-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="0f3ac-121">Properties</span></span>
|<span data-ttu-id="0f3ac-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="0f3ac-122">Property</span></span>|<span data-ttu-id="0f3ac-123">Тип</span><span class="sxs-lookup"><span data-stu-id="0f3ac-123">Type</span></span>|<span data-ttu-id="0f3ac-124">Описание</span><span class="sxs-lookup"><span data-stu-id="0f3ac-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f3ac-125">displayName</span><span class="sxs-lookup"><span data-stu-id="0f3ac-125">displayName</span></span>|<span data-ttu-id="0f3ac-126">Строка</span><span class="sxs-lookup"><span data-stu-id="0f3ac-126">String</span></span>|<span data-ttu-id="0f3ac-127">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="0f3ac-127">Policy display name.</span></span>|
|<span data-ttu-id="0f3ac-128">description</span><span class="sxs-lookup"><span data-stu-id="0f3ac-128">description</span></span>|<span data-ttu-id="0f3ac-129">Строка</span><span class="sxs-lookup"><span data-stu-id="0f3ac-129">String</span></span>|<span data-ttu-id="0f3ac-130">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="0f3ac-130">The policy's description.</span></span>|
|<span data-ttu-id="0f3ac-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0f3ac-131">createdDateTime</span></span>|<span data-ttu-id="0f3ac-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f3ac-132">DateTimeOffset</span></span>|<span data-ttu-id="0f3ac-133">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="0f3ac-133">The date and time the policy was created.</span></span>|
|<span data-ttu-id="0f3ac-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0f3ac-134">lastModifiedDateTime</span></span>|<span data-ttu-id="0f3ac-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f3ac-135">DateTimeOffset</span></span>|<span data-ttu-id="0f3ac-136">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="0f3ac-136">Last time the policy was modified.</span></span>|
|<span data-ttu-id="0f3ac-137">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0f3ac-137">roleScopeTagIds</span></span>|<span data-ttu-id="0f3ac-138">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="0f3ac-138">String collection</span></span>|<span data-ttu-id="0f3ac-139">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="0f3ac-139">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="0f3ac-140">id</span><span class="sxs-lookup"><span data-stu-id="0f3ac-140">id</span></span>|<span data-ttu-id="0f3ac-141">Строка</span><span class="sxs-lookup"><span data-stu-id="0f3ac-141">String</span></span>|<span data-ttu-id="0f3ac-142">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0f3ac-142">Key of the entity.</span></span>|
|<span data-ttu-id="0f3ac-143">version</span><span class="sxs-lookup"><span data-stu-id="0f3ac-143">version</span></span>|<span data-ttu-id="0f3ac-144">String</span><span class="sxs-lookup"><span data-stu-id="0f3ac-144">String</span></span>|<span data-ttu-id="0f3ac-145">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="0f3ac-145">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f3ac-146">Связи</span><span class="sxs-lookup"><span data-stu-id="0f3ac-146">Relationships</span></span>
<span data-ttu-id="0f3ac-147">Нет</span><span class="sxs-lookup"><span data-stu-id="0f3ac-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0f3ac-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0f3ac-148">JSON Representation</span></span>
<span data-ttu-id="0f3ac-149">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0f3ac-149">Here is a JSON representation of the resource.</span></span>
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





