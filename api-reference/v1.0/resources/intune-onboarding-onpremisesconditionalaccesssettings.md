---
title: Тип ресурса onPremisesConditionalAccessSettings
description: Одноэлементный объект, представляющий параметры условного доступа к локальной среде Exchange для клиента.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 88d513cc59b9570b355e67fa417a9856519cf551
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875994"
---
# <a name="onpremisesconditionalaccesssettings-resource-type"></a><span data-ttu-id="859d3-103">Тип ресурса onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="859d3-103">onPremisesConditionalAccessSettings resource type</span></span>

> <span data-ttu-id="859d3-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="859d3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="859d3-105">Одноэлементный объект, представляющий параметры условного доступа к локальной среде Exchange для клиента.</span><span class="sxs-lookup"><span data-stu-id="859d3-105">Singleton entity which represents the Exchange OnPremises Conditional Access Settings for a tenant.</span></span>
## <a name="methods"></a><span data-ttu-id="859d3-106">Методы</span><span class="sxs-lookup"><span data-stu-id="859d3-106">Methods</span></span>
|<span data-ttu-id="859d3-107">Метод</span><span class="sxs-lookup"><span data-stu-id="859d3-107">Method</span></span>|<span data-ttu-id="859d3-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="859d3-108">Return Type</span></span>|<span data-ttu-id="859d3-109">Описание</span><span class="sxs-lookup"><span data-stu-id="859d3-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="859d3-110">Получение объекта onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="859d3-110">Get onPremisesConditionalAccessSettings</span></span>](../api/intune-onboarding-onpremisesconditionalaccesssettings-get.md)|[<span data-ttu-id="859d3-111">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="859d3-111">onPremisesConditionalAccessSettings</span></span>](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|<span data-ttu-id="859d3-112">Чтение свойств и связей объекта [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="859d3-112">Read properties and relationships of the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>|
|[<span data-ttu-id="859d3-113">Обновление объекта onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="859d3-113">Update onPremisesConditionalAccessSettings</span></span>](../api/intune-onboarding-onpremisesconditionalaccesssettings-update.md)|[<span data-ttu-id="859d3-114">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="859d3-114">onPremisesConditionalAccessSettings</span></span>](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|<span data-ttu-id="859d3-115">Обновление свойств объекта [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="859d3-115">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="859d3-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="859d3-116">Properties</span></span>
|<span data-ttu-id="859d3-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="859d3-117">Property</span></span>|<span data-ttu-id="859d3-118">Тип</span><span class="sxs-lookup"><span data-stu-id="859d3-118">Type</span></span>|<span data-ttu-id="859d3-119">Описание</span><span class="sxs-lookup"><span data-stu-id="859d3-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="859d3-120">id</span><span class="sxs-lookup"><span data-stu-id="859d3-120">id</span></span>|<span data-ttu-id="859d3-121">Строка</span><span class="sxs-lookup"><span data-stu-id="859d3-121">String</span></span>|<span data-ttu-id="859d3-122">Н/Д</span><span class="sxs-lookup"><span data-stu-id="859d3-122">Not yet documented</span></span>|
|<span data-ttu-id="859d3-123">enabled</span><span class="sxs-lookup"><span data-stu-id="859d3-123">enabled</span></span>|<span data-ttu-id="859d3-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="859d3-124">Boolean</span></span>|<span data-ttu-id="859d3-125">Указывает, включен ли в этой организации условный доступ к локальной среде</span><span class="sxs-lookup"><span data-stu-id="859d3-125">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="859d3-126">includedGroups</span><span class="sxs-lookup"><span data-stu-id="859d3-126">includedGroups</span></span>|<span data-ttu-id="859d3-127">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="859d3-127">Guid collection</span></span>|<span data-ttu-id="859d3-128">Группы пользователей, для которых включается условный доступ к локальной среде.</span><span class="sxs-lookup"><span data-stu-id="859d3-128">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="859d3-129">У всех пользователей в этих группах должны быть управляемые мобильные устройства, соответствующие требованиям для доступа к почте.</span><span class="sxs-lookup"><span data-stu-id="859d3-129">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="859d3-130">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="859d3-130">excludedGroups</span></span>|<span data-ttu-id="859d3-131">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="859d3-131">Guid collection</span></span>|<span data-ttu-id="859d3-132">Группы пользователей, на которые не распространяется условный доступ к локальной среде.</span><span class="sxs-lookup"><span data-stu-id="859d3-132">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="859d3-133">На всех пользователей из этих группах не будет распространяться политика условного доступа.</span><span class="sxs-lookup"><span data-stu-id="859d3-133">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="859d3-134">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="859d3-134">overrideDefaultRule</span></span>|<span data-ttu-id="859d3-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="859d3-135">Boolean</span></span>|<span data-ttu-id="859d3-136">Указывает, следует ли переопределять правило доступа по умолчанию при разрешении устройства, чтобы обеспечить предоставление доступа.</span><span class="sxs-lookup"><span data-stu-id="859d3-136">Override the default access rule when allowing a device to ensure access is granted.</span></span>|

## <a name="relationships"></a><span data-ttu-id="859d3-137">Связи</span><span class="sxs-lookup"><span data-stu-id="859d3-137">Relationships</span></span>
<span data-ttu-id="859d3-138">Нет</span><span class="sxs-lookup"><span data-stu-id="859d3-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="859d3-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="859d3-139">JSON Representation</span></span>
<span data-ttu-id="859d3-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="859d3-140">Here is a JSON representation of the resource.</span></span>
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



