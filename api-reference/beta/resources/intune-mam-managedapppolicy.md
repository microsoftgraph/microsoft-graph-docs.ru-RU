---
title: Тип ресурса managedAppPolicy
description: Ресурс ManagedAppPolicy представляет базовый тип политик для определенных платформ.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3cea81d492e708c1d21039c6286fe01e70a590b4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840735"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="5c323-103">Тип ресурса managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="5c323-103">managedAppPolicy resource type</span></span>

> <span data-ttu-id="5c323-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5c323-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5c323-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c323-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5c323-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5c323-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5c323-107">Ресурс ManagedAppPolicy представляет базовый тип политик для определенных платформ.</span><span class="sxs-lookup"><span data-stu-id="5c323-107">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>
## <a name="methods"></a><span data-ttu-id="5c323-108">Методы</span><span class="sxs-lookup"><span data-stu-id="5c323-108">Methods</span></span>
|<span data-ttu-id="5c323-109">Метод</span><span class="sxs-lookup"><span data-stu-id="5c323-109">Method</span></span>|<span data-ttu-id="5c323-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5c323-110">Return Type</span></span>|<span data-ttu-id="5c323-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5c323-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5c323-112">Список объектов managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="5c323-112">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="5c323-113">Коллекция [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5c323-113">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="5c323-114">Список свойств и связей объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5c323-114">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="5c323-115">Получение объекта managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="5c323-115">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="5c323-116">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="5c323-116">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="5c323-117">Чтение свойств и связей объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="5c323-117">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="5c323-118">Действие targetApps</span><span class="sxs-lookup"><span data-stu-id="5c323-118">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="5c323-119">Нет</span><span class="sxs-lookup"><span data-stu-id="5c323-119">None</span></span>|<span data-ttu-id="5c323-120">Н/Д</span><span class="sxs-lookup"><span data-stu-id="5c323-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="5c323-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="5c323-121">Properties</span></span>
|<span data-ttu-id="5c323-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="5c323-122">Property</span></span>|<span data-ttu-id="5c323-123">Тип</span><span class="sxs-lookup"><span data-stu-id="5c323-123">Type</span></span>|<span data-ttu-id="5c323-124">Описание</span><span class="sxs-lookup"><span data-stu-id="5c323-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c323-125">displayName</span><span class="sxs-lookup"><span data-stu-id="5c323-125">displayName</span></span>|<span data-ttu-id="5c323-126">Строка</span><span class="sxs-lookup"><span data-stu-id="5c323-126">String</span></span>|<span data-ttu-id="5c323-127">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="5c323-127">Policy display name.</span></span>|
|<span data-ttu-id="5c323-128">описание</span><span class="sxs-lookup"><span data-stu-id="5c323-128">description</span></span>|<span data-ttu-id="5c323-129">Строка</span><span class="sxs-lookup"><span data-stu-id="5c323-129">String</span></span>|<span data-ttu-id="5c323-130">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="5c323-130">The policy's description.</span></span>|
|<span data-ttu-id="5c323-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5c323-131">createdDateTime</span></span>|<span data-ttu-id="5c323-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c323-132">DateTimeOffset</span></span>|<span data-ttu-id="5c323-133">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="5c323-133">The date and time the policy was created.</span></span>|
|<span data-ttu-id="5c323-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5c323-134">lastModifiedDateTime</span></span>|<span data-ttu-id="5c323-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c323-135">DateTimeOffset</span></span>|<span data-ttu-id="5c323-136">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="5c323-136">Last time the policy was modified.</span></span>|
|<span data-ttu-id="5c323-137">id</span><span class="sxs-lookup"><span data-stu-id="5c323-137">id</span></span>|<span data-ttu-id="5c323-138">Строка</span><span class="sxs-lookup"><span data-stu-id="5c323-138">String</span></span>|<span data-ttu-id="5c323-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5c323-139">Key of the entity.</span></span>|
|<span data-ttu-id="5c323-140">version</span><span class="sxs-lookup"><span data-stu-id="5c323-140">version</span></span>|<span data-ttu-id="5c323-141">Строка</span><span class="sxs-lookup"><span data-stu-id="5c323-141">String</span></span>|<span data-ttu-id="5c323-142">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="5c323-142">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5c323-143">Связи</span><span class="sxs-lookup"><span data-stu-id="5c323-143">Relationships</span></span>
<span data-ttu-id="5c323-144">Нет</span><span class="sxs-lookup"><span data-stu-id="5c323-144">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5c323-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5c323-145">JSON Representation</span></span>
<span data-ttu-id="5c323-146">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5c323-146">Here is a JSON representation of the resource.</span></span>
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





