---
title: Тип ресурса managedAppPolicy
description: Ресурс ManagedAppPolicy представляет базовый тип политик для определенных платформ.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7f0e26ea51641bf2a291802d391bfaace18da31f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43468520"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="dba65-103">Тип ресурса managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="dba65-103">managedAppPolicy resource type</span></span>

<span data-ttu-id="dba65-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dba65-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dba65-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dba65-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dba65-106">Ресурс ManagedAppPolicy представляет базовый тип политик для определенных платформ.</span><span class="sxs-lookup"><span data-stu-id="dba65-106">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>

## <a name="methods"></a><span data-ttu-id="dba65-107">Методы</span><span class="sxs-lookup"><span data-stu-id="dba65-107">Methods</span></span>
|<span data-ttu-id="dba65-108">Метод</span><span class="sxs-lookup"><span data-stu-id="dba65-108">Method</span></span>|<span data-ttu-id="dba65-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="dba65-109">Return Type</span></span>|<span data-ttu-id="dba65-110">Описание</span><span class="sxs-lookup"><span data-stu-id="dba65-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="dba65-111">Список объектов managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="dba65-111">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="dba65-112">Коллекция [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="dba65-112">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="dba65-113">Список свойств и связей объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dba65-113">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="dba65-114">Получение объекта managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="dba65-114">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="dba65-115">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="dba65-115">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="dba65-116">Чтение свойств и связей объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dba65-116">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="dba65-117">Действие targetApps</span><span class="sxs-lookup"><span data-stu-id="dba65-117">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="dba65-118">Нет</span><span class="sxs-lookup"><span data-stu-id="dba65-118">None</span></span>|<span data-ttu-id="dba65-119">Н/Д</span><span class="sxs-lookup"><span data-stu-id="dba65-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="dba65-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="dba65-120">Properties</span></span>
|<span data-ttu-id="dba65-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="dba65-121">Property</span></span>|<span data-ttu-id="dba65-122">Тип</span><span class="sxs-lookup"><span data-stu-id="dba65-122">Type</span></span>|<span data-ttu-id="dba65-123">Описание</span><span class="sxs-lookup"><span data-stu-id="dba65-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dba65-124">displayName</span><span class="sxs-lookup"><span data-stu-id="dba65-124">displayName</span></span>|<span data-ttu-id="dba65-125">Строка</span><span class="sxs-lookup"><span data-stu-id="dba65-125">String</span></span>|<span data-ttu-id="dba65-126">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="dba65-126">Policy display name.</span></span>|
|<span data-ttu-id="dba65-127">description</span><span class="sxs-lookup"><span data-stu-id="dba65-127">description</span></span>|<span data-ttu-id="dba65-128">String</span><span class="sxs-lookup"><span data-stu-id="dba65-128">String</span></span>|<span data-ttu-id="dba65-129">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="dba65-129">The policy's description.</span></span>|
|<span data-ttu-id="dba65-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dba65-130">createdDateTime</span></span>|<span data-ttu-id="dba65-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dba65-131">DateTimeOffset</span></span>|<span data-ttu-id="dba65-132">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="dba65-132">The date and time the policy was created.</span></span>|
|<span data-ttu-id="dba65-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dba65-133">lastModifiedDateTime</span></span>|<span data-ttu-id="dba65-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dba65-134">DateTimeOffset</span></span>|<span data-ttu-id="dba65-135">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="dba65-135">Last time the policy was modified.</span></span>|
|<span data-ttu-id="dba65-136">id</span><span class="sxs-lookup"><span data-stu-id="dba65-136">id</span></span>|<span data-ttu-id="dba65-137">String</span><span class="sxs-lookup"><span data-stu-id="dba65-137">String</span></span>|<span data-ttu-id="dba65-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="dba65-138">Key of the entity.</span></span>|
|<span data-ttu-id="dba65-139">version</span><span class="sxs-lookup"><span data-stu-id="dba65-139">version</span></span>|<span data-ttu-id="dba65-140">String</span><span class="sxs-lookup"><span data-stu-id="dba65-140">String</span></span>|<span data-ttu-id="dba65-141">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="dba65-141">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dba65-142">Отношения</span><span class="sxs-lookup"><span data-stu-id="dba65-142">Relationships</span></span>
<span data-ttu-id="dba65-143">Нет</span><span class="sxs-lookup"><span data-stu-id="dba65-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dba65-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dba65-144">JSON Representation</span></span>
<span data-ttu-id="dba65-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dba65-145">Here is a JSON representation of the resource.</span></span>
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
  "id": "String (identifier)",
  "version": "String"
}
```







