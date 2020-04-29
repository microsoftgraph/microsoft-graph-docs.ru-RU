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
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="6174e-103">Тип ресурса managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="6174e-103">managedAppPolicy resource type</span></span>

<span data-ttu-id="6174e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6174e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6174e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6174e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6174e-106">Ресурс ManagedAppPolicy представляет базовый тип политик для определенных платформ.</span><span class="sxs-lookup"><span data-stu-id="6174e-106">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>

## <a name="methods"></a><span data-ttu-id="6174e-107">Методы</span><span class="sxs-lookup"><span data-stu-id="6174e-107">Methods</span></span>
|<span data-ttu-id="6174e-108">Метод</span><span class="sxs-lookup"><span data-stu-id="6174e-108">Method</span></span>|<span data-ttu-id="6174e-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6174e-109">Return Type</span></span>|<span data-ttu-id="6174e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6174e-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6174e-111">Список объектов managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="6174e-111">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="6174e-112">Коллекция [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6174e-112">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="6174e-113">Список свойств и связей объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6174e-113">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="6174e-114">Получение объекта managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="6174e-114">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="6174e-115">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="6174e-115">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="6174e-116">Чтение свойств и связей объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6174e-116">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="6174e-117">Действие targetApps</span><span class="sxs-lookup"><span data-stu-id="6174e-117">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="6174e-118">Нет</span><span class="sxs-lookup"><span data-stu-id="6174e-118">None</span></span>|<span data-ttu-id="6174e-119">Н/Д</span><span class="sxs-lookup"><span data-stu-id="6174e-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="6174e-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="6174e-120">Properties</span></span>
|<span data-ttu-id="6174e-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="6174e-121">Property</span></span>|<span data-ttu-id="6174e-122">Тип</span><span class="sxs-lookup"><span data-stu-id="6174e-122">Type</span></span>|<span data-ttu-id="6174e-123">Описание</span><span class="sxs-lookup"><span data-stu-id="6174e-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6174e-124">displayName</span><span class="sxs-lookup"><span data-stu-id="6174e-124">displayName</span></span>|<span data-ttu-id="6174e-125">Строка</span><span class="sxs-lookup"><span data-stu-id="6174e-125">String</span></span>|<span data-ttu-id="6174e-126">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="6174e-126">Policy display name.</span></span>|
|<span data-ttu-id="6174e-127">description</span><span class="sxs-lookup"><span data-stu-id="6174e-127">description</span></span>|<span data-ttu-id="6174e-128">String</span><span class="sxs-lookup"><span data-stu-id="6174e-128">String</span></span>|<span data-ttu-id="6174e-129">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="6174e-129">The policy's description.</span></span>|
|<span data-ttu-id="6174e-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6174e-130">createdDateTime</span></span>|<span data-ttu-id="6174e-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6174e-131">DateTimeOffset</span></span>|<span data-ttu-id="6174e-132">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="6174e-132">The date and time the policy was created.</span></span>|
|<span data-ttu-id="6174e-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6174e-133">lastModifiedDateTime</span></span>|<span data-ttu-id="6174e-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6174e-134">DateTimeOffset</span></span>|<span data-ttu-id="6174e-135">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="6174e-135">Last time the policy was modified.</span></span>|
|<span data-ttu-id="6174e-136">id</span><span class="sxs-lookup"><span data-stu-id="6174e-136">id</span></span>|<span data-ttu-id="6174e-137">String</span><span class="sxs-lookup"><span data-stu-id="6174e-137">String</span></span>|<span data-ttu-id="6174e-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6174e-138">Key of the entity.</span></span>|
|<span data-ttu-id="6174e-139">version</span><span class="sxs-lookup"><span data-stu-id="6174e-139">version</span></span>|<span data-ttu-id="6174e-140">String</span><span class="sxs-lookup"><span data-stu-id="6174e-140">String</span></span>|<span data-ttu-id="6174e-141">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="6174e-141">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6174e-142">Связи</span><span class="sxs-lookup"><span data-stu-id="6174e-142">Relationships</span></span>
<span data-ttu-id="6174e-143">Нет</span><span class="sxs-lookup"><span data-stu-id="6174e-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6174e-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6174e-144">JSON Representation</span></span>
<span data-ttu-id="6174e-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6174e-145">Here is a JSON representation of the resource.</span></span>
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







