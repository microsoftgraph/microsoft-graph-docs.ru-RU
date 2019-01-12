---
title: Тип ресурса managedAppPolicy
description: Ресурс ManagedAppPolicy представляет базовый тип политик для определенных платформ.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5054566f0ee80940165ba19f8f0da197b5e4f3c0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981107"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="2ba12-103">Тип ресурса managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="2ba12-103">managedAppPolicy resource type</span></span>

> <span data-ttu-id="2ba12-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2ba12-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2ba12-105">Ресурс ManagedAppPolicy представляет базовый тип политик для определенных платформ.</span><span class="sxs-lookup"><span data-stu-id="2ba12-105">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>
## <a name="methods"></a><span data-ttu-id="2ba12-106">Методы</span><span class="sxs-lookup"><span data-stu-id="2ba12-106">Methods</span></span>
|<span data-ttu-id="2ba12-107">Метод</span><span class="sxs-lookup"><span data-stu-id="2ba12-107">Method</span></span>|<span data-ttu-id="2ba12-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2ba12-108">Return Type</span></span>|<span data-ttu-id="2ba12-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2ba12-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2ba12-110">Список объектов managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="2ba12-110">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="2ba12-111">Коллекция [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2ba12-111">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="2ba12-112">Список свойств и связей объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2ba12-112">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="2ba12-113">Получение объекта managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="2ba12-113">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="2ba12-114">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="2ba12-114">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="2ba12-115">Чтение свойств и связей объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2ba12-115">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="2ba12-116">Действие targetApps</span><span class="sxs-lookup"><span data-stu-id="2ba12-116">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="2ba12-117">Нет</span><span class="sxs-lookup"><span data-stu-id="2ba12-117">None</span></span>|<span data-ttu-id="2ba12-118">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2ba12-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="2ba12-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="2ba12-119">Properties</span></span>
|<span data-ttu-id="2ba12-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="2ba12-120">Property</span></span>|<span data-ttu-id="2ba12-121">Тип</span><span class="sxs-lookup"><span data-stu-id="2ba12-121">Type</span></span>|<span data-ttu-id="2ba12-122">Описание</span><span class="sxs-lookup"><span data-stu-id="2ba12-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ba12-123">displayName</span><span class="sxs-lookup"><span data-stu-id="2ba12-123">displayName</span></span>|<span data-ttu-id="2ba12-124">Строка</span><span class="sxs-lookup"><span data-stu-id="2ba12-124">String</span></span>|<span data-ttu-id="2ba12-125">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="2ba12-125">Policy display name.</span></span>|
|<span data-ttu-id="2ba12-126">описание</span><span class="sxs-lookup"><span data-stu-id="2ba12-126">description</span></span>|<span data-ttu-id="2ba12-127">Строка</span><span class="sxs-lookup"><span data-stu-id="2ba12-127">String</span></span>|<span data-ttu-id="2ba12-128">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="2ba12-128">The policy's description.</span></span>|
|<span data-ttu-id="2ba12-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2ba12-129">createdDateTime</span></span>|<span data-ttu-id="2ba12-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ba12-130">DateTimeOffset</span></span>|<span data-ttu-id="2ba12-131">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="2ba12-131">The date and time the policy was created.</span></span>|
|<span data-ttu-id="2ba12-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2ba12-132">lastModifiedDateTime</span></span>|<span data-ttu-id="2ba12-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ba12-133">DateTimeOffset</span></span>|<span data-ttu-id="2ba12-134">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="2ba12-134">Last time the policy was modified.</span></span>|
|<span data-ttu-id="2ba12-135">id</span><span class="sxs-lookup"><span data-stu-id="2ba12-135">id</span></span>|<span data-ttu-id="2ba12-136">Строка</span><span class="sxs-lookup"><span data-stu-id="2ba12-136">String</span></span>|<span data-ttu-id="2ba12-137">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2ba12-137">Key of the entity.</span></span>|
|<span data-ttu-id="2ba12-138">version</span><span class="sxs-lookup"><span data-stu-id="2ba12-138">version</span></span>|<span data-ttu-id="2ba12-139">Строка</span><span class="sxs-lookup"><span data-stu-id="2ba12-139">String</span></span>|<span data-ttu-id="2ba12-140">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="2ba12-140">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ba12-141">Связи</span><span class="sxs-lookup"><span data-stu-id="2ba12-141">Relationships</span></span>
<span data-ttu-id="2ba12-142">Нет</span><span class="sxs-lookup"><span data-stu-id="2ba12-142">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2ba12-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2ba12-143">JSON Representation</span></span>
<span data-ttu-id="2ba12-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2ba12-144">Here is a JSON representation of the resource.</span></span>
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



