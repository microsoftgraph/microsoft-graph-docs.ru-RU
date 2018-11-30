---
title: Тип ресурса managedAppPolicy
description: Ресурс ManagedAppPolicy представляет базовый тип политик для определенных платформ.
ms.openlocfilehash: ab87690e611effa239a8471612dbb201ea6b75b8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078858"
---
# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="67a23-103">Тип ресурса managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="67a23-103">managedAppPolicy resource type</span></span>

> <span data-ttu-id="67a23-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="67a23-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="67a23-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67a23-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="67a23-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="67a23-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="67a23-107">Ресурс ManagedAppPolicy представляет базовый тип политик для определенных платформ.</span><span class="sxs-lookup"><span data-stu-id="67a23-107">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>
## <a name="methods"></a><span data-ttu-id="67a23-108">Методы</span><span class="sxs-lookup"><span data-stu-id="67a23-108">Methods</span></span>
|<span data-ttu-id="67a23-109">Метод</span><span class="sxs-lookup"><span data-stu-id="67a23-109">Method</span></span>|<span data-ttu-id="67a23-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="67a23-110">Return Type</span></span>|<span data-ttu-id="67a23-111">Описание</span><span class="sxs-lookup"><span data-stu-id="67a23-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="67a23-112">Список объектов managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="67a23-112">List managedAppPolicies</span></span>](../api/intune-mam-managedapppolicy-list.md)|<span data-ttu-id="67a23-113">Коллекция [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="67a23-113">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="67a23-114">Список свойств и связей объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="67a23-114">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="67a23-115">Получение объекта managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="67a23-115">Get managedAppPolicy</span></span>](../api/intune-mam-managedapppolicy-get.md)|[<span data-ttu-id="67a23-116">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="67a23-116">managedAppPolicy</span></span>](../resources/intune-mam-managedapppolicy.md)|<span data-ttu-id="67a23-117">Чтение свойств и связей объекта [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="67a23-117">Read properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="67a23-118">Действие targetApps</span><span class="sxs-lookup"><span data-stu-id="67a23-118">targetApps action</span></span>](../api/intune-mam-managedapppolicy-targetapps.md)|<span data-ttu-id="67a23-119">Нет</span><span class="sxs-lookup"><span data-stu-id="67a23-119">None</span></span>|<span data-ttu-id="67a23-120">Н/Д</span><span class="sxs-lookup"><span data-stu-id="67a23-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="67a23-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="67a23-121">Properties</span></span>
|<span data-ttu-id="67a23-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="67a23-122">Property</span></span>|<span data-ttu-id="67a23-123">Тип</span><span class="sxs-lookup"><span data-stu-id="67a23-123">Type</span></span>|<span data-ttu-id="67a23-124">Описание</span><span class="sxs-lookup"><span data-stu-id="67a23-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67a23-125">displayName</span><span class="sxs-lookup"><span data-stu-id="67a23-125">displayName</span></span>|<span data-ttu-id="67a23-126">String</span><span class="sxs-lookup"><span data-stu-id="67a23-126">String</span></span>|<span data-ttu-id="67a23-127">Отображаемое имя политики.</span><span class="sxs-lookup"><span data-stu-id="67a23-127">Policy display name.</span></span>|
|<span data-ttu-id="67a23-128">описание</span><span class="sxs-lookup"><span data-stu-id="67a23-128">description</span></span>|<span data-ttu-id="67a23-129">String</span><span class="sxs-lookup"><span data-stu-id="67a23-129">String</span></span>|<span data-ttu-id="67a23-130">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="67a23-130">The policy's description.</span></span>|
|<span data-ttu-id="67a23-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="67a23-131">createdDateTime</span></span>|<span data-ttu-id="67a23-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67a23-132">DateTimeOffset</span></span>|<span data-ttu-id="67a23-133">Дата и время создания политики.</span><span class="sxs-lookup"><span data-stu-id="67a23-133">The date and time the policy was created.</span></span>|
|<span data-ttu-id="67a23-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="67a23-134">lastModifiedDateTime</span></span>|<span data-ttu-id="67a23-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67a23-135">DateTimeOffset</span></span>|<span data-ttu-id="67a23-136">Время последнего изменения политики.</span><span class="sxs-lookup"><span data-stu-id="67a23-136">Last time the policy was modified.</span></span>|
|<span data-ttu-id="67a23-137">id</span><span class="sxs-lookup"><span data-stu-id="67a23-137">id</span></span>|<span data-ttu-id="67a23-138">String</span><span class="sxs-lookup"><span data-stu-id="67a23-138">String</span></span>|<span data-ttu-id="67a23-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="67a23-139">Key of the entity.</span></span>|
|<span data-ttu-id="67a23-140">version</span><span class="sxs-lookup"><span data-stu-id="67a23-140">version</span></span>|<span data-ttu-id="67a23-141">String</span><span class="sxs-lookup"><span data-stu-id="67a23-141">String</span></span>|<span data-ttu-id="67a23-142">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="67a23-142">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="67a23-143">Связи</span><span class="sxs-lookup"><span data-stu-id="67a23-143">Relationships</span></span>
<span data-ttu-id="67a23-144">Нет</span><span class="sxs-lookup"><span data-stu-id="67a23-144">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="67a23-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="67a23-145">JSON Representation</span></span>
<span data-ttu-id="67a23-146">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="67a23-146">Here is a JSON representation of the resource.</span></span>
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





