---
title: Тип ресурса officeConfiguration
description: Одноэлементный объект, служащий контейнером для всех функций управления устройствами.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 20e86afa8d0d5fddf5b87a6c6667e2e16baa391a
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753097"
---
# <a name="officeconfiguration-resource-type"></a><span data-ttu-id="9837b-103">Тип ресурса officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="9837b-103">officeConfiguration resource type</span></span>

<span data-ttu-id="9837b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9837b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9837b-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9837b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9837b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9837b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9837b-107">Одноэлементный объект, служащий контейнером для всех функций управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="9837b-107">Singleton entity that acts as a container for all device management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="9837b-108">Методы</span><span class="sxs-lookup"><span data-stu-id="9837b-108">Methods</span></span>
|<span data-ttu-id="9837b-109">Метод</span><span class="sxs-lookup"><span data-stu-id="9837b-109">Method</span></span>|<span data-ttu-id="9837b-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9837b-110">Return Type</span></span>|<span data-ttu-id="9837b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9837b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9837b-112">Get officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="9837b-112">Get officeConfiguration</span></span>|[<span data-ttu-id="9837b-113">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="9837b-113">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="9837b-114">Чтение свойств и связей [объекта OfficeConfiguration.](../resources/intune-cirrus-officeconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9837b-114">Read properties and relationships of the [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|
|<span data-ttu-id="9837b-115">Обновление officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="9837b-115">Update officeConfiguration</span></span>|[<span data-ttu-id="9837b-116">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="9837b-116">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="9837b-117">Обновление свойств объекта [officeConfiguration.](../resources/intune-cirrus-officeconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9837b-117">Update the properties of a [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9837b-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="9837b-118">Properties</span></span>
|<span data-ttu-id="9837b-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="9837b-119">Property</span></span>|<span data-ttu-id="9837b-120">Тип</span><span class="sxs-lookup"><span data-stu-id="9837b-120">Type</span></span>|<span data-ttu-id="9837b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="9837b-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9837b-122">id</span><span class="sxs-lookup"><span data-stu-id="9837b-122">id</span></span>|<span data-ttu-id="9837b-123">String</span><span class="sxs-lookup"><span data-stu-id="9837b-123">String</span></span>|<span data-ttu-id="9837b-124">Id конфигурации офиса.</span><span class="sxs-lookup"><span data-stu-id="9837b-124">Id of the office configuration.</span></span>|
|<span data-ttu-id="9837b-125">tenantCheckinStatuses</span><span class="sxs-lookup"><span data-stu-id="9837b-125">tenantCheckinStatuses</span></span>|<span data-ttu-id="9837b-126">[коллекция officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)</span><span class="sxs-lookup"><span data-stu-id="9837b-126">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="9837b-127">Список состояния регистрации клиента office.</span><span class="sxs-lookup"><span data-stu-id="9837b-127">List of office Client check-in status.</span></span>|
|<span data-ttu-id="9837b-128">tenantUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="9837b-128">tenantUserCheckinSummary</span></span>|[<span data-ttu-id="9837b-129">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="9837b-129">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="9837b-130">Объект, описывая статуи регистрации клиента</span><span class="sxs-lookup"><span data-stu-id="9837b-130">Entity that describes tenant check-in statues</span></span>|

## <a name="relationships"></a><span data-ttu-id="9837b-131">Связи</span><span class="sxs-lookup"><span data-stu-id="9837b-131">Relationships</span></span>
|<span data-ttu-id="9837b-132">Связь</span><span class="sxs-lookup"><span data-stu-id="9837b-132">Relationship</span></span>|<span data-ttu-id="9837b-133">Тип</span><span class="sxs-lookup"><span data-stu-id="9837b-133">Type</span></span>|<span data-ttu-id="9837b-134">Описание</span><span class="sxs-lookup"><span data-stu-id="9837b-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9837b-135">clientConfigurations</span><span class="sxs-lookup"><span data-stu-id="9837b-135">clientConfigurations</span></span>|<span data-ttu-id="9837b-136">[коллекция officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9837b-136">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) collection</span></span>|<span data-ttu-id="9837b-137">Список конфигурации клиента office.</span><span class="sxs-lookup"><span data-stu-id="9837b-137">List of office Client configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9837b-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9837b-138">JSON Representation</span></span>
<span data-ttu-id="9837b-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9837b-139">Here is a JSON representation of the resource.</span></span>
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




