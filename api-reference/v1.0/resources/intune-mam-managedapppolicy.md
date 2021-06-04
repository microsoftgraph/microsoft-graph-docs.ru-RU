---
title: Тип ресурса managedAppPolicy
description: Ресурс ManagedAppPolicy представляет базовый тип политик для определенных платформ.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 61fedfab47ee44d187d2de81c0699885c4af06f4
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752779"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="62205-103">Тип ресурса managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="62205-103">managedAppPolicy resource type</span></span>

<span data-ttu-id="62205-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62205-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="62205-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="62205-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62205-106">Ресурс ManagedAppPolicy представляет базовый тип политик для определенных платформ.</span><span class="sxs-lookup"><span data-stu-id="62205-106">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>

## <a name="methods"></a><span data-ttu-id="62205-107">Методы</span><span class="sxs-lookup"><span data-stu-id="62205-107">Methods</span></span>
|<span data-ttu-id="62205-108">Метод</span><span class="sxs-lookup"><span data-stu-id="62205-108">Method</span></span>|<span data-ttu-id="62205-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="62205-109">Return Type</span></span>|<span data-ttu-id="62205-110">Описание</span><span class="sxs-lookup"><span data-stu-id="62205-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="62205-111">Список объектов managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="62205-111">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="62205-112">Коллекция [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="62205-112">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="62205-113">Список свойств и связей объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="62205-113">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="62205-114">Получение объекта managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="62205-114">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="62205-115">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="62205-115">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="62205-116">Чтение свойств и связей объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="62205-116">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="62205-117">Действие targetApps</span><span class="sxs-lookup"><span data-stu-id="62205-117">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="62205-118">Нет</span><span class="sxs-lookup"><span data-stu-id="62205-118">None</span></span>|<span data-ttu-id="62205-119">Н/Д</span><span class="sxs-lookup"><span data-stu-id="62205-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="62205-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="62205-120">Properties</span></span>
|<span data-ttu-id="62205-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="62205-121">Property</span></span>|<span data-ttu-id="62205-122">Тип</span><span class="sxs-lookup"><span data-stu-id="62205-122">Type</span></span>|<span data-ttu-id="62205-123">Описание</span><span class="sxs-lookup"><span data-stu-id="62205-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62205-124">displayName</span><span class="sxs-lookup"><span data-stu-id="62205-124">displayName</span></span>|<span data-ttu-id="62205-125">String</span><span class="sxs-lookup"><span data-stu-id="62205-125">String</span></span>|<span data-ttu-id="62205-126">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="62205-126">Policy display name.</span></span>|
|<span data-ttu-id="62205-127">description</span><span class="sxs-lookup"><span data-stu-id="62205-127">description</span></span>|<span data-ttu-id="62205-128">String</span><span class="sxs-lookup"><span data-stu-id="62205-128">String</span></span>|<span data-ttu-id="62205-129">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="62205-129">The policy's description.</span></span>|
|<span data-ttu-id="62205-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="62205-130">createdDateTime</span></span>|<span data-ttu-id="62205-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62205-131">DateTimeOffset</span></span>|<span data-ttu-id="62205-132">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="62205-132">The date and time the policy was created.</span></span>|
|<span data-ttu-id="62205-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="62205-133">lastModifiedDateTime</span></span>|<span data-ttu-id="62205-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62205-134">DateTimeOffset</span></span>|<span data-ttu-id="62205-135">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="62205-135">Last time the policy was modified.</span></span>|
|<span data-ttu-id="62205-136">id</span><span class="sxs-lookup"><span data-stu-id="62205-136">id</span></span>|<span data-ttu-id="62205-137">String</span><span class="sxs-lookup"><span data-stu-id="62205-137">String</span></span>|<span data-ttu-id="62205-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="62205-138">Key of the entity.</span></span>|
|<span data-ttu-id="62205-139">version</span><span class="sxs-lookup"><span data-stu-id="62205-139">version</span></span>|<span data-ttu-id="62205-140">String</span><span class="sxs-lookup"><span data-stu-id="62205-140">String</span></span>|<span data-ttu-id="62205-141">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="62205-141">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="62205-142">Отношения</span><span class="sxs-lookup"><span data-stu-id="62205-142">Relationships</span></span>
<span data-ttu-id="62205-143">Нет</span><span class="sxs-lookup"><span data-stu-id="62205-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="62205-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="62205-144">JSON Representation</span></span>
<span data-ttu-id="62205-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="62205-145">Here is a JSON representation of the resource.</span></span>
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




