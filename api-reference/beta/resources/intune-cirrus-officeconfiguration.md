---
title: Тип ресурса Оффицеконфигуратион
description: Одноэлементный объект, служащий контейнером для всех функций управления устройствами.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 276a9bd60e988d0bb961ef849c8ce57d8eb9bb47
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48723974"
---
# <a name="officeconfiguration-resource-type"></a><span data-ttu-id="1a875-103">Тип ресурса Оффицеконфигуратион</span><span class="sxs-lookup"><span data-stu-id="1a875-103">officeConfiguration resource type</span></span>

<span data-ttu-id="1a875-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a875-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1a875-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a875-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a875-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1a875-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a875-107">Одноэлементный объект, служащий контейнером для всех функций управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="1a875-107">Singleton entity that acts as a container for all device management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="1a875-108">Методы</span><span class="sxs-lookup"><span data-stu-id="1a875-108">Methods</span></span>
|<span data-ttu-id="1a875-109">Метод</span><span class="sxs-lookup"><span data-stu-id="1a875-109">Method</span></span>|<span data-ttu-id="1a875-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1a875-110">Return Type</span></span>|<span data-ttu-id="1a875-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1a875-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a875-112">Получение Оффицеконфигуратион</span><span class="sxs-lookup"><span data-stu-id="1a875-112">Get officeConfiguration</span></span>|[<span data-ttu-id="1a875-113">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="1a875-113">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="1a875-114">Чтение свойств и связей объекта [оффицеконфигуратион](../resources/intune-cirrus-officeconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="1a875-114">Read properties and relationships of the [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|
|<span data-ttu-id="1a875-115">Обновление Оффицеконфигуратион</span><span class="sxs-lookup"><span data-stu-id="1a875-115">Update officeConfiguration</span></span>|[<span data-ttu-id="1a875-116">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="1a875-116">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="1a875-117">Обновление свойств объекта [оффицеконфигуратион](../resources/intune-cirrus-officeconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="1a875-117">Update the properties of a [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1a875-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="1a875-118">Properties</span></span>
|<span data-ttu-id="1a875-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="1a875-119">Property</span></span>|<span data-ttu-id="1a875-120">Тип</span><span class="sxs-lookup"><span data-stu-id="1a875-120">Type</span></span>|<span data-ttu-id="1a875-121">Описание</span><span class="sxs-lookup"><span data-stu-id="1a875-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a875-122">id</span><span class="sxs-lookup"><span data-stu-id="1a875-122">id</span></span>|<span data-ttu-id="1a875-123">Строка</span><span class="sxs-lookup"><span data-stu-id="1a875-123">String</span></span>|<span data-ttu-id="1a875-124">Идентификатор конфигурации Office.</span><span class="sxs-lookup"><span data-stu-id="1a875-124">Id of the office configuration.</span></span>|
|<span data-ttu-id="1a875-125">тенантчеккинстатусес</span><span class="sxs-lookup"><span data-stu-id="1a875-125">tenantCheckinStatuses</span></span>|<span data-ttu-id="1a875-126">Коллекция [оффицеклиентчеккинстатус](../resources/intune-cirrus-officeclientcheckinstatus.md)</span><span class="sxs-lookup"><span data-stu-id="1a875-126">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="1a875-127">Список состояния возврата клиента Office.</span><span class="sxs-lookup"><span data-stu-id="1a875-127">List of office Client check-in status.</span></span>|
|<span data-ttu-id="1a875-128">тенантусерчеккинсуммари</span><span class="sxs-lookup"><span data-stu-id="1a875-128">tenantUserCheckinSummary</span></span>|[<span data-ttu-id="1a875-129">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="1a875-129">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="1a875-130">Сущность, описывающая возврат клиента статуес</span><span class="sxs-lookup"><span data-stu-id="1a875-130">Entity that describes tenant check-in statues</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a875-131">Связи</span><span class="sxs-lookup"><span data-stu-id="1a875-131">Relationships</span></span>
|<span data-ttu-id="1a875-132">Связь</span><span class="sxs-lookup"><span data-stu-id="1a875-132">Relationship</span></span>|<span data-ttu-id="1a875-133">Тип</span><span class="sxs-lookup"><span data-stu-id="1a875-133">Type</span></span>|<span data-ttu-id="1a875-134">Описание</span><span class="sxs-lookup"><span data-stu-id="1a875-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a875-135">клиентконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="1a875-135">clientConfigurations</span></span>|<span data-ttu-id="1a875-136">Коллекция [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a875-136">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) collection</span></span>|<span data-ttu-id="1a875-137">Список конфигураций клиентов Office.</span><span class="sxs-lookup"><span data-stu-id="1a875-137">List of office Client configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1a875-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1a875-138">JSON Representation</span></span>
<span data-ttu-id="1a875-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1a875-139">Here is a JSON representation of the resource.</span></span>
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





