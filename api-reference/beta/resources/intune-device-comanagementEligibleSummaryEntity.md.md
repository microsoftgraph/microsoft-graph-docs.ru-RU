---
title: Тип ресурса Команажементелигиблесуммарентити
description: Тип ресурса Команажементелигиблесуммарентити
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 80c2afff56d845097990ef927a743678a248c9fd
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636583"
---
# <a name="comanagementeligiblesummaryentity-resource-type"></a><span data-ttu-id="dbf3f-103">Тип ресурса Команажементелигиблесуммарентити</span><span class="sxs-lookup"><span data-stu-id="dbf3f-103">comanagementEligibleSummaryEntity resource type</span></span>

> <span data-ttu-id="dbf3f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dbf3f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dbf3f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dbf3f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dbf3f-106">Состояние конфигурации мобильного приложения для управляемого устройства для данного устройства.</span><span class="sxs-lookup"><span data-stu-id="dbf3f-106">Managed Device Mobile App Configuration State for a given device.</span></span>

## <a name="methods"></a><span data-ttu-id="dbf3f-107">Методы</span><span class="sxs-lookup"><span data-stu-id="dbf3f-107">Methods</span></span>
|<span data-ttu-id="dbf3f-108">Метод</span><span class="sxs-lookup"><span data-stu-id="dbf3f-108">Method</span></span>|<span data-ttu-id="dbf3f-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="dbf3f-109">Return Type</span></span>|<span data-ttu-id="dbf3f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="dbf3f-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="dbf3f-111">Список Команажементелигиблесуммарентити</span><span class="sxs-lookup"><span data-stu-id="dbf3f-111">List comanagementEligibleSummaryEntity</span></span>](../api/intune-device-comanagementEligibleSummaryEntity-list.md)|<span data-ttu-id="dbf3f-112">Коллекция Команажементелигиблесуммарентити</span><span class="sxs-lookup"><span data-stu-id="dbf3f-112">comanagementEligibleSummaryEntity collection</span></span>|<span data-ttu-id="dbf3f-113">Список свойств и связей объектов Команажементелигиблесуммарентити.</span><span class="sxs-lookup"><span data-stu-id="dbf3f-113">List properties and relationships of the comanagementEligibleSummaryEntity objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="dbf3f-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="dbf3f-114">Properties</span></span>
|<span data-ttu-id="dbf3f-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="dbf3f-115">Property</span></span>|<span data-ttu-id="dbf3f-116">Тип</span><span class="sxs-lookup"><span data-stu-id="dbf3f-116">Type</span></span>|<span data-ttu-id="dbf3f-117">Описание</span><span class="sxs-lookup"><span data-stu-id="dbf3f-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dbf3f-118">id</span><span class="sxs-lookup"><span data-stu-id="dbf3f-118">id</span></span>|<span data-ttu-id="dbf3f-119">Строка</span><span class="sxs-lookup"><span data-stu-id="dbf3f-119">String</span></span>|<span data-ttu-id="dbf3f-120">Уникальный идентификатор Елигибледевицесуммарентити</span><span class="sxs-lookup"><span data-stu-id="dbf3f-120">Unique Id of the EligibleDeviceSummaryEntity</span></span>|
|<span data-ttu-id="dbf3f-121">команажедкаунт</span><span class="sxs-lookup"><span data-stu-id="dbf3f-121">coManagedCount</span></span>|<span data-ttu-id="dbf3f-122">Int32</span><span class="sxs-lookup"><span data-stu-id="dbf3f-122">Int32</span></span>|<span data-ttu-id="dbf3f-123">Количество устройств, которые уже соуправлялись</span><span class="sxs-lookup"><span data-stu-id="dbf3f-123">Count of devices already CoManaged</span></span>|
|<span data-ttu-id="dbf3f-124">елигиблекаунт</span><span class="sxs-lookup"><span data-stu-id="dbf3f-124">eligibleCount</span></span>|<span data-ttu-id="dbf3f-125">Int32</span><span class="sxs-lookup"><span data-stu-id="dbf3f-125">Int32</span></span>|<span data-ttu-id="dbf3f-126">Количество устройств, полностью доступных для управления</span><span class="sxs-lookup"><span data-stu-id="dbf3f-126">Count of devices fully eligible for CoManagement</span></span>|
|<span data-ttu-id="dbf3f-127">елигиблебутнотааджоинедкаунт</span><span class="sxs-lookup"><span data-stu-id="dbf3f-127">eligibleButNotAadJoinedCount</span></span>|<span data-ttu-id="dbf3f-128">Int32</span><span class="sxs-lookup"><span data-stu-id="dbf3f-128">Int32</span></span>|<span data-ttu-id="dbf3f-129">Количество устройств, подходящих для управления, но еще не присоединенных к Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="dbf3f-129">Count of devices eligible for CoManagement but not yet joined to Azure Active Directory</span></span>|
|<span data-ttu-id="dbf3f-130">нидсосупдатекаунт</span><span class="sxs-lookup"><span data-stu-id="dbf3f-130">needsOSUpdateCount</span></span>|<span data-ttu-id="dbf3f-131">Int32</span><span class="sxs-lookup"><span data-stu-id="dbf3f-131">Int32</span></span>|<span data-ttu-id="dbf3f-132">Количество устройств, которые будут доступны для управления после обновления ОС</span><span class="sxs-lookup"><span data-stu-id="dbf3f-132">Count of devices that will be eligible for CoManagement after an OS update</span></span>|

## <a name="relationships"></a><span data-ttu-id="dbf3f-133">Связи</span><span class="sxs-lookup"><span data-stu-id="dbf3f-133">Relationships</span></span>
<span data-ttu-id="dbf3f-134">Нет</span><span class="sxs-lookup"><span data-stu-id="dbf3f-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dbf3f-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dbf3f-135">JSON Representation</span></span>
<span data-ttu-id="dbf3f-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dbf3f-136">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.comanagementEligibleSummaryEntity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.comanagementEligibleSummaryEntity",
  "id": "String (identifier)",
  "coManagedCount": 1024,
  "eligibleCount": 1024,
  "eligibleButNotAadJoinedCount": 1024,
  "needsOSUpdateCount": 1024
}
```

