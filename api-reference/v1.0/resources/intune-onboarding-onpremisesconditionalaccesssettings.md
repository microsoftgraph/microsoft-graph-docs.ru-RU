---
title: Тип ресурса onPremisesConditionalAccessSettings
description: Одноэлементный объект, представляющий параметры условного доступа к локальной среде Exchange для клиента.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f307b137a39323e5e3c6b644602b1c0df3ab5512
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262281"
---
# <a name="onpremisesconditionalaccesssettings-resource-type"></a><span data-ttu-id="8f014-103">Тип ресурса onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="8f014-103">onPremisesConditionalAccessSettings resource type</span></span>

> <span data-ttu-id="8f014-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8f014-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f014-105">Одноэлементный объект, представляющий параметры условного доступа к локальной среде Exchange для клиента.</span><span class="sxs-lookup"><span data-stu-id="8f014-105">Singleton entity which represents the Exchange OnPremises Conditional Access Settings for a tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="8f014-106">Методы</span><span class="sxs-lookup"><span data-stu-id="8f014-106">Methods</span></span>
|<span data-ttu-id="8f014-107">Метод</span><span class="sxs-lookup"><span data-stu-id="8f014-107">Method</span></span>|<span data-ttu-id="8f014-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8f014-108">Return Type</span></span>|<span data-ttu-id="8f014-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8f014-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8f014-110">Получение объекта onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="8f014-110">Get onPremisesConditionalAccessSettings</span></span>](../api/intune-onboarding-onpremisesconditionalaccesssettings-get.md)|<span data-ttu-id="8f014-111">[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md);</span><span class="sxs-lookup"><span data-stu-id="8f014-111">[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)</span></span>|<span data-ttu-id="8f014-112">Чтение свойств и связей объекта [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="8f014-112">Read properties and relationships of the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>|
|[<span data-ttu-id="8f014-113">Обновление объекта onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="8f014-113">Update onPremisesConditionalAccessSettings</span></span>](../api/intune-onboarding-onpremisesconditionalaccesssettings-update.md)|[<span data-ttu-id="8f014-114">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="8f014-114">onPremisesConditionalAccessSettings</span></span>](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|<span data-ttu-id="8f014-115">Обновление свойств объекта [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="8f014-115">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8f014-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="8f014-116">Properties</span></span>
|<span data-ttu-id="8f014-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="8f014-117">Property</span></span>|<span data-ttu-id="8f014-118">Тип</span><span class="sxs-lookup"><span data-stu-id="8f014-118">Type</span></span>|<span data-ttu-id="8f014-119">Описание</span><span class="sxs-lookup"><span data-stu-id="8f014-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f014-120">id</span><span class="sxs-lookup"><span data-stu-id="8f014-120">id</span></span>|<span data-ttu-id="8f014-121">String</span><span class="sxs-lookup"><span data-stu-id="8f014-121">String</span></span>|<span data-ttu-id="8f014-122">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8f014-122">Not yet documented</span></span>|
|<span data-ttu-id="8f014-123">enabled</span><span class="sxs-lookup"><span data-stu-id="8f014-123">enabled</span></span>|<span data-ttu-id="8f014-124">Логический</span><span class="sxs-lookup"><span data-stu-id="8f014-124">Boolean</span></span>|<span data-ttu-id="8f014-125">Указывает, включен ли в этой организации условный доступ к локальной среде</span><span class="sxs-lookup"><span data-stu-id="8f014-125">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="8f014-126">includedGroups</span><span class="sxs-lookup"><span data-stu-id="8f014-126">includedGroups</span></span>|<span data-ttu-id="8f014-127">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="8f014-127">Guid collection</span></span>|<span data-ttu-id="8f014-128">Группы пользователей, для которых включается условный доступ к локальной среде.</span><span class="sxs-lookup"><span data-stu-id="8f014-128">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="8f014-129">У всех пользователей в этих группах должны быть управляемые мобильные устройства, соответствующие требованиям для доступа к почте.</span><span class="sxs-lookup"><span data-stu-id="8f014-129">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="8f014-130">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="8f014-130">excludedGroups</span></span>|<span data-ttu-id="8f014-131">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="8f014-131">Guid collection</span></span>|<span data-ttu-id="8f014-132">Группы пользователей, на которые не распространяется условный доступ к локальной среде.</span><span class="sxs-lookup"><span data-stu-id="8f014-132">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="8f014-133">На всех пользователей из этих группах не будет распространяться политика условного доступа.</span><span class="sxs-lookup"><span data-stu-id="8f014-133">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="8f014-134">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="8f014-134">overrideDefaultRule</span></span>|<span data-ttu-id="8f014-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f014-135">Boolean</span></span>|<span data-ttu-id="8f014-136">Указывает, следует ли переопределять правило доступа по умолчанию при разрешении устройства, чтобы обеспечить предоставление доступа.</span><span class="sxs-lookup"><span data-stu-id="8f014-136">Override the default access rule when allowing a device to ensure access is granted.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8f014-137">Связи</span><span class="sxs-lookup"><span data-stu-id="8f014-137">Relationships</span></span>
<span data-ttu-id="8f014-138">Нет</span><span class="sxs-lookup"><span data-stu-id="8f014-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8f014-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8f014-139">JSON Representation</span></span>
<span data-ttu-id="8f014-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8f014-140">Here is a JSON representation of the resource.</span></span>
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



