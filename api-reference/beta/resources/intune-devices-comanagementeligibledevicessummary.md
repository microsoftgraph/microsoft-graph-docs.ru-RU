---
title: Тип ресурса Команажементелигибледевицессуммари
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 03baadeea1441d5eecc1ff6e8974724b19a59949
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48697786"
---
# <a name="comanagementeligibledevicessummary-resource-type"></a><span data-ttu-id="bdb42-103">Тип ресурса Команажементелигибледевицессуммари</span><span class="sxs-lookup"><span data-stu-id="bdb42-103">comanagementEligibleDevicesSummary resource type</span></span>

<span data-ttu-id="bdb42-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bdb42-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bdb42-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bdb42-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bdb42-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bdb42-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bdb42-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="bdb42-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="bdb42-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="bdb42-108">Properties</span></span>
|<span data-ttu-id="bdb42-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="bdb42-109">Property</span></span>|<span data-ttu-id="bdb42-110">Тип</span><span class="sxs-lookup"><span data-stu-id="bdb42-110">Type</span></span>|<span data-ttu-id="bdb42-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bdb42-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bdb42-112">команажедкаунт</span><span class="sxs-lookup"><span data-stu-id="bdb42-112">comanagedCount</span></span>|<span data-ttu-id="bdb42-113">Int32</span><span class="sxs-lookup"><span data-stu-id="bdb42-113">Int32</span></span>|<span data-ttu-id="bdb42-114">Количество устройств, уже Co-Managed</span><span class="sxs-lookup"><span data-stu-id="bdb42-114">Count of devices already Co-Managed</span></span>|
|<span data-ttu-id="bdb42-115">елигиблекаунт</span><span class="sxs-lookup"><span data-stu-id="bdb42-115">eligibleCount</span></span>|<span data-ttu-id="bdb42-116">Int32</span><span class="sxs-lookup"><span data-stu-id="bdb42-116">Int32</span></span>|<span data-ttu-id="bdb42-117">Количество устройств, полностью доступных для Co-Management</span><span class="sxs-lookup"><span data-stu-id="bdb42-117">Count of devices fully eligible for Co-Management</span></span>|
|<span data-ttu-id="bdb42-118">елигиблебутнотазуреаджоинедкаунт</span><span class="sxs-lookup"><span data-stu-id="bdb42-118">eligibleButNotAzureAdJoinedCount</span></span>|<span data-ttu-id="bdb42-119">Int32</span><span class="sxs-lookup"><span data-stu-id="bdb42-119">Int32</span></span>|<span data-ttu-id="bdb42-120">Количество устройств, подходящих для Co-Management, но еще не присоединенных к Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="bdb42-120">Count of devices eligible for Co-Management but not yet joined to Azure Active Directory</span></span>|
|<span data-ttu-id="bdb42-121">нидсосупдатекаунт</span><span class="sxs-lookup"><span data-stu-id="bdb42-121">needsOsUpdateCount</span></span>|<span data-ttu-id="bdb42-122">Int32</span><span class="sxs-lookup"><span data-stu-id="bdb42-122">Int32</span></span>|<span data-ttu-id="bdb42-123">Количество устройств, которые будут доступны Co-Management после обновления ОС</span><span class="sxs-lookup"><span data-stu-id="bdb42-123">Count of devices that will be eligible for Co-Management after an OS update</span></span>|
|<span data-ttu-id="bdb42-124">инелигиблекаунт</span><span class="sxs-lookup"><span data-stu-id="bdb42-124">ineligibleCount</span></span>|<span data-ttu-id="bdb42-125">Int32</span><span class="sxs-lookup"><span data-stu-id="bdb42-125">Int32</span></span>|<span data-ttu-id="bdb42-126">Количество устройств, доступных для Co-Management</span><span class="sxs-lookup"><span data-stu-id="bdb42-126">Count of devices ineligible for Co-Management</span></span>|

## <a name="relationships"></a><span data-ttu-id="bdb42-127">Связи</span><span class="sxs-lookup"><span data-stu-id="bdb42-127">Relationships</span></span>
<span data-ttu-id="bdb42-128">Нет</span><span class="sxs-lookup"><span data-stu-id="bdb42-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bdb42-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bdb42-129">JSON Representation</span></span>
<span data-ttu-id="bdb42-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bdb42-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.comanagementEligibleDevicesSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.comanagementEligibleDevicesSummary",
  "comanagedCount": 1024,
  "eligibleCount": 1024,
  "eligibleButNotAzureAdJoinedCount": 1024,
  "needsOsUpdateCount": 1024,
  "ineligibleCount": 1024
}
```





