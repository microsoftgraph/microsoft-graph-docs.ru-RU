---
title: Тип ресурса managedAppPolicy
description: Ресурс ManagedAppPolicy представляет базовый тип политик для определенных платформ.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5766e3a467a157bac0d876fd0178dc3ba1cb94e2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888083"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="cf5cf-103">Тип ресурса managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="cf5cf-103">managedAppPolicy resource type</span></span>

> <span data-ttu-id="cf5cf-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="cf5cf-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cf5cf-105">Ресурс ManagedAppPolicy представляет базовый тип политик для определенных платформ.</span><span class="sxs-lookup"><span data-stu-id="cf5cf-105">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>
## <a name="methods"></a><span data-ttu-id="cf5cf-106">Методы</span><span class="sxs-lookup"><span data-stu-id="cf5cf-106">Methods</span></span>
|<span data-ttu-id="cf5cf-107">Метод</span><span class="sxs-lookup"><span data-stu-id="cf5cf-107">Method</span></span>|<span data-ttu-id="cf5cf-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="cf5cf-108">Return Type</span></span>|<span data-ttu-id="cf5cf-109">Описание</span><span class="sxs-lookup"><span data-stu-id="cf5cf-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cf5cf-110">Список объектов managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="cf5cf-110">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="cf5cf-111">Коллекция [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="cf5cf-111">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="cf5cf-112">Список свойств и связей объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="cf5cf-112">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="cf5cf-113">Получение объекта managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="cf5cf-113">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="cf5cf-114">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="cf5cf-114">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="cf5cf-115">Чтение свойств и связей объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="cf5cf-115">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="cf5cf-116">Действие targetApps</span><span class="sxs-lookup"><span data-stu-id="cf5cf-116">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="cf5cf-117">Нет</span><span class="sxs-lookup"><span data-stu-id="cf5cf-117">None</span></span>|<span data-ttu-id="cf5cf-118">Н/Д</span><span class="sxs-lookup"><span data-stu-id="cf5cf-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="cf5cf-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="cf5cf-119">Properties</span></span>
|<span data-ttu-id="cf5cf-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="cf5cf-120">Property</span></span>|<span data-ttu-id="cf5cf-121">Тип</span><span class="sxs-lookup"><span data-stu-id="cf5cf-121">Type</span></span>|<span data-ttu-id="cf5cf-122">Описание</span><span class="sxs-lookup"><span data-stu-id="cf5cf-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf5cf-123">displayName</span><span class="sxs-lookup"><span data-stu-id="cf5cf-123">displayName</span></span>|<span data-ttu-id="cf5cf-124">Строка</span><span class="sxs-lookup"><span data-stu-id="cf5cf-124">String</span></span>|<span data-ttu-id="cf5cf-125">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="cf5cf-125">Policy display name.</span></span>|
|<span data-ttu-id="cf5cf-126">описание</span><span class="sxs-lookup"><span data-stu-id="cf5cf-126">description</span></span>|<span data-ttu-id="cf5cf-127">Строка</span><span class="sxs-lookup"><span data-stu-id="cf5cf-127">String</span></span>|<span data-ttu-id="cf5cf-128">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="cf5cf-128">The policy's description.</span></span>|
|<span data-ttu-id="cf5cf-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cf5cf-129">createdDateTime</span></span>|<span data-ttu-id="cf5cf-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf5cf-130">DateTimeOffset</span></span>|<span data-ttu-id="cf5cf-131">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="cf5cf-131">The date and time the policy was created.</span></span>|
|<span data-ttu-id="cf5cf-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cf5cf-132">lastModifiedDateTime</span></span>|<span data-ttu-id="cf5cf-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf5cf-133">DateTimeOffset</span></span>|<span data-ttu-id="cf5cf-134">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="cf5cf-134">Last time the policy was modified.</span></span>|
|<span data-ttu-id="cf5cf-135">id</span><span class="sxs-lookup"><span data-stu-id="cf5cf-135">id</span></span>|<span data-ttu-id="cf5cf-136">Строка</span><span class="sxs-lookup"><span data-stu-id="cf5cf-136">String</span></span>|<span data-ttu-id="cf5cf-137">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="cf5cf-137">Key of the entity.</span></span>|
|<span data-ttu-id="cf5cf-138">version</span><span class="sxs-lookup"><span data-stu-id="cf5cf-138">version</span></span>|<span data-ttu-id="cf5cf-139">Строка</span><span class="sxs-lookup"><span data-stu-id="cf5cf-139">String</span></span>|<span data-ttu-id="cf5cf-140">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="cf5cf-140">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cf5cf-141">Связи</span><span class="sxs-lookup"><span data-stu-id="cf5cf-141">Relationships</span></span>
<span data-ttu-id="cf5cf-142">Нет</span><span class="sxs-lookup"><span data-stu-id="cf5cf-142">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="cf5cf-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cf5cf-143">JSON Representation</span></span>
<span data-ttu-id="cf5cf-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cf5cf-144">Here is a JSON representation of the resource.</span></span>
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



