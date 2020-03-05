---
title: Тип ресурса Оффицеконфигуратион
description: Одноэлементный объект, служащий контейнером для всех функций управления устройствами.
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6967972cbc94d28d6fde605ba72f3497b9b48e46
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42488245"
---
# <a name="officeconfiguration-resource-type"></a><span data-ttu-id="185b4-103">Тип ресурса Оффицеконфигуратион</span><span class="sxs-lookup"><span data-stu-id="185b4-103">officeConfiguration resource type</span></span>

<span data-ttu-id="185b4-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="185b4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="185b4-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="185b4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="185b4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="185b4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="185b4-107">Одноэлементный объект, служащий контейнером для всех функций управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="185b4-107">Singleton entity that acts as a container for all device management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="185b4-108">Методы</span><span class="sxs-lookup"><span data-stu-id="185b4-108">Methods</span></span>
|<span data-ttu-id="185b4-109">Метод</span><span class="sxs-lookup"><span data-stu-id="185b4-109">Method</span></span>|<span data-ttu-id="185b4-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="185b4-110">Return Type</span></span>|<span data-ttu-id="185b4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="185b4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="185b4-112">Получение Оффицеконфигуратион</span><span class="sxs-lookup"><span data-stu-id="185b4-112">Get officeConfiguration</span></span>|[<span data-ttu-id="185b4-113">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="185b4-113">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="185b4-114">Чтение свойств и связей объекта [оффицеконфигуратион](../resources/intune-cirrus-officeconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="185b4-114">Read properties and relationships of the [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|
|<span data-ttu-id="185b4-115">Обновление Оффицеконфигуратион</span><span class="sxs-lookup"><span data-stu-id="185b4-115">Update officeConfiguration</span></span>|[<span data-ttu-id="185b4-116">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="185b4-116">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="185b4-117">Обновление свойств объекта [оффицеконфигуратион](../resources/intune-cirrus-officeconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="185b4-117">Update the properties of a [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="185b4-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="185b4-118">Properties</span></span>
|<span data-ttu-id="185b4-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="185b4-119">Property</span></span>|<span data-ttu-id="185b4-120">Тип</span><span class="sxs-lookup"><span data-stu-id="185b4-120">Type</span></span>|<span data-ttu-id="185b4-121">Описание</span><span class="sxs-lookup"><span data-stu-id="185b4-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="185b4-122">id</span><span class="sxs-lookup"><span data-stu-id="185b4-122">id</span></span>|<span data-ttu-id="185b4-123">String</span><span class="sxs-lookup"><span data-stu-id="185b4-123">String</span></span>|<span data-ttu-id="185b4-124">Идентификатор конфигурации Office.</span><span class="sxs-lookup"><span data-stu-id="185b4-124">Id of the office configuration.</span></span>|
|<span data-ttu-id="185b4-125">тенантчеккинстатусес</span><span class="sxs-lookup"><span data-stu-id="185b4-125">tenantCheckinStatuses</span></span>|<span data-ttu-id="185b4-126">Коллекция [оффицеклиентчеккинстатус](../resources/intune-cirrus-officeclientcheckinstatus.md)</span><span class="sxs-lookup"><span data-stu-id="185b4-126">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="185b4-127">Список состояния возврата клиента Office.</span><span class="sxs-lookup"><span data-stu-id="185b4-127">List of office Client check-in status.</span></span>|
|<span data-ttu-id="185b4-128">тенантусерчеккинсуммари</span><span class="sxs-lookup"><span data-stu-id="185b4-128">tenantUserCheckinSummary</span></span>|[<span data-ttu-id="185b4-129">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="185b4-129">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="185b4-130">Сущность, описывающая возврат клиента статуес</span><span class="sxs-lookup"><span data-stu-id="185b4-130">Entity that describes tenant check-in statues</span></span>|

## <a name="relationships"></a><span data-ttu-id="185b4-131">Связи</span><span class="sxs-lookup"><span data-stu-id="185b4-131">Relationships</span></span>
|<span data-ttu-id="185b4-132">Связь</span><span class="sxs-lookup"><span data-stu-id="185b4-132">Relationship</span></span>|<span data-ttu-id="185b4-133">Тип</span><span class="sxs-lookup"><span data-stu-id="185b4-133">Type</span></span>|<span data-ttu-id="185b4-134">Описание</span><span class="sxs-lookup"><span data-stu-id="185b4-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="185b4-135">клиентконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="185b4-135">clientConfigurations</span></span>|<span data-ttu-id="185b4-136">Коллекция [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="185b4-136">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) collection</span></span>|<span data-ttu-id="185b4-137">Список конфигураций клиентов Office.</span><span class="sxs-lookup"><span data-stu-id="185b4-137">List of office Client configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="185b4-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="185b4-138">JSON Representation</span></span>
<span data-ttu-id="185b4-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="185b4-139">Here is a JSON representation of the resource.</span></span>
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



