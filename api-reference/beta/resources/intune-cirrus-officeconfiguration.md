---
title: Тип ресурса Оффицеконфигуратион
description: Одноэлементный объект, служащий контейнером для всех функций управления устройствами.
localization_priority: Normal
author: dougeby
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 203efb4eab301f64eedfaceeba0e007c1a0b0123
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43362612"
---
# <a name="officeconfiguration-resource-type"></a><span data-ttu-id="f1ce7-103">Тип ресурса Оффицеконфигуратион</span><span class="sxs-lookup"><span data-stu-id="f1ce7-103">officeConfiguration resource type</span></span>

<span data-ttu-id="f1ce7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1ce7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f1ce7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1ce7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1ce7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f1ce7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1ce7-107">Одноэлементный объект, служащий контейнером для всех функций управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="f1ce7-107">Singleton entity that acts as a container for all device management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="f1ce7-108">Методы</span><span class="sxs-lookup"><span data-stu-id="f1ce7-108">Methods</span></span>
|<span data-ttu-id="f1ce7-109">Метод</span><span class="sxs-lookup"><span data-stu-id="f1ce7-109">Method</span></span>|<span data-ttu-id="f1ce7-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f1ce7-110">Return Type</span></span>|<span data-ttu-id="f1ce7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f1ce7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1ce7-112">Получение Оффицеконфигуратион</span><span class="sxs-lookup"><span data-stu-id="f1ce7-112">Get officeConfiguration</span></span>|[<span data-ttu-id="f1ce7-113">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="f1ce7-113">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="f1ce7-114">Чтение свойств и связей объекта [оффицеконфигуратион](../resources/intune-cirrus-officeconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f1ce7-114">Read properties and relationships of the [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|
|<span data-ttu-id="f1ce7-115">Обновление Оффицеконфигуратион</span><span class="sxs-lookup"><span data-stu-id="f1ce7-115">Update officeConfiguration</span></span>|[<span data-ttu-id="f1ce7-116">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="f1ce7-116">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="f1ce7-117">Обновление свойств объекта [оффицеконфигуратион](../resources/intune-cirrus-officeconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f1ce7-117">Update the properties of a [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f1ce7-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="f1ce7-118">Properties</span></span>
|<span data-ttu-id="f1ce7-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="f1ce7-119">Property</span></span>|<span data-ttu-id="f1ce7-120">Тип</span><span class="sxs-lookup"><span data-stu-id="f1ce7-120">Type</span></span>|<span data-ttu-id="f1ce7-121">Описание</span><span class="sxs-lookup"><span data-stu-id="f1ce7-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1ce7-122">id</span><span class="sxs-lookup"><span data-stu-id="f1ce7-122">id</span></span>|<span data-ttu-id="f1ce7-123">String</span><span class="sxs-lookup"><span data-stu-id="f1ce7-123">String</span></span>|<span data-ttu-id="f1ce7-124">Идентификатор конфигурации Office.</span><span class="sxs-lookup"><span data-stu-id="f1ce7-124">Id of the office configuration.</span></span>|
|<span data-ttu-id="f1ce7-125">тенантчеккинстатусес</span><span class="sxs-lookup"><span data-stu-id="f1ce7-125">tenantCheckinStatuses</span></span>|<span data-ttu-id="f1ce7-126">Коллекция [оффицеклиентчеккинстатус](../resources/intune-cirrus-officeclientcheckinstatus.md)</span><span class="sxs-lookup"><span data-stu-id="f1ce7-126">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="f1ce7-127">Список состояния возврата клиента Office.</span><span class="sxs-lookup"><span data-stu-id="f1ce7-127">List of office Client check-in status.</span></span>|
|<span data-ttu-id="f1ce7-128">тенантусерчеккинсуммари</span><span class="sxs-lookup"><span data-stu-id="f1ce7-128">tenantUserCheckinSummary</span></span>|[<span data-ttu-id="f1ce7-129">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="f1ce7-129">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="f1ce7-130">Сущность, описывающая возврат клиента статуес</span><span class="sxs-lookup"><span data-stu-id="f1ce7-130">Entity that describes tenant check-in statues</span></span>|

## <a name="relationships"></a><span data-ttu-id="f1ce7-131">Связи</span><span class="sxs-lookup"><span data-stu-id="f1ce7-131">Relationships</span></span>
|<span data-ttu-id="f1ce7-132">Связь</span><span class="sxs-lookup"><span data-stu-id="f1ce7-132">Relationship</span></span>|<span data-ttu-id="f1ce7-133">Тип</span><span class="sxs-lookup"><span data-stu-id="f1ce7-133">Type</span></span>|<span data-ttu-id="f1ce7-134">Описание</span><span class="sxs-lookup"><span data-stu-id="f1ce7-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1ce7-135">клиентконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="f1ce7-135">clientConfigurations</span></span>|<span data-ttu-id="f1ce7-136">Коллекция [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1ce7-136">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) collection</span></span>|<span data-ttu-id="f1ce7-137">Список конфигураций клиентов Office.</span><span class="sxs-lookup"><span data-stu-id="f1ce7-137">List of office Client configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f1ce7-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f1ce7-138">JSON Representation</span></span>
<span data-ttu-id="f1ce7-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f1ce7-139">Here is a JSON representation of the resource.</span></span>
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



