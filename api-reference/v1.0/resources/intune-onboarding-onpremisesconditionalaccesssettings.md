---
title: Тип ресурса onPremisesConditionalAccessSettings
description: Одноэлементный объект, представляющий параметры условного доступа к локальной среде Exchange для клиента.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2fda9b2c4e8dff366fc347ea145ba627e6c764ff
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448041"
---
# <a name="onpremisesconditionalaccesssettings-resource-type"></a><span data-ttu-id="1c177-103">Тип ресурса onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="1c177-103">onPremisesConditionalAccessSettings resource type</span></span>

<span data-ttu-id="1c177-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1c177-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1c177-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1c177-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c177-106">Одноэлементный объект, представляющий параметры условного доступа к локальной среде Exchange для клиента.</span><span class="sxs-lookup"><span data-stu-id="1c177-106">Singleton entity which represents the Exchange OnPremises Conditional Access Settings for a tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="1c177-107">Методы</span><span class="sxs-lookup"><span data-stu-id="1c177-107">Methods</span></span>
|<span data-ttu-id="1c177-108">Метод</span><span class="sxs-lookup"><span data-stu-id="1c177-108">Method</span></span>|<span data-ttu-id="1c177-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1c177-109">Return Type</span></span>|<span data-ttu-id="1c177-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1c177-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1c177-111">Получение объекта onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="1c177-111">Get onPremisesConditionalAccessSettings</span></span>](../api/intune-onboarding-onpremisesconditionalaccesssettings-get.md)|<span data-ttu-id="1c177-112">[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md);</span><span class="sxs-lookup"><span data-stu-id="1c177-112">[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)</span></span>|<span data-ttu-id="1c177-113">Чтение свойств и связей объекта [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="1c177-113">Read properties and relationships of the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>|
|[<span data-ttu-id="1c177-114">Обновление объекта onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="1c177-114">Update onPremisesConditionalAccessSettings</span></span>](../api/intune-onboarding-onpremisesconditionalaccesssettings-update.md)|[<span data-ttu-id="1c177-115">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="1c177-115">onPremisesConditionalAccessSettings</span></span>](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|<span data-ttu-id="1c177-116">Обновление свойств объекта [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="1c177-116">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1c177-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="1c177-117">Properties</span></span>
|<span data-ttu-id="1c177-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="1c177-118">Property</span></span>|<span data-ttu-id="1c177-119">Тип</span><span class="sxs-lookup"><span data-stu-id="1c177-119">Type</span></span>|<span data-ttu-id="1c177-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1c177-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c177-121">id</span><span class="sxs-lookup"><span data-stu-id="1c177-121">id</span></span>|<span data-ttu-id="1c177-122">String</span><span class="sxs-lookup"><span data-stu-id="1c177-122">String</span></span>|<span data-ttu-id="1c177-123">Н/Д</span><span class="sxs-lookup"><span data-stu-id="1c177-123">Not yet documented</span></span>|
|<span data-ttu-id="1c177-124">enabled</span><span class="sxs-lookup"><span data-stu-id="1c177-124">enabled</span></span>|<span data-ttu-id="1c177-125">Логический</span><span class="sxs-lookup"><span data-stu-id="1c177-125">Boolean</span></span>|<span data-ttu-id="1c177-126">Указывает, включен ли в этой организации условный доступ к локальной среде</span><span class="sxs-lookup"><span data-stu-id="1c177-126">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="1c177-127">includedGroups</span><span class="sxs-lookup"><span data-stu-id="1c177-127">includedGroups</span></span>|<span data-ttu-id="1c177-128">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="1c177-128">Guid collection</span></span>|<span data-ttu-id="1c177-129">Группы пользователей, для которых включается условный доступ к локальной среде.</span><span class="sxs-lookup"><span data-stu-id="1c177-129">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="1c177-130">У всех пользователей в этих группах должны быть управляемые мобильные устройства, соответствующие требованиям для доступа к почте.</span><span class="sxs-lookup"><span data-stu-id="1c177-130">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="1c177-131">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="1c177-131">excludedGroups</span></span>|<span data-ttu-id="1c177-132">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="1c177-132">Guid collection</span></span>|<span data-ttu-id="1c177-133">Группы пользователей, на которые не распространяется условный доступ к локальной среде.</span><span class="sxs-lookup"><span data-stu-id="1c177-133">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="1c177-134">На всех пользователей из этих группах не будет распространяться политика условного доступа.</span><span class="sxs-lookup"><span data-stu-id="1c177-134">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="1c177-135">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="1c177-135">overrideDefaultRule</span></span>|<span data-ttu-id="1c177-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c177-136">Boolean</span></span>|<span data-ttu-id="1c177-137">Указывает, следует ли переопределять правило доступа по умолчанию при разрешении устройства, чтобы обеспечить предоставление доступа.</span><span class="sxs-lookup"><span data-stu-id="1c177-137">Override the default access rule when allowing a device to ensure access is granted.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1c177-138">Связи</span><span class="sxs-lookup"><span data-stu-id="1c177-138">Relationships</span></span>
<span data-ttu-id="1c177-139">Нет</span><span class="sxs-lookup"><span data-stu-id="1c177-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1c177-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1c177-140">JSON Representation</span></span>
<span data-ttu-id="1c177-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1c177-141">Here is a JSON representation of the resource.</span></span>
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




