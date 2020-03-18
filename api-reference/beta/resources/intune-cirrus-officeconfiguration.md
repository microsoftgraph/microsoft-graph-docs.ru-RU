---
title: Тип ресурса Оффицеконфигуратион
description: Одноэлементный объект, служащий контейнером для всех функций управления устройствами.
localization_priority: Normal
author: davidmu1
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 26d6023224048166d0d287ce893c07663638e1f9
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797320"
---
# <a name="officeconfiguration-resource-type"></a><span data-ttu-id="2e2c2-103">Тип ресурса Оффицеконфигуратион</span><span class="sxs-lookup"><span data-stu-id="2e2c2-103">officeConfiguration resource type</span></span>

> <span data-ttu-id="2e2c2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e2c2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2e2c2-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2e2c2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e2c2-106">Одноэлементный объект, служащий контейнером для всех функций управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="2e2c2-106">Singleton entity that acts as a container for all device management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="2e2c2-107">Методы</span><span class="sxs-lookup"><span data-stu-id="2e2c2-107">Methods</span></span>
|<span data-ttu-id="2e2c2-108">Метод</span><span class="sxs-lookup"><span data-stu-id="2e2c2-108">Method</span></span>|<span data-ttu-id="2e2c2-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2e2c2-109">Return Type</span></span>|<span data-ttu-id="2e2c2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2e2c2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e2c2-111">Получение Оффицеконфигуратион</span><span class="sxs-lookup"><span data-stu-id="2e2c2-111">Get officeConfiguration</span></span>|[<span data-ttu-id="2e2c2-112">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="2e2c2-112">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="2e2c2-113">Чтение свойств и связей объекта [оффицеконфигуратион](../resources/intune-cirrus-officeconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="2e2c2-113">Read properties and relationships of the [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|
|<span data-ttu-id="2e2c2-114">Обновление Оффицеконфигуратион</span><span class="sxs-lookup"><span data-stu-id="2e2c2-114">Update officeConfiguration</span></span>|[<span data-ttu-id="2e2c2-115">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="2e2c2-115">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="2e2c2-116">Обновление свойств объекта [оффицеконфигуратион](../resources/intune-cirrus-officeconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="2e2c2-116">Update the properties of a [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2e2c2-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="2e2c2-117">Properties</span></span>
|<span data-ttu-id="2e2c2-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="2e2c2-118">Property</span></span>|<span data-ttu-id="2e2c2-119">Тип</span><span class="sxs-lookup"><span data-stu-id="2e2c2-119">Type</span></span>|<span data-ttu-id="2e2c2-120">Описание</span><span class="sxs-lookup"><span data-stu-id="2e2c2-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e2c2-121">id</span><span class="sxs-lookup"><span data-stu-id="2e2c2-121">id</span></span>|<span data-ttu-id="2e2c2-122">String</span><span class="sxs-lookup"><span data-stu-id="2e2c2-122">String</span></span>|<span data-ttu-id="2e2c2-123">Идентификатор конфигурации Office.</span><span class="sxs-lookup"><span data-stu-id="2e2c2-123">Id of the office configuration.</span></span>|
|<span data-ttu-id="2e2c2-124">тенантчеккинстатусес</span><span class="sxs-lookup"><span data-stu-id="2e2c2-124">tenantCheckinStatuses</span></span>|<span data-ttu-id="2e2c2-125">Коллекция [оффицеклиентчеккинстатус](../resources/intune-cirrus-officeclientcheckinstatus.md)</span><span class="sxs-lookup"><span data-stu-id="2e2c2-125">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="2e2c2-126">Список состояния возврата клиента Office.</span><span class="sxs-lookup"><span data-stu-id="2e2c2-126">List of office Client check-in status.</span></span>|
|<span data-ttu-id="2e2c2-127">тенантусерчеккинсуммари</span><span class="sxs-lookup"><span data-stu-id="2e2c2-127">tenantUserCheckinSummary</span></span>|[<span data-ttu-id="2e2c2-128">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="2e2c2-128">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="2e2c2-129">Сущность, описывающая возврат клиента статуес</span><span class="sxs-lookup"><span data-stu-id="2e2c2-129">Entity that describes tenant check-in statues</span></span>|

## <a name="relationships"></a><span data-ttu-id="2e2c2-130">Связи</span><span class="sxs-lookup"><span data-stu-id="2e2c2-130">Relationships</span></span>
|<span data-ttu-id="2e2c2-131">Связь</span><span class="sxs-lookup"><span data-stu-id="2e2c2-131">Relationship</span></span>|<span data-ttu-id="2e2c2-132">Тип</span><span class="sxs-lookup"><span data-stu-id="2e2c2-132">Type</span></span>|<span data-ttu-id="2e2c2-133">Описание</span><span class="sxs-lookup"><span data-stu-id="2e2c2-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e2c2-134">клиентконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="2e2c2-134">clientConfigurations</span></span>|<span data-ttu-id="2e2c2-135">Коллекция [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2e2c2-135">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) collection</span></span>|<span data-ttu-id="2e2c2-136">Список конфигураций клиентов Office.</span><span class="sxs-lookup"><span data-stu-id="2e2c2-136">List of office Client configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2e2c2-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2e2c2-137">JSON Representation</span></span>
<span data-ttu-id="2e2c2-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2e2c2-138">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeConfiguration",
  "id": "String (identifier)",
  "tenantCheckinStatuses": [
    {
      "@odata.type": "microsoft.graph.officeClientCheckinStatus",
      "userPrincipalName": "String",
      "deviceName": "String",
      "devicePlatform": "String",
      "devicePlatformVersion": "String",
      "wasSuccessful": true,
      "userId": "String",
      "checkinDateTime": "String (timestamp)",
      "errorMessage": "String",
      "appliedPolicies": [
        "String"
      ]
    }
  ],
  "tenantUserCheckinSummary": {
    "@odata.type": "microsoft.graph.officeUserCheckinSummary",
    "succeededUserCount": 1024,
    "failedUserCount": 1024
  }
}
```



