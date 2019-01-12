---
title: Тип ресурса managedAppPolicy
description: Ресурс ManagedAppPolicy представляет базовый тип политик для определенных платформ.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 45a8365bb7a1ea97c156921cfbd923ba9b52dd1b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937504"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="ce7a8-103">Тип ресурса managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="ce7a8-103">managedAppPolicy resource type</span></span>

> <span data-ttu-id="ce7a8-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ce7a8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ce7a8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce7a8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ce7a8-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ce7a8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ce7a8-107">Ресурс ManagedAppPolicy представляет базовый тип политик для определенных платформ.</span><span class="sxs-lookup"><span data-stu-id="ce7a8-107">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>
## <a name="methods"></a><span data-ttu-id="ce7a8-108">Методы</span><span class="sxs-lookup"><span data-stu-id="ce7a8-108">Methods</span></span>
|<span data-ttu-id="ce7a8-109">Метод</span><span class="sxs-lookup"><span data-stu-id="ce7a8-109">Method</span></span>|<span data-ttu-id="ce7a8-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ce7a8-110">Return Type</span></span>|<span data-ttu-id="ce7a8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ce7a8-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ce7a8-112">Список объектов managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="ce7a8-112">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="ce7a8-113">Коллекция [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ce7a8-113">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="ce7a8-114">Список свойств и связей объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ce7a8-114">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="ce7a8-115">Получение объекта managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="ce7a8-115">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="ce7a8-116">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="ce7a8-116">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="ce7a8-117">Чтение свойств и связей объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ce7a8-117">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="ce7a8-118">Действие targetApps</span><span class="sxs-lookup"><span data-stu-id="ce7a8-118">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="ce7a8-119">Нет</span><span class="sxs-lookup"><span data-stu-id="ce7a8-119">None</span></span>|<span data-ttu-id="ce7a8-120">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ce7a8-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="ce7a8-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="ce7a8-121">Properties</span></span>
|<span data-ttu-id="ce7a8-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="ce7a8-122">Property</span></span>|<span data-ttu-id="ce7a8-123">Тип</span><span class="sxs-lookup"><span data-stu-id="ce7a8-123">Type</span></span>|<span data-ttu-id="ce7a8-124">Описание</span><span class="sxs-lookup"><span data-stu-id="ce7a8-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce7a8-125">displayName</span><span class="sxs-lookup"><span data-stu-id="ce7a8-125">displayName</span></span>|<span data-ttu-id="ce7a8-126">String</span><span class="sxs-lookup"><span data-stu-id="ce7a8-126">String</span></span>|<span data-ttu-id="ce7a8-127">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="ce7a8-127">Policy display name.</span></span>|
|<span data-ttu-id="ce7a8-128">описание</span><span class="sxs-lookup"><span data-stu-id="ce7a8-128">description</span></span>|<span data-ttu-id="ce7a8-129">String</span><span class="sxs-lookup"><span data-stu-id="ce7a8-129">String</span></span>|<span data-ttu-id="ce7a8-130">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="ce7a8-130">The policy's description.</span></span>|
|<span data-ttu-id="ce7a8-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ce7a8-131">createdDateTime</span></span>|<span data-ttu-id="ce7a8-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce7a8-132">DateTimeOffset</span></span>|<span data-ttu-id="ce7a8-133">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="ce7a8-133">The date and time the policy was created.</span></span>|
|<span data-ttu-id="ce7a8-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ce7a8-134">lastModifiedDateTime</span></span>|<span data-ttu-id="ce7a8-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce7a8-135">DateTimeOffset</span></span>|<span data-ttu-id="ce7a8-136">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="ce7a8-136">Last time the policy was modified.</span></span>|
|<span data-ttu-id="ce7a8-137">id</span><span class="sxs-lookup"><span data-stu-id="ce7a8-137">id</span></span>|<span data-ttu-id="ce7a8-138">String</span><span class="sxs-lookup"><span data-stu-id="ce7a8-138">String</span></span>|<span data-ttu-id="ce7a8-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ce7a8-139">Key of the entity.</span></span>|
|<span data-ttu-id="ce7a8-140">version</span><span class="sxs-lookup"><span data-stu-id="ce7a8-140">version</span></span>|<span data-ttu-id="ce7a8-141">String</span><span class="sxs-lookup"><span data-stu-id="ce7a8-141">String</span></span>|<span data-ttu-id="ce7a8-142">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="ce7a8-142">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ce7a8-143">Связи</span><span class="sxs-lookup"><span data-stu-id="ce7a8-143">Relationships</span></span>
<span data-ttu-id="ce7a8-144">Нет</span><span class="sxs-lookup"><span data-stu-id="ce7a8-144">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ce7a8-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ce7a8-145">JSON Representation</span></span>
<span data-ttu-id="ce7a8-146">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ce7a8-146">Here is a JSON representation of the resource.</span></span>
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





