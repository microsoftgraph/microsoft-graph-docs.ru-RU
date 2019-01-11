---
title: Тип ресурса officeConfiguration
description: Одноэлементный объект, служащий контейнером для всех функций управления устройствами.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 096a54db296181e58020bb9bc694056c0b9e949a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817262"
---
# <a name="officeconfiguration-resource-type"></a><span data-ttu-id="19c31-103">Тип ресурса officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="19c31-103">officeConfiguration resource type</span></span>

> <span data-ttu-id="19c31-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="19c31-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="19c31-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19c31-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="19c31-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="19c31-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="19c31-107">Одноэлементный объект, служащий контейнером для всех функций управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="19c31-107">Singleton entity that acts as a container for all device management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="19c31-108">Методы</span><span class="sxs-lookup"><span data-stu-id="19c31-108">Methods</span></span>
|<span data-ttu-id="19c31-109">Метод</span><span class="sxs-lookup"><span data-stu-id="19c31-109">Method</span></span>|<span data-ttu-id="19c31-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="19c31-110">Return Type</span></span>|<span data-ttu-id="19c31-111">Описание</span><span class="sxs-lookup"><span data-stu-id="19c31-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19c31-112">Получение officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="19c31-112">Get officeConfiguration</span></span>|[<span data-ttu-id="19c31-113">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="19c31-113">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="19c31-114">Чтение свойства и связи объекта [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="19c31-114">Read properties and relationships of the [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|
|<span data-ttu-id="19c31-115">Обновление officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="19c31-115">Update officeConfiguration</span></span>|[<span data-ttu-id="19c31-116">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="19c31-116">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="19c31-117">Обновление свойства объекта [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="19c31-117">Update the properties of a [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="19c31-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="19c31-118">Properties</span></span>
|<span data-ttu-id="19c31-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="19c31-119">Property</span></span>|<span data-ttu-id="19c31-120">Тип</span><span class="sxs-lookup"><span data-stu-id="19c31-120">Type</span></span>|<span data-ttu-id="19c31-121">Описание</span><span class="sxs-lookup"><span data-stu-id="19c31-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19c31-122">id</span><span class="sxs-lookup"><span data-stu-id="19c31-122">id</span></span>|<span data-ttu-id="19c31-123">Строка</span><span class="sxs-lookup"><span data-stu-id="19c31-123">String</span></span>|<span data-ttu-id="19c31-124">Идентификатор конфигурации office.</span><span class="sxs-lookup"><span data-stu-id="19c31-124">Id of the office configuration.</span></span>|
|<span data-ttu-id="19c31-125">tenantCheckinStatuses</span><span class="sxs-lookup"><span data-stu-id="19c31-125">tenantCheckinStatuses</span></span>|<span data-ttu-id="19c31-126">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="19c31-126">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="19c31-127">Список office состояние возврата клиента.</span><span class="sxs-lookup"><span data-stu-id="19c31-127">List of office Client check-in status.</span></span>|
|<span data-ttu-id="19c31-128">tenantUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="19c31-128">tenantUserCheckinSummary</span></span>|[<span data-ttu-id="19c31-129">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="19c31-129">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="19c31-130">Сущности, которая описывает клиента возврат statues</span><span class="sxs-lookup"><span data-stu-id="19c31-130">Entity that describes tenant check-in statues</span></span>|

## <a name="relationships"></a><span data-ttu-id="19c31-131">Связи</span><span class="sxs-lookup"><span data-stu-id="19c31-131">Relationships</span></span>
|<span data-ttu-id="19c31-132">Связь</span><span class="sxs-lookup"><span data-stu-id="19c31-132">Relationship</span></span>|<span data-ttu-id="19c31-133">Тип</span><span class="sxs-lookup"><span data-stu-id="19c31-133">Type</span></span>|<span data-ttu-id="19c31-134">Описание</span><span class="sxs-lookup"><span data-stu-id="19c31-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19c31-135">clientConfigurations</span><span class="sxs-lookup"><span data-stu-id="19c31-135">clientConfigurations</span></span>|<span data-ttu-id="19c31-136">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="19c31-136">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) collection</span></span>|<span data-ttu-id="19c31-137">Список настройки клиента office.</span><span class="sxs-lookup"><span data-stu-id="19c31-137">List of office Client configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="19c31-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="19c31-138">JSON Representation</span></span>
<span data-ttu-id="19c31-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="19c31-139">Here is a JSON representation of the resource.</span></span>
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



