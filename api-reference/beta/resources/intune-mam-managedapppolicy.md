---
title: Тип ресурса managedAppPolicy
description: Ресурс ManagedAppPolicy представляет базовый тип политик для определенных платформ.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bc3047eed950cc547f47fa45fbf609e86ba025bb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35998382"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="bacc6-103">Тип ресурса managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="bacc6-103">managedAppPolicy resource type</span></span>

> <span data-ttu-id="bacc6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bacc6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bacc6-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bacc6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bacc6-106">Ресурс ManagedAppPolicy представляет базовый тип политик для определенных платформ.</span><span class="sxs-lookup"><span data-stu-id="bacc6-106">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>

## <a name="methods"></a><span data-ttu-id="bacc6-107">Методы</span><span class="sxs-lookup"><span data-stu-id="bacc6-107">Methods</span></span>
|<span data-ttu-id="bacc6-108">Метод</span><span class="sxs-lookup"><span data-stu-id="bacc6-108">Method</span></span>|<span data-ttu-id="bacc6-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bacc6-109">Return Type</span></span>|<span data-ttu-id="bacc6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bacc6-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bacc6-111">Список объектов managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="bacc6-111">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="bacc6-112">Коллекция [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bacc6-112">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="bacc6-113">Список свойств и связей объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bacc6-113">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="bacc6-114">Получение объекта managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="bacc6-114">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="bacc6-115">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="bacc6-115">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="bacc6-116">Чтение свойств и связей объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bacc6-116">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="bacc6-117">Действие targetApps</span><span class="sxs-lookup"><span data-stu-id="bacc6-117">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="bacc6-118">Нет</span><span class="sxs-lookup"><span data-stu-id="bacc6-118">None</span></span>|<span data-ttu-id="bacc6-119">Н/Д</span><span class="sxs-lookup"><span data-stu-id="bacc6-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="bacc6-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="bacc6-120">Properties</span></span>
|<span data-ttu-id="bacc6-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="bacc6-121">Property</span></span>|<span data-ttu-id="bacc6-122">Тип</span><span class="sxs-lookup"><span data-stu-id="bacc6-122">Type</span></span>|<span data-ttu-id="bacc6-123">Описание</span><span class="sxs-lookup"><span data-stu-id="bacc6-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bacc6-124">displayName</span><span class="sxs-lookup"><span data-stu-id="bacc6-124">displayName</span></span>|<span data-ttu-id="bacc6-125">Строка</span><span class="sxs-lookup"><span data-stu-id="bacc6-125">String</span></span>|<span data-ttu-id="bacc6-126">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="bacc6-126">Policy display name.</span></span>|
|<span data-ttu-id="bacc6-127">description</span><span class="sxs-lookup"><span data-stu-id="bacc6-127">description</span></span>|<span data-ttu-id="bacc6-128">String</span><span class="sxs-lookup"><span data-stu-id="bacc6-128">String</span></span>|<span data-ttu-id="bacc6-129">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="bacc6-129">The policy's description.</span></span>|
|<span data-ttu-id="bacc6-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bacc6-130">createdDateTime</span></span>|<span data-ttu-id="bacc6-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bacc6-131">DateTimeOffset</span></span>|<span data-ttu-id="bacc6-132">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="bacc6-132">The date and time the policy was created.</span></span>|
|<span data-ttu-id="bacc6-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bacc6-133">lastModifiedDateTime</span></span>|<span data-ttu-id="bacc6-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bacc6-134">DateTimeOffset</span></span>|<span data-ttu-id="bacc6-135">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="bacc6-135">Last time the policy was modified.</span></span>|
|<span data-ttu-id="bacc6-136">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bacc6-136">roleScopeTagIds</span></span>|<span data-ttu-id="bacc6-137">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="bacc6-137">String collection</span></span>|<span data-ttu-id="bacc6-138">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="bacc6-138">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="bacc6-139">id</span><span class="sxs-lookup"><span data-stu-id="bacc6-139">id</span></span>|<span data-ttu-id="bacc6-140">String</span><span class="sxs-lookup"><span data-stu-id="bacc6-140">String</span></span>|<span data-ttu-id="bacc6-141">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bacc6-141">Key of the entity.</span></span>|
|<span data-ttu-id="bacc6-142">version</span><span class="sxs-lookup"><span data-stu-id="bacc6-142">version</span></span>|<span data-ttu-id="bacc6-143">String</span><span class="sxs-lookup"><span data-stu-id="bacc6-143">String</span></span>|<span data-ttu-id="bacc6-144">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="bacc6-144">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bacc6-145">Отношения</span><span class="sxs-lookup"><span data-stu-id="bacc6-145">Relationships</span></span>
<span data-ttu-id="bacc6-146">Нет</span><span class="sxs-lookup"><span data-stu-id="bacc6-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bacc6-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bacc6-147">JSON Representation</span></span>
<span data-ttu-id="bacc6-148">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bacc6-148">Here is a JSON representation of the resource.</span></span>
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





