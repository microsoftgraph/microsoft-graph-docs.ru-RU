---
title: Тип ресурса onPremisesConditionalAccessSettings
description: Одноэлементный объект, представляющий параметры условного доступа к локальной среде Exchange для клиента.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 44e0174ce6b7c8918e100c345189f79050038f9b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43441767"
---
# <a name="onpremisesconditionalaccesssettings-resource-type"></a><span data-ttu-id="15649-103">Тип ресурса onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="15649-103">onPremisesConditionalAccessSettings resource type</span></span>

<span data-ttu-id="15649-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15649-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="15649-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="15649-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15649-106">Одноэлементный объект, представляющий параметры условного доступа к локальной среде Exchange для клиента.</span><span class="sxs-lookup"><span data-stu-id="15649-106">Singleton entity which represents the Exchange OnPremises Conditional Access Settings for a tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="15649-107">Методы</span><span class="sxs-lookup"><span data-stu-id="15649-107">Methods</span></span>
|<span data-ttu-id="15649-108">Метод</span><span class="sxs-lookup"><span data-stu-id="15649-108">Method</span></span>|<span data-ttu-id="15649-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="15649-109">Return Type</span></span>|<span data-ttu-id="15649-110">Описание</span><span class="sxs-lookup"><span data-stu-id="15649-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="15649-111">Получение объекта onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="15649-111">Get onPremisesConditionalAccessSettings</span></span>](../api/intune-onboarding-onpremisesconditionalaccesssettings-get.md)|<span data-ttu-id="15649-112">[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md);</span><span class="sxs-lookup"><span data-stu-id="15649-112">[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)</span></span>|<span data-ttu-id="15649-113">Чтение свойств и связей объекта [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="15649-113">Read properties and relationships of the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>|
|[<span data-ttu-id="15649-114">Обновление объекта onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="15649-114">Update onPremisesConditionalAccessSettings</span></span>](../api/intune-onboarding-onpremisesconditionalaccesssettings-update.md)|[<span data-ttu-id="15649-115">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="15649-115">onPremisesConditionalAccessSettings</span></span>](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|<span data-ttu-id="15649-116">Обновление свойств объекта [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="15649-116">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="15649-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="15649-117">Properties</span></span>
|<span data-ttu-id="15649-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="15649-118">Property</span></span>|<span data-ttu-id="15649-119">Тип</span><span class="sxs-lookup"><span data-stu-id="15649-119">Type</span></span>|<span data-ttu-id="15649-120">Описание</span><span class="sxs-lookup"><span data-stu-id="15649-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15649-121">id</span><span class="sxs-lookup"><span data-stu-id="15649-121">id</span></span>|<span data-ttu-id="15649-122">String</span><span class="sxs-lookup"><span data-stu-id="15649-122">String</span></span>|<span data-ttu-id="15649-123">Н/Д</span><span class="sxs-lookup"><span data-stu-id="15649-123">Not yet documented</span></span>|
|<span data-ttu-id="15649-124">enabled</span><span class="sxs-lookup"><span data-stu-id="15649-124">enabled</span></span>|<span data-ttu-id="15649-125">Логический</span><span class="sxs-lookup"><span data-stu-id="15649-125">Boolean</span></span>|<span data-ttu-id="15649-126">Указывает, включен ли в этой организации условный доступ к локальной среде</span><span class="sxs-lookup"><span data-stu-id="15649-126">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="15649-127">includedGroups</span><span class="sxs-lookup"><span data-stu-id="15649-127">includedGroups</span></span>|<span data-ttu-id="15649-128">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="15649-128">Guid collection</span></span>|<span data-ttu-id="15649-129">Группы пользователей, для которых включается условный доступ к локальной среде.</span><span class="sxs-lookup"><span data-stu-id="15649-129">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="15649-130">У всех пользователей в этих группах должны быть управляемые мобильные устройства, соответствующие требованиям для доступа к почте.</span><span class="sxs-lookup"><span data-stu-id="15649-130">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="15649-131">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="15649-131">excludedGroups</span></span>|<span data-ttu-id="15649-132">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="15649-132">Guid collection</span></span>|<span data-ttu-id="15649-133">Группы пользователей, на которые не распространяется условный доступ к локальной среде.</span><span class="sxs-lookup"><span data-stu-id="15649-133">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="15649-134">На всех пользователей из этих группах не будет распространяться политика условного доступа.</span><span class="sxs-lookup"><span data-stu-id="15649-134">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="15649-135">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="15649-135">overrideDefaultRule</span></span>|<span data-ttu-id="15649-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="15649-136">Boolean</span></span>|<span data-ttu-id="15649-137">Указывает, следует ли переопределять правило доступа по умолчанию при разрешении устройства, чтобы обеспечить предоставление доступа.</span><span class="sxs-lookup"><span data-stu-id="15649-137">Override the default access rule when allowing a device to ensure access is granted.</span></span>|

## <a name="relationships"></a><span data-ttu-id="15649-138">Отношения</span><span class="sxs-lookup"><span data-stu-id="15649-138">Relationships</span></span>
<span data-ttu-id="15649-139">Нет</span><span class="sxs-lookup"><span data-stu-id="15649-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="15649-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="15649-140">JSON Representation</span></span>
<span data-ttu-id="15649-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="15649-141">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.onPremisesConditionalAccessSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "id": "String (identifier)",
  "enabled": true,
  "includedGroups": [
    "Guid"
  ],
  "excludedGroups": [
    "Guid"
  ],
  "overrideDefaultRule": true
}
```







