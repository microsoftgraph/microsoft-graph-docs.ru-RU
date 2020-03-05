---
title: Тип ресурса managedAppPolicy
description: Ресурс ManagedAppPolicy представляет базовый тип политик для определенных платформ.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 55045faa017c852b812c04b2565269773090ee2e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448384"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="bb505-103">Тип ресурса managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="bb505-103">managedAppPolicy resource type</span></span>

<span data-ttu-id="bb505-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="bb505-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bb505-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bb505-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb505-106">Ресурс ManagedAppPolicy представляет базовый тип политик для определенных платформ.</span><span class="sxs-lookup"><span data-stu-id="bb505-106">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>

## <a name="methods"></a><span data-ttu-id="bb505-107">Методы</span><span class="sxs-lookup"><span data-stu-id="bb505-107">Methods</span></span>
|<span data-ttu-id="bb505-108">Метод</span><span class="sxs-lookup"><span data-stu-id="bb505-108">Method</span></span>|<span data-ttu-id="bb505-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bb505-109">Return Type</span></span>|<span data-ttu-id="bb505-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bb505-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bb505-111">Список объектов managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="bb505-111">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="bb505-112">Коллекция [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bb505-112">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="bb505-113">Список свойств и связей объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bb505-113">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="bb505-114">Получение объекта managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="bb505-114">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="bb505-115">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="bb505-115">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="bb505-116">Чтение свойств и связей объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bb505-116">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="bb505-117">Действие targetApps</span><span class="sxs-lookup"><span data-stu-id="bb505-117">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="bb505-118">Нет</span><span class="sxs-lookup"><span data-stu-id="bb505-118">None</span></span>|<span data-ttu-id="bb505-119">Н/Д</span><span class="sxs-lookup"><span data-stu-id="bb505-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="bb505-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="bb505-120">Properties</span></span>
|<span data-ttu-id="bb505-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="bb505-121">Property</span></span>|<span data-ttu-id="bb505-122">Тип</span><span class="sxs-lookup"><span data-stu-id="bb505-122">Type</span></span>|<span data-ttu-id="bb505-123">Описание</span><span class="sxs-lookup"><span data-stu-id="bb505-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb505-124">displayName</span><span class="sxs-lookup"><span data-stu-id="bb505-124">displayName</span></span>|<span data-ttu-id="bb505-125">Строка</span><span class="sxs-lookup"><span data-stu-id="bb505-125">String</span></span>|<span data-ttu-id="bb505-126">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="bb505-126">Policy display name.</span></span>|
|<span data-ttu-id="bb505-127">description</span><span class="sxs-lookup"><span data-stu-id="bb505-127">description</span></span>|<span data-ttu-id="bb505-128">String</span><span class="sxs-lookup"><span data-stu-id="bb505-128">String</span></span>|<span data-ttu-id="bb505-129">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="bb505-129">The policy's description.</span></span>|
|<span data-ttu-id="bb505-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bb505-130">createdDateTime</span></span>|<span data-ttu-id="bb505-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb505-131">DateTimeOffset</span></span>|<span data-ttu-id="bb505-132">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="bb505-132">The date and time the policy was created.</span></span>|
|<span data-ttu-id="bb505-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bb505-133">lastModifiedDateTime</span></span>|<span data-ttu-id="bb505-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb505-134">DateTimeOffset</span></span>|<span data-ttu-id="bb505-135">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="bb505-135">Last time the policy was modified.</span></span>|
|<span data-ttu-id="bb505-136">id</span><span class="sxs-lookup"><span data-stu-id="bb505-136">id</span></span>|<span data-ttu-id="bb505-137">String</span><span class="sxs-lookup"><span data-stu-id="bb505-137">String</span></span>|<span data-ttu-id="bb505-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bb505-138">Key of the entity.</span></span>|
|<span data-ttu-id="bb505-139">version</span><span class="sxs-lookup"><span data-stu-id="bb505-139">version</span></span>|<span data-ttu-id="bb505-140">String</span><span class="sxs-lookup"><span data-stu-id="bb505-140">String</span></span>|<span data-ttu-id="bb505-141">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="bb505-141">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb505-142">Связи</span><span class="sxs-lookup"><span data-stu-id="bb505-142">Relationships</span></span>
<span data-ttu-id="bb505-143">Нет</span><span class="sxs-lookup"><span data-stu-id="bb505-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bb505-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bb505-144">JSON Representation</span></span>
<span data-ttu-id="bb505-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bb505-145">Here is a JSON representation of the resource.</span></span>
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




