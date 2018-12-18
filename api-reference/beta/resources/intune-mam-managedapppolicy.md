---
title: Тип ресурса managedAppPolicy
description: Ресурс ManagedAppPolicy представляет базовый тип политик для определенных платформ.
author: tfitzmac
ms.openlocfilehash: d971f99c4f081d5b40179d406f6a50acf5812e4f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27313463"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="dacf8-103">Тип ресурса managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="dacf8-103">managedAppPolicy resource type</span></span>

> <span data-ttu-id="dacf8-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="dacf8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dacf8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dacf8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dacf8-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="dacf8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dacf8-107">Ресурс ManagedAppPolicy представляет базовый тип политик для определенных платформ.</span><span class="sxs-lookup"><span data-stu-id="dacf8-107">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>
## <a name="methods"></a><span data-ttu-id="dacf8-108">Методы</span><span class="sxs-lookup"><span data-stu-id="dacf8-108">Methods</span></span>
|<span data-ttu-id="dacf8-109">Метод</span><span class="sxs-lookup"><span data-stu-id="dacf8-109">Method</span></span>|<span data-ttu-id="dacf8-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="dacf8-110">Return Type</span></span>|<span data-ttu-id="dacf8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="dacf8-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="dacf8-112">Список объектов managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="dacf8-112">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="dacf8-113">Коллекция [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="dacf8-113">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="dacf8-114">Список свойств и связей объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dacf8-114">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="dacf8-115">Получение объекта managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="dacf8-115">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="dacf8-116">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="dacf8-116">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="dacf8-117">Чтение свойств и связей объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dacf8-117">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="dacf8-118">Действие targetApps</span><span class="sxs-lookup"><span data-stu-id="dacf8-118">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="dacf8-119">Нет</span><span class="sxs-lookup"><span data-stu-id="dacf8-119">None</span></span>|<span data-ttu-id="dacf8-120">Н/Д</span><span class="sxs-lookup"><span data-stu-id="dacf8-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="dacf8-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="dacf8-121">Properties</span></span>
|<span data-ttu-id="dacf8-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="dacf8-122">Property</span></span>|<span data-ttu-id="dacf8-123">Тип</span><span class="sxs-lookup"><span data-stu-id="dacf8-123">Type</span></span>|<span data-ttu-id="dacf8-124">Описание</span><span class="sxs-lookup"><span data-stu-id="dacf8-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dacf8-125">displayName</span><span class="sxs-lookup"><span data-stu-id="dacf8-125">displayName</span></span>|<span data-ttu-id="dacf8-126">Строка</span><span class="sxs-lookup"><span data-stu-id="dacf8-126">String</span></span>|<span data-ttu-id="dacf8-127">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="dacf8-127">Policy display name.</span></span>|
|<span data-ttu-id="dacf8-128">описание</span><span class="sxs-lookup"><span data-stu-id="dacf8-128">description</span></span>|<span data-ttu-id="dacf8-129">Строка</span><span class="sxs-lookup"><span data-stu-id="dacf8-129">String</span></span>|<span data-ttu-id="dacf8-130">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="dacf8-130">The policy's description.</span></span>|
|<span data-ttu-id="dacf8-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dacf8-131">createdDateTime</span></span>|<span data-ttu-id="dacf8-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dacf8-132">DateTimeOffset</span></span>|<span data-ttu-id="dacf8-133">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="dacf8-133">The date and time the policy was created.</span></span>|
|<span data-ttu-id="dacf8-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dacf8-134">lastModifiedDateTime</span></span>|<span data-ttu-id="dacf8-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dacf8-135">DateTimeOffset</span></span>|<span data-ttu-id="dacf8-136">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="dacf8-136">Last time the policy was modified.</span></span>|
|<span data-ttu-id="dacf8-137">id</span><span class="sxs-lookup"><span data-stu-id="dacf8-137">id</span></span>|<span data-ttu-id="dacf8-138">Строка</span><span class="sxs-lookup"><span data-stu-id="dacf8-138">String</span></span>|<span data-ttu-id="dacf8-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="dacf8-139">Key of the entity.</span></span>|
|<span data-ttu-id="dacf8-140">version</span><span class="sxs-lookup"><span data-stu-id="dacf8-140">version</span></span>|<span data-ttu-id="dacf8-141">Строка</span><span class="sxs-lookup"><span data-stu-id="dacf8-141">String</span></span>|<span data-ttu-id="dacf8-142">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="dacf8-142">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dacf8-143">Связи</span><span class="sxs-lookup"><span data-stu-id="dacf8-143">Relationships</span></span>
<span data-ttu-id="dacf8-144">Нет</span><span class="sxs-lookup"><span data-stu-id="dacf8-144">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="dacf8-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dacf8-145">JSON Representation</span></span>
<span data-ttu-id="dacf8-146">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dacf8-146">Here is a JSON representation of the resource.</span></span>
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





