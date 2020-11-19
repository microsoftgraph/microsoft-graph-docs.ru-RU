---
title: Тип ресурса Команажементелигибледевицессуммари
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4c7244bd594e38a8f129aa81389b159caff6b928
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49214640"
---
# <a name="comanagementeligibledevicessummary-resource-type"></a><span data-ttu-id="21058-103">Тип ресурса Команажементелигибледевицессуммари</span><span class="sxs-lookup"><span data-stu-id="21058-103">comanagementEligibleDevicesSummary resource type</span></span>

<span data-ttu-id="21058-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21058-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="21058-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21058-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21058-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="21058-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21058-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="21058-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="21058-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="21058-108">Properties</span></span>
|<span data-ttu-id="21058-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="21058-109">Property</span></span>|<span data-ttu-id="21058-110">Тип</span><span class="sxs-lookup"><span data-stu-id="21058-110">Type</span></span>|<span data-ttu-id="21058-111">Описание</span><span class="sxs-lookup"><span data-stu-id="21058-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21058-112">команажедкаунт</span><span class="sxs-lookup"><span data-stu-id="21058-112">comanagedCount</span></span>|<span data-ttu-id="21058-113">Int32</span><span class="sxs-lookup"><span data-stu-id="21058-113">Int32</span></span>|<span data-ttu-id="21058-114">Количество устройств, уже Co-Managed</span><span class="sxs-lookup"><span data-stu-id="21058-114">Count of devices already Co-Managed</span></span>|
|<span data-ttu-id="21058-115">елигиблекаунт</span><span class="sxs-lookup"><span data-stu-id="21058-115">eligibleCount</span></span>|<span data-ttu-id="21058-116">Int32</span><span class="sxs-lookup"><span data-stu-id="21058-116">Int32</span></span>|<span data-ttu-id="21058-117">Количество устройств, полностью доступных для Co-Management</span><span class="sxs-lookup"><span data-stu-id="21058-117">Count of devices fully eligible for Co-Management</span></span>|
|<span data-ttu-id="21058-118">елигиблебутнотазуреаджоинедкаунт</span><span class="sxs-lookup"><span data-stu-id="21058-118">eligibleButNotAzureAdJoinedCount</span></span>|<span data-ttu-id="21058-119">Int32</span><span class="sxs-lookup"><span data-stu-id="21058-119">Int32</span></span>|<span data-ttu-id="21058-120">Количество устройств, подходящих для Co-Management, но еще не присоединенных к Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="21058-120">Count of devices eligible for Co-Management but not yet joined to Azure Active Directory</span></span>|
|<span data-ttu-id="21058-121">нидсосупдатекаунт</span><span class="sxs-lookup"><span data-stu-id="21058-121">needsOsUpdateCount</span></span>|<span data-ttu-id="21058-122">Int32</span><span class="sxs-lookup"><span data-stu-id="21058-122">Int32</span></span>|<span data-ttu-id="21058-123">Количество устройств, которые будут доступны Co-Management после обновления ОС</span><span class="sxs-lookup"><span data-stu-id="21058-123">Count of devices that will be eligible for Co-Management after an OS update</span></span>|
|<span data-ttu-id="21058-124">инелигиблекаунт</span><span class="sxs-lookup"><span data-stu-id="21058-124">ineligibleCount</span></span>|<span data-ttu-id="21058-125">Int32</span><span class="sxs-lookup"><span data-stu-id="21058-125">Int32</span></span>|<span data-ttu-id="21058-126">Количество устройств, доступных для Co-Management</span><span class="sxs-lookup"><span data-stu-id="21058-126">Count of devices ineligible for Co-Management</span></span>|

## <a name="relationships"></a><span data-ttu-id="21058-127">Связи</span><span class="sxs-lookup"><span data-stu-id="21058-127">Relationships</span></span>
<span data-ttu-id="21058-128">Нет</span><span class="sxs-lookup"><span data-stu-id="21058-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="21058-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="21058-129">JSON Representation</span></span>
<span data-ttu-id="21058-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="21058-130">Here is a JSON representation of the resource.</span></span>
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




