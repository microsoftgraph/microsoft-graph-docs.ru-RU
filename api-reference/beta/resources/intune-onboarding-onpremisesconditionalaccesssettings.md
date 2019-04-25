---
title: Тип ресурса onPremisesConditionalAccessSettings
description: Одноэлементный объект, представляющий параметры условного доступа к локальной среде Exchange для клиента.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8fe4dd79722392ea5c0e5e6487c3c3dbc3587d4e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566454"
---
# <a name="onpremisesconditionalaccesssettings-resource-type"></a><span data-ttu-id="22914-103">Тип ресурса onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="22914-103">onPremisesConditionalAccessSettings resource type</span></span>

> <span data-ttu-id="22914-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22914-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22914-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="22914-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22914-106">Одноэлементный объект, представляющий параметры условного доступа к локальной среде Exchange для клиента.</span><span class="sxs-lookup"><span data-stu-id="22914-106">Singleton entity which represents the Exchange OnPremises Conditional Access Settings for a tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="22914-107">Методы</span><span class="sxs-lookup"><span data-stu-id="22914-107">Methods</span></span>
|<span data-ttu-id="22914-108">Метод</span><span class="sxs-lookup"><span data-stu-id="22914-108">Method</span></span>|<span data-ttu-id="22914-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="22914-109">Return Type</span></span>|<span data-ttu-id="22914-110">Описание</span><span class="sxs-lookup"><span data-stu-id="22914-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="22914-111">Получение объекта onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="22914-111">Get onPremisesConditionalAccessSettings</span></span>](../api/intune-onboarding-onpremisesconditionalaccesssettings-get.md)|<span data-ttu-id="22914-112">[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md);</span><span class="sxs-lookup"><span data-stu-id="22914-112">[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)</span></span>|<span data-ttu-id="22914-113">Чтение свойств и связей объекта [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="22914-113">Read properties and relationships of the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>|
|[<span data-ttu-id="22914-114">Обновление объекта onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="22914-114">Update onPremisesConditionalAccessSettings</span></span>](../api/intune-onboarding-onpremisesconditionalaccesssettings-update.md)|[<span data-ttu-id="22914-115">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="22914-115">onPremisesConditionalAccessSettings</span></span>](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|<span data-ttu-id="22914-116">Обновление свойств объекта [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="22914-116">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="22914-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="22914-117">Properties</span></span>
|<span data-ttu-id="22914-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="22914-118">Property</span></span>|<span data-ttu-id="22914-119">Тип</span><span class="sxs-lookup"><span data-stu-id="22914-119">Type</span></span>|<span data-ttu-id="22914-120">Описание</span><span class="sxs-lookup"><span data-stu-id="22914-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22914-121">id</span><span class="sxs-lookup"><span data-stu-id="22914-121">id</span></span>|<span data-ttu-id="22914-122">String</span><span class="sxs-lookup"><span data-stu-id="22914-122">String</span></span>|<span data-ttu-id="22914-123">Н/Д</span><span class="sxs-lookup"><span data-stu-id="22914-123">Not yet documented</span></span>|
|<span data-ttu-id="22914-124">enabled</span><span class="sxs-lookup"><span data-stu-id="22914-124">enabled</span></span>|<span data-ttu-id="22914-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="22914-125">Boolean</span></span>|<span data-ttu-id="22914-126">Указывает, включен ли в этой организации условный доступ к локальной среде</span><span class="sxs-lookup"><span data-stu-id="22914-126">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="22914-127">includedGroups</span><span class="sxs-lookup"><span data-stu-id="22914-127">includedGroups</span></span>|<span data-ttu-id="22914-128">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="22914-128">Guid collection</span></span>|<span data-ttu-id="22914-129">Группы пользователей, для которых включается условный доступ к локальной среде.</span><span class="sxs-lookup"><span data-stu-id="22914-129">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="22914-130">У всех пользователей в этих группах должны быть управляемые мобильные устройства, соответствующие требованиям для доступа к почте.</span><span class="sxs-lookup"><span data-stu-id="22914-130">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="22914-131">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="22914-131">excludedGroups</span></span>|<span data-ttu-id="22914-132">Коллекция объектов Guid</span><span class="sxs-lookup"><span data-stu-id="22914-132">Guid collection</span></span>|<span data-ttu-id="22914-133">Группы пользователей, на которые не распространяется условный доступ к локальной среде.</span><span class="sxs-lookup"><span data-stu-id="22914-133">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="22914-134">На всех пользователей из этих группах не будет распространяться политика условного доступа.</span><span class="sxs-lookup"><span data-stu-id="22914-134">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="22914-135">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="22914-135">overrideDefaultRule</span></span>|<span data-ttu-id="22914-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="22914-136">Boolean</span></span>|<span data-ttu-id="22914-137">Указывает, следует ли переопределять правило доступа по умолчанию при разрешении устройства, чтобы обеспечить предоставление доступа.</span><span class="sxs-lookup"><span data-stu-id="22914-137">Override the default access rule when allowing a device to ensure access is granted.</span></span>|

## <a name="relationships"></a><span data-ttu-id="22914-138">Отношения</span><span class="sxs-lookup"><span data-stu-id="22914-138">Relationships</span></span>
<span data-ttu-id="22914-139">Нет</span><span class="sxs-lookup"><span data-stu-id="22914-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="22914-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="22914-140">JSON Representation</span></span>
<span data-ttu-id="22914-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="22914-141">Here is a JSON representation of the resource.</span></span>
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





