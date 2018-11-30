---
title: Тип ресурса managedAppPolicy
description: Ресурс ManagedAppPolicy представляет базовый тип политик для определенных платформ.
ms.openlocfilehash: 0cd886e594e58dec3486af6d447969f1610c84fe
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027059"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="97c4c-103">Тип ресурса managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="97c4c-103">managedAppPolicy resource type</span></span>

> <span data-ttu-id="97c4c-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="97c4c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="97c4c-105">Ресурс ManagedAppPolicy представляет базовый тип политик для определенных платформ.</span><span class="sxs-lookup"><span data-stu-id="97c4c-105">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>
## <a name="methods"></a><span data-ttu-id="97c4c-106">Методы</span><span class="sxs-lookup"><span data-stu-id="97c4c-106">Methods</span></span>
|<span data-ttu-id="97c4c-107">Метод</span><span class="sxs-lookup"><span data-stu-id="97c4c-107">Method</span></span>|<span data-ttu-id="97c4c-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="97c4c-108">Return Type</span></span>|<span data-ttu-id="97c4c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="97c4c-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="97c4c-110">Список объектов managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="97c4c-110">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="97c4c-111">Коллекция [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="97c4c-111">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="97c4c-112">Список свойств и связей объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="97c4c-112">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="97c4c-113">Получение объекта managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="97c4c-113">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="97c4c-114">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="97c4c-114">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="97c4c-115">Чтение свойств и связей объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="97c4c-115">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="97c4c-116">Действие targetApps</span><span class="sxs-lookup"><span data-stu-id="97c4c-116">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="97c4c-117">Нет</span><span class="sxs-lookup"><span data-stu-id="97c4c-117">None</span></span>|<span data-ttu-id="97c4c-118">Н/Д</span><span class="sxs-lookup"><span data-stu-id="97c4c-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="97c4c-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="97c4c-119">Properties</span></span>
|<span data-ttu-id="97c4c-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="97c4c-120">Property</span></span>|<span data-ttu-id="97c4c-121">Тип</span><span class="sxs-lookup"><span data-stu-id="97c4c-121">Type</span></span>|<span data-ttu-id="97c4c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="97c4c-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97c4c-123">displayName</span><span class="sxs-lookup"><span data-stu-id="97c4c-123">displayName</span></span>|<span data-ttu-id="97c4c-124">String</span><span class="sxs-lookup"><span data-stu-id="97c4c-124">String</span></span>|<span data-ttu-id="97c4c-125">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="97c4c-125">Policy display name.</span></span>|
|<span data-ttu-id="97c4c-126">описание</span><span class="sxs-lookup"><span data-stu-id="97c4c-126">description</span></span>|<span data-ttu-id="97c4c-127">String</span><span class="sxs-lookup"><span data-stu-id="97c4c-127">String</span></span>|<span data-ttu-id="97c4c-128">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="97c4c-128">The policy's description.</span></span>|
|<span data-ttu-id="97c4c-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="97c4c-129">createdDateTime</span></span>|<span data-ttu-id="97c4c-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97c4c-130">DateTimeOffset</span></span>|<span data-ttu-id="97c4c-131">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="97c4c-131">The date and time the policy was created.</span></span>|
|<span data-ttu-id="97c4c-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="97c4c-132">lastModifiedDateTime</span></span>|<span data-ttu-id="97c4c-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97c4c-133">DateTimeOffset</span></span>|<span data-ttu-id="97c4c-134">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="97c4c-134">Last time the policy was modified.</span></span>|
|<span data-ttu-id="97c4c-135">id</span><span class="sxs-lookup"><span data-stu-id="97c4c-135">id</span></span>|<span data-ttu-id="97c4c-136">String</span><span class="sxs-lookup"><span data-stu-id="97c4c-136">String</span></span>|<span data-ttu-id="97c4c-137">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="97c4c-137">Key of the entity.</span></span>|
|<span data-ttu-id="97c4c-138">version</span><span class="sxs-lookup"><span data-stu-id="97c4c-138">version</span></span>|<span data-ttu-id="97c4c-139">String</span><span class="sxs-lookup"><span data-stu-id="97c4c-139">String</span></span>|<span data-ttu-id="97c4c-140">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="97c4c-140">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="97c4c-141">Связи</span><span class="sxs-lookup"><span data-stu-id="97c4c-141">Relationships</span></span>
<span data-ttu-id="97c4c-142">Нет</span><span class="sxs-lookup"><span data-stu-id="97c4c-142">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="97c4c-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="97c4c-143">JSON Representation</span></span>
<span data-ttu-id="97c4c-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="97c4c-144">Here is a JSON representation of the resource.</span></span>
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



