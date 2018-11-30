---
title: Тип ресурса onPremisesConditionalAccessSettings
description: Одноэлементный объект, представляющий параметры условного доступа к локальной среде Exchange для клиента.
ms.openlocfilehash: 903a3e6a3fafd837fc8c5caf55eb57d23ddd0d2a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026470"
---
# <a name="onpremisesconditionalaccesssettings-resource-type"></a><span data-ttu-id="412e4-103">Тип ресурса onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="412e4-103">onPremisesConditionalAccessSettings resource type</span></span>

> <span data-ttu-id="412e4-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="412e4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="412e4-105">Одноэлементный объект, представляющий параметры условного доступа к локальной среде Exchange для клиента.</span><span class="sxs-lookup"><span data-stu-id="412e4-105">Singleton entity which represents the Exchange OnPremises Conditional Access Settings for a tenant.</span></span>
## <a name="methods"></a><span data-ttu-id="412e4-106">Методы</span><span class="sxs-lookup"><span data-stu-id="412e4-106">Methods</span></span>
|<span data-ttu-id="412e4-107">Метод</span><span class="sxs-lookup"><span data-stu-id="412e4-107">Method</span></span>|<span data-ttu-id="412e4-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="412e4-108">Return Type</span></span>|<span data-ttu-id="412e4-109">Описание</span><span class="sxs-lookup"><span data-stu-id="412e4-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="412e4-110">Получение объекта onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="412e4-110">Get onPremisesConditionalAccessSettings</span></span>](../api/intune-onboarding-onpremisesconditionalaccesssettings-get.md)|[<span data-ttu-id="412e4-111">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="412e4-111">onPremisesConditionalAccessSettings</span></span>](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|<span data-ttu-id="412e4-112">Чтение свойств и связей объекта [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="412e4-112">Read properties and relationships of the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>|
|[<span data-ttu-id="412e4-113">Обновление объекта onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="412e4-113">Update onPremisesConditionalAccessSettings</span></span>](../api/intune-onboarding-onpremisesconditionalaccesssettings-update.md)|[<span data-ttu-id="412e4-114">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="412e4-114">onPremisesConditionalAccessSettings</span></span>](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|<span data-ttu-id="412e4-115">Обновление свойств объекта [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="412e4-115">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="412e4-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="412e4-116">Properties</span></span>
|<span data-ttu-id="412e4-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="412e4-117">Property</span></span>|<span data-ttu-id="412e4-118">Тип</span><span class="sxs-lookup"><span data-stu-id="412e4-118">Type</span></span>|<span data-ttu-id="412e4-119">Описание</span><span class="sxs-lookup"><span data-stu-id="412e4-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="412e4-120">id</span><span class="sxs-lookup"><span data-stu-id="412e4-120">id</span></span>|<span data-ttu-id="412e4-121">String</span><span class="sxs-lookup"><span data-stu-id="412e4-121">String</span></span>|<span data-ttu-id="412e4-122">Н/Д</span><span class="sxs-lookup"><span data-stu-id="412e4-122">Not yet documented</span></span>|
|<span data-ttu-id="412e4-123">enabled</span><span class="sxs-lookup"><span data-stu-id="412e4-123">enabled</span></span>|<span data-ttu-id="412e4-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="412e4-124">Boolean</span></span>|<span data-ttu-id="412e4-125">Указывает, включен ли в этой организации условный доступ к локальной среде</span><span class="sxs-lookup"><span data-stu-id="412e4-125">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="412e4-126">includedGroups</span><span class="sxs-lookup"><span data-stu-id="412e4-126">includedGroups</span></span>|<span data-ttu-id="412e4-127">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="412e4-127">Guid collection</span></span>|<span data-ttu-id="412e4-128">Группы пользователей, для которых включается условный доступ к локальной среде.</span><span class="sxs-lookup"><span data-stu-id="412e4-128">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="412e4-129">У всех пользователей в этих группах должны быть управляемые мобильные устройства, соответствующие требованиям для доступа к почте.</span><span class="sxs-lookup"><span data-stu-id="412e4-129">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="412e4-130">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="412e4-130">excludedGroups</span></span>|<span data-ttu-id="412e4-131">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="412e4-131">Guid collection</span></span>|<span data-ttu-id="412e4-132">Группы пользователей, на которые не распространяется условный доступ к локальной среде.</span><span class="sxs-lookup"><span data-stu-id="412e4-132">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="412e4-133">На всех пользователей из этих группах не будет распространяться политика условного доступа.</span><span class="sxs-lookup"><span data-stu-id="412e4-133">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="412e4-134">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="412e4-134">overrideDefaultRule</span></span>|<span data-ttu-id="412e4-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="412e4-135">Boolean</span></span>|<span data-ttu-id="412e4-136">Указывает, следует ли переопределять правило доступа по умолчанию при разрешении устройства, чтобы обеспечить предоставление доступа.</span><span class="sxs-lookup"><span data-stu-id="412e4-136">Override the default access rule when allowing a device to ensure access is granted.</span></span>|

## <a name="relationships"></a><span data-ttu-id="412e4-137">Связи</span><span class="sxs-lookup"><span data-stu-id="412e4-137">Relationships</span></span>
<span data-ttu-id="412e4-138">Нет</span><span class="sxs-lookup"><span data-stu-id="412e4-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="412e4-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="412e4-139">JSON Representation</span></span>
<span data-ttu-id="412e4-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="412e4-140">Here is a JSON representation of the resource.</span></span>
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



