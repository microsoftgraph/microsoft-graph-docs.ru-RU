---
title: Тип ресурса Оффицеконфигуратион
description: Одноэлементный объект, служащий контейнером для всех функций управления устройствами.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7e5c36a23be0ab32a14a08eaff297b832ba5274c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32526365"
---
# <a name="officeconfiguration-resource-type"></a><span data-ttu-id="11748-103">Тип ресурса Оффицеконфигуратион</span><span class="sxs-lookup"><span data-stu-id="11748-103">officeConfiguration resource type</span></span>

> <span data-ttu-id="11748-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11748-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="11748-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="11748-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11748-106">Одноэлементный объект, служащий контейнером для всех функций управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="11748-106">Singleton entity that acts as a container for all device management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="11748-107">Методы</span><span class="sxs-lookup"><span data-stu-id="11748-107">Methods</span></span>
|<span data-ttu-id="11748-108">Метод</span><span class="sxs-lookup"><span data-stu-id="11748-108">Method</span></span>|<span data-ttu-id="11748-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="11748-109">Return Type</span></span>|<span data-ttu-id="11748-110">Описание</span><span class="sxs-lookup"><span data-stu-id="11748-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11748-111">Получение Оффицеконфигуратион</span><span class="sxs-lookup"><span data-stu-id="11748-111">Get officeConfiguration</span></span>|[<span data-ttu-id="11748-112">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="11748-112">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="11748-113">Чтение свойств и связей объекта [оффицеконфигуратион](../resources/intune-cirrus-officeconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="11748-113">Read properties and relationships of the [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|
|<span data-ttu-id="11748-114">Обновление Оффицеконфигуратион</span><span class="sxs-lookup"><span data-stu-id="11748-114">Update officeConfiguration</span></span>|[<span data-ttu-id="11748-115">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="11748-115">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="11748-116">Обновление свойств объекта [оффицеконфигуратион](../resources/intune-cirrus-officeconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="11748-116">Update the properties of a [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="11748-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="11748-117">Properties</span></span>
|<span data-ttu-id="11748-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="11748-118">Property</span></span>|<span data-ttu-id="11748-119">Тип</span><span class="sxs-lookup"><span data-stu-id="11748-119">Type</span></span>|<span data-ttu-id="11748-120">Описание</span><span class="sxs-lookup"><span data-stu-id="11748-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11748-121">id</span><span class="sxs-lookup"><span data-stu-id="11748-121">id</span></span>|<span data-ttu-id="11748-122">String</span><span class="sxs-lookup"><span data-stu-id="11748-122">String</span></span>|<span data-ttu-id="11748-123">Идентификатор конфигурации Office.</span><span class="sxs-lookup"><span data-stu-id="11748-123">Id of the office configuration.</span></span>|
|<span data-ttu-id="11748-124">Тенантчеккинстатусес</span><span class="sxs-lookup"><span data-stu-id="11748-124">tenantCheckinStatuses</span></span>|<span data-ttu-id="11748-125">Коллекция [оффицеклиентчеккинстатус](../resources/intune-cirrus-officeclientcheckinstatus.md)</span><span class="sxs-lookup"><span data-stu-id="11748-125">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="11748-126">Список состояния возврата клиента Office.</span><span class="sxs-lookup"><span data-stu-id="11748-126">List of office Client check-in status.</span></span>|
|<span data-ttu-id="11748-127">Тенантусерчеккинсуммари</span><span class="sxs-lookup"><span data-stu-id="11748-127">tenantUserCheckinSummary</span></span>|[<span data-ttu-id="11748-128">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="11748-128">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="11748-129">Сущность, описывающая возврат клиента статуес</span><span class="sxs-lookup"><span data-stu-id="11748-129">Entity that describes tenant check-in statues</span></span>|

## <a name="relationships"></a><span data-ttu-id="11748-130">Связи</span><span class="sxs-lookup"><span data-stu-id="11748-130">Relationships</span></span>
|<span data-ttu-id="11748-131">Отношение</span><span class="sxs-lookup"><span data-stu-id="11748-131">Relationship</span></span>|<span data-ttu-id="11748-132">Тип</span><span class="sxs-lookup"><span data-stu-id="11748-132">Type</span></span>|<span data-ttu-id="11748-133">Описание</span><span class="sxs-lookup"><span data-stu-id="11748-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11748-134">Клиентконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="11748-134">clientConfigurations</span></span>|<span data-ttu-id="11748-135">Коллекция [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="11748-135">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) collection</span></span>|<span data-ttu-id="11748-136">Список конфигураций клиентов Office.</span><span class="sxs-lookup"><span data-stu-id="11748-136">List of office Client configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="11748-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="11748-137">JSON Representation</span></span>
<span data-ttu-id="11748-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="11748-138">Here is a JSON representation of the resource.</span></span>
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



