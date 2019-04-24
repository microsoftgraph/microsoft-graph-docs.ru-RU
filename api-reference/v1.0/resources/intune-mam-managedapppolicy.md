---
title: Тип ресурса managedAppPolicy
description: Ресурс ManagedAppPolicy представляет базовый тип политик для определенных платформ.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2615d1331c024c1a04bc7db618e36966cc5bcdff
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32465344"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="87549-103">Тип ресурса managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="87549-103">managedAppPolicy resource type</span></span>

> <span data-ttu-id="87549-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="87549-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87549-105">Ресурс ManagedAppPolicy представляет базовый тип политик для определенных платформ.</span><span class="sxs-lookup"><span data-stu-id="87549-105">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>

## <a name="methods"></a><span data-ttu-id="87549-106">Методы</span><span class="sxs-lookup"><span data-stu-id="87549-106">Methods</span></span>
|<span data-ttu-id="87549-107">Метод</span><span class="sxs-lookup"><span data-stu-id="87549-107">Method</span></span>|<span data-ttu-id="87549-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="87549-108">Return Type</span></span>|<span data-ttu-id="87549-109">Описание</span><span class="sxs-lookup"><span data-stu-id="87549-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="87549-110">Список объектов managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="87549-110">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="87549-111">Коллекция [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="87549-111">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="87549-112">Список свойств и связей объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="87549-112">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="87549-113">Получение объекта managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="87549-113">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="87549-114">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="87549-114">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="87549-115">Чтение свойств и связей объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="87549-115">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="87549-116">Действие targetApps</span><span class="sxs-lookup"><span data-stu-id="87549-116">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="87549-117">Нет</span><span class="sxs-lookup"><span data-stu-id="87549-117">None</span></span>|<span data-ttu-id="87549-118">Н/Д</span><span class="sxs-lookup"><span data-stu-id="87549-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="87549-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="87549-119">Properties</span></span>
|<span data-ttu-id="87549-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="87549-120">Property</span></span>|<span data-ttu-id="87549-121">Тип</span><span class="sxs-lookup"><span data-stu-id="87549-121">Type</span></span>|<span data-ttu-id="87549-122">Описание</span><span class="sxs-lookup"><span data-stu-id="87549-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87549-123">displayName</span><span class="sxs-lookup"><span data-stu-id="87549-123">displayName</span></span>|<span data-ttu-id="87549-124">String</span><span class="sxs-lookup"><span data-stu-id="87549-124">String</span></span>|<span data-ttu-id="87549-125">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="87549-125">Policy display name.</span></span>|
|<span data-ttu-id="87549-126">description</span><span class="sxs-lookup"><span data-stu-id="87549-126">description</span></span>|<span data-ttu-id="87549-127">String</span><span class="sxs-lookup"><span data-stu-id="87549-127">String</span></span>|<span data-ttu-id="87549-128">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="87549-128">The policy's description.</span></span>|
|<span data-ttu-id="87549-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="87549-129">createdDateTime</span></span>|<span data-ttu-id="87549-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87549-130">DateTimeOffset</span></span>|<span data-ttu-id="87549-131">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="87549-131">The date and time the policy was created.</span></span>|
|<span data-ttu-id="87549-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="87549-132">lastModifiedDateTime</span></span>|<span data-ttu-id="87549-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87549-133">DateTimeOffset</span></span>|<span data-ttu-id="87549-134">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="87549-134">Last time the policy was modified.</span></span>|
|<span data-ttu-id="87549-135">id</span><span class="sxs-lookup"><span data-stu-id="87549-135">id</span></span>|<span data-ttu-id="87549-136">Строка</span><span class="sxs-lookup"><span data-stu-id="87549-136">String</span></span>|<span data-ttu-id="87549-137">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="87549-137">Key of the entity.</span></span>|
|<span data-ttu-id="87549-138">version</span><span class="sxs-lookup"><span data-stu-id="87549-138">version</span></span>|<span data-ttu-id="87549-139">String</span><span class="sxs-lookup"><span data-stu-id="87549-139">String</span></span>|<span data-ttu-id="87549-140">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="87549-140">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="87549-141">Отношения</span><span class="sxs-lookup"><span data-stu-id="87549-141">Relationships</span></span>
<span data-ttu-id="87549-142">Нет</span><span class="sxs-lookup"><span data-stu-id="87549-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="87549-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="87549-143">JSON Representation</span></span>
<span data-ttu-id="87549-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="87549-144">Here is a JSON representation of the resource.</span></span>
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



