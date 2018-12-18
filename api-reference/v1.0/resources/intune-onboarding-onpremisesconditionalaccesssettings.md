---
title: Тип ресурса onPremisesConditionalAccessSettings
description: Одноэлементный объект, представляющий параметры условного доступа к локальной среде Exchange для клиента.
author: tfitzmac
ms.openlocfilehash: 534d76b00246763c6dec49149920a1f296148596
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353930"
---
# <a name="onpremisesconditionalaccesssettings-resource-type"></a><span data-ttu-id="2f072-103">Тип ресурса onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="2f072-103">onPremisesConditionalAccessSettings resource type</span></span>

> <span data-ttu-id="2f072-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2f072-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2f072-105">Одноэлементный объект, представляющий параметры условного доступа к локальной среде Exchange для клиента.</span><span class="sxs-lookup"><span data-stu-id="2f072-105">Singleton entity which represents the Exchange OnPremises Conditional Access Settings for a tenant.</span></span>
## <a name="methods"></a><span data-ttu-id="2f072-106">Методы</span><span class="sxs-lookup"><span data-stu-id="2f072-106">Methods</span></span>
|<span data-ttu-id="2f072-107">Метод</span><span class="sxs-lookup"><span data-stu-id="2f072-107">Method</span></span>|<span data-ttu-id="2f072-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2f072-108">Return Type</span></span>|<span data-ttu-id="2f072-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2f072-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2f072-110">Получение объекта onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="2f072-110">Get onPremisesConditionalAccessSettings</span></span>](../api/intune-onboarding-onpremisesconditionalaccesssettings-get.md)|[<span data-ttu-id="2f072-111">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="2f072-111">onPremisesConditionalAccessSettings</span></span>](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|<span data-ttu-id="2f072-112">Чтение свойств и связей объекта [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="2f072-112">Read properties and relationships of the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>|
|[<span data-ttu-id="2f072-113">Обновление объекта onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="2f072-113">Update onPremisesConditionalAccessSettings</span></span>](../api/intune-onboarding-onpremisesconditionalaccesssettings-update.md)|[<span data-ttu-id="2f072-114">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="2f072-114">onPremisesConditionalAccessSettings</span></span>](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|<span data-ttu-id="2f072-115">Обновление свойств объекта [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="2f072-115">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2f072-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="2f072-116">Properties</span></span>
|<span data-ttu-id="2f072-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="2f072-117">Property</span></span>|<span data-ttu-id="2f072-118">Тип</span><span class="sxs-lookup"><span data-stu-id="2f072-118">Type</span></span>|<span data-ttu-id="2f072-119">Описание</span><span class="sxs-lookup"><span data-stu-id="2f072-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f072-120">id</span><span class="sxs-lookup"><span data-stu-id="2f072-120">id</span></span>|<span data-ttu-id="2f072-121">Строка</span><span class="sxs-lookup"><span data-stu-id="2f072-121">String</span></span>|<span data-ttu-id="2f072-122">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2f072-122">Not yet documented</span></span>|
|<span data-ttu-id="2f072-123">enabled</span><span class="sxs-lookup"><span data-stu-id="2f072-123">enabled</span></span>|<span data-ttu-id="2f072-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f072-124">Boolean</span></span>|<span data-ttu-id="2f072-125">Указывает, включен ли в этой организации условный доступ к локальной среде</span><span class="sxs-lookup"><span data-stu-id="2f072-125">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="2f072-126">includedGroups</span><span class="sxs-lookup"><span data-stu-id="2f072-126">includedGroups</span></span>|<span data-ttu-id="2f072-127">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="2f072-127">Guid collection</span></span>|<span data-ttu-id="2f072-128">Группы пользователей, для которых включается условный доступ к локальной среде.</span><span class="sxs-lookup"><span data-stu-id="2f072-128">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="2f072-129">У всех пользователей в этих группах должны быть управляемые мобильные устройства, соответствующие требованиям для доступа к почте.</span><span class="sxs-lookup"><span data-stu-id="2f072-129">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="2f072-130">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="2f072-130">excludedGroups</span></span>|<span data-ttu-id="2f072-131">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="2f072-131">Guid collection</span></span>|<span data-ttu-id="2f072-132">Группы пользователей, на которые не распространяется условный доступ к локальной среде.</span><span class="sxs-lookup"><span data-stu-id="2f072-132">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="2f072-133">На всех пользователей из этих группах не будет распространяться политика условного доступа.</span><span class="sxs-lookup"><span data-stu-id="2f072-133">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="2f072-134">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="2f072-134">overrideDefaultRule</span></span>|<span data-ttu-id="2f072-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f072-135">Boolean</span></span>|<span data-ttu-id="2f072-136">Указывает, следует ли переопределять правило доступа по умолчанию при разрешении устройства, чтобы обеспечить предоставление доступа.</span><span class="sxs-lookup"><span data-stu-id="2f072-136">Override the default access rule when allowing a device to ensure access is granted.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2f072-137">Связи</span><span class="sxs-lookup"><span data-stu-id="2f072-137">Relationships</span></span>
<span data-ttu-id="2f072-138">Нет</span><span class="sxs-lookup"><span data-stu-id="2f072-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2f072-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2f072-139">JSON Representation</span></span>
<span data-ttu-id="2f072-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2f072-140">Here is a JSON representation of the resource.</span></span>
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



