---
title: Тип ресурса managedAppPolicy
description: Ресурс ManagedAppPolicy представляет базовый тип политик для определенных платформ.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4aef589e8667dd3002175b478203384cd7cb2181
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037984"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="bf3ee-103">Тип ресурса managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="bf3ee-103">managedAppPolicy resource type</span></span>

> <span data-ttu-id="bf3ee-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bf3ee-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf3ee-105">Ресурс ManagedAppPolicy представляет базовый тип политик для определенных платформ.</span><span class="sxs-lookup"><span data-stu-id="bf3ee-105">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>

## <a name="methods"></a><span data-ttu-id="bf3ee-106">Методы</span><span class="sxs-lookup"><span data-stu-id="bf3ee-106">Methods</span></span>
|<span data-ttu-id="bf3ee-107">Метод</span><span class="sxs-lookup"><span data-stu-id="bf3ee-107">Method</span></span>|<span data-ttu-id="bf3ee-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bf3ee-108">Return Type</span></span>|<span data-ttu-id="bf3ee-109">Описание</span><span class="sxs-lookup"><span data-stu-id="bf3ee-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bf3ee-110">Список объектов managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="bf3ee-110">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="bf3ee-111">Коллекция [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bf3ee-111">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="bf3ee-112">Список свойств и связей объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bf3ee-112">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="bf3ee-113">Получение объекта managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="bf3ee-113">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="bf3ee-114">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="bf3ee-114">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="bf3ee-115">Чтение свойств и связей объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bf3ee-115">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="bf3ee-116">Действие targetApps</span><span class="sxs-lookup"><span data-stu-id="bf3ee-116">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="bf3ee-117">Нет</span><span class="sxs-lookup"><span data-stu-id="bf3ee-117">None</span></span>|<span data-ttu-id="bf3ee-118">Н/Д</span><span class="sxs-lookup"><span data-stu-id="bf3ee-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="bf3ee-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="bf3ee-119">Properties</span></span>
|<span data-ttu-id="bf3ee-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="bf3ee-120">Property</span></span>|<span data-ttu-id="bf3ee-121">Тип</span><span class="sxs-lookup"><span data-stu-id="bf3ee-121">Type</span></span>|<span data-ttu-id="bf3ee-122">Описание</span><span class="sxs-lookup"><span data-stu-id="bf3ee-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf3ee-123">displayName</span><span class="sxs-lookup"><span data-stu-id="bf3ee-123">displayName</span></span>|<span data-ttu-id="bf3ee-124">Строка</span><span class="sxs-lookup"><span data-stu-id="bf3ee-124">String</span></span>|<span data-ttu-id="bf3ee-125">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="bf3ee-125">Policy display name.</span></span>|
|<span data-ttu-id="bf3ee-126">description</span><span class="sxs-lookup"><span data-stu-id="bf3ee-126">description</span></span>|<span data-ttu-id="bf3ee-127">String</span><span class="sxs-lookup"><span data-stu-id="bf3ee-127">String</span></span>|<span data-ttu-id="bf3ee-128">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="bf3ee-128">The policy's description.</span></span>|
|<span data-ttu-id="bf3ee-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bf3ee-129">createdDateTime</span></span>|<span data-ttu-id="bf3ee-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf3ee-130">DateTimeOffset</span></span>|<span data-ttu-id="bf3ee-131">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="bf3ee-131">The date and time the policy was created.</span></span>|
|<span data-ttu-id="bf3ee-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bf3ee-132">lastModifiedDateTime</span></span>|<span data-ttu-id="bf3ee-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf3ee-133">DateTimeOffset</span></span>|<span data-ttu-id="bf3ee-134">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="bf3ee-134">Last time the policy was modified.</span></span>|
|<span data-ttu-id="bf3ee-135">id</span><span class="sxs-lookup"><span data-stu-id="bf3ee-135">id</span></span>|<span data-ttu-id="bf3ee-136">String</span><span class="sxs-lookup"><span data-stu-id="bf3ee-136">String</span></span>|<span data-ttu-id="bf3ee-137">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bf3ee-137">Key of the entity.</span></span>|
|<span data-ttu-id="bf3ee-138">version</span><span class="sxs-lookup"><span data-stu-id="bf3ee-138">version</span></span>|<span data-ttu-id="bf3ee-139">String</span><span class="sxs-lookup"><span data-stu-id="bf3ee-139">String</span></span>|<span data-ttu-id="bf3ee-140">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="bf3ee-140">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bf3ee-141">Отношения</span><span class="sxs-lookup"><span data-stu-id="bf3ee-141">Relationships</span></span>
<span data-ttu-id="bf3ee-142">Нет</span><span class="sxs-lookup"><span data-stu-id="bf3ee-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bf3ee-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bf3ee-143">JSON Representation</span></span>
<span data-ttu-id="bf3ee-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bf3ee-144">Here is a JSON representation of the resource.</span></span>
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



