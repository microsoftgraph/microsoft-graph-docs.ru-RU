---
title: Тип ресурса officeConfiguration
description: Одноэлементный объект, служащий контейнером для всех функций управления устройствами.
author: tfitzmac
ms.openlocfilehash: bf74789d4debda00b21173ff2974db8224cd15f0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305546"
---
# <a name="officeconfiguration-resource-type"></a><span data-ttu-id="b534d-103">Тип ресурса officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="b534d-103">officeConfiguration resource type</span></span>

> <span data-ttu-id="b534d-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b534d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b534d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b534d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b534d-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b534d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b534d-107">Одноэлементный объект, служащий контейнером для всех функций управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="b534d-107">Singleton entity that acts as a container for all device management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="b534d-108">Методы</span><span class="sxs-lookup"><span data-stu-id="b534d-108">Methods</span></span>
|<span data-ttu-id="b534d-109">Метод</span><span class="sxs-lookup"><span data-stu-id="b534d-109">Method</span></span>|<span data-ttu-id="b534d-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b534d-110">Return Type</span></span>|<span data-ttu-id="b534d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b534d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b534d-112">Получение officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="b534d-112">Get officeConfiguration</span></span>|[<span data-ttu-id="b534d-113">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="b534d-113">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="b534d-114">Чтение свойства и связи объекта [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="b534d-114">Read properties and relationships of the [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|
|<span data-ttu-id="b534d-115">Обновление officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="b534d-115">Update officeConfiguration</span></span>|[<span data-ttu-id="b534d-116">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="b534d-116">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="b534d-117">Обновление свойства объекта [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="b534d-117">Update the properties of a [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b534d-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="b534d-118">Properties</span></span>
|<span data-ttu-id="b534d-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="b534d-119">Property</span></span>|<span data-ttu-id="b534d-120">Тип</span><span class="sxs-lookup"><span data-stu-id="b534d-120">Type</span></span>|<span data-ttu-id="b534d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="b534d-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b534d-122">id</span><span class="sxs-lookup"><span data-stu-id="b534d-122">id</span></span>|<span data-ttu-id="b534d-123">Строка</span><span class="sxs-lookup"><span data-stu-id="b534d-123">String</span></span>|<span data-ttu-id="b534d-124">Идентификатор конфигурации office.</span><span class="sxs-lookup"><span data-stu-id="b534d-124">Id of the office configuration.</span></span>|
|<span data-ttu-id="b534d-125">tenantCheckinStatuses</span><span class="sxs-lookup"><span data-stu-id="b534d-125">tenantCheckinStatuses</span></span>|<span data-ttu-id="b534d-126">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="b534d-126">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="b534d-127">Список office состояние возврата клиента.</span><span class="sxs-lookup"><span data-stu-id="b534d-127">List of office Client check-in status.</span></span>|
|<span data-ttu-id="b534d-128">tenantUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="b534d-128">tenantUserCheckinSummary</span></span>|[<span data-ttu-id="b534d-129">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="b534d-129">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="b534d-130">Сущности, которая описывает клиента возврат statues</span><span class="sxs-lookup"><span data-stu-id="b534d-130">Entity that describes tenant check-in statues</span></span>|

## <a name="relationships"></a><span data-ttu-id="b534d-131">Связи</span><span class="sxs-lookup"><span data-stu-id="b534d-131">Relationships</span></span>
|<span data-ttu-id="b534d-132">Связь</span><span class="sxs-lookup"><span data-stu-id="b534d-132">Relationship</span></span>|<span data-ttu-id="b534d-133">Тип</span><span class="sxs-lookup"><span data-stu-id="b534d-133">Type</span></span>|<span data-ttu-id="b534d-134">Описание</span><span class="sxs-lookup"><span data-stu-id="b534d-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b534d-135">clientConfigurations</span><span class="sxs-lookup"><span data-stu-id="b534d-135">clientConfigurations</span></span>|<span data-ttu-id="b534d-136">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="b534d-136">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) collection</span></span>|<span data-ttu-id="b534d-137">Список настройки клиента office.</span><span class="sxs-lookup"><span data-stu-id="b534d-137">List of office Client configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b534d-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b534d-138">JSON Representation</span></span>
<span data-ttu-id="b534d-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b534d-139">Here is a JSON representation of the resource.</span></span>
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



