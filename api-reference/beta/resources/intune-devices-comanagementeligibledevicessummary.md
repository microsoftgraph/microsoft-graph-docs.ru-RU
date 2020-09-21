---
title: Тип ресурса Команажементелигибледевицессуммари
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b67734bf98a48c31a1346bd730c8521fd8a8d681
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060771"
---
# <a name="comanagementeligibledevicessummary-resource-type"></a><span data-ttu-id="1f283-103">Тип ресурса Команажементелигибледевицессуммари</span><span class="sxs-lookup"><span data-stu-id="1f283-103">comanagementEligibleDevicesSummary resource type</span></span>

<span data-ttu-id="1f283-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f283-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1f283-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f283-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1f283-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1f283-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f283-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="1f283-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="1f283-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="1f283-108">Properties</span></span>
|<span data-ttu-id="1f283-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="1f283-109">Property</span></span>|<span data-ttu-id="1f283-110">Тип</span><span class="sxs-lookup"><span data-stu-id="1f283-110">Type</span></span>|<span data-ttu-id="1f283-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1f283-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f283-112">команажедкаунт</span><span class="sxs-lookup"><span data-stu-id="1f283-112">comanagedCount</span></span>|<span data-ttu-id="1f283-113">Int32</span><span class="sxs-lookup"><span data-stu-id="1f283-113">Int32</span></span>|<span data-ttu-id="1f283-114">Количество устройств, для которых уже осуществляется совместное управление</span><span class="sxs-lookup"><span data-stu-id="1f283-114">Count of devices already Co-Managed</span></span>|
|<span data-ttu-id="1f283-115">елигиблекаунт</span><span class="sxs-lookup"><span data-stu-id="1f283-115">eligibleCount</span></span>|<span data-ttu-id="1f283-116">Int32</span><span class="sxs-lookup"><span data-stu-id="1f283-116">Int32</span></span>|<span data-ttu-id="1f283-117">Количество устройств, полностью доступных для совместного управления</span><span class="sxs-lookup"><span data-stu-id="1f283-117">Count of devices fully eligible for Co-Management</span></span>|
|<span data-ttu-id="1f283-118">елигиблебутнотазуреаджоинедкаунт</span><span class="sxs-lookup"><span data-stu-id="1f283-118">eligibleButNotAzureAdJoinedCount</span></span>|<span data-ttu-id="1f283-119">Int32</span><span class="sxs-lookup"><span data-stu-id="1f283-119">Int32</span></span>|<span data-ttu-id="1f283-120">Количество устройств, подходящих для совместного управления, но еще не включенных в Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="1f283-120">Count of devices eligible for Co-Management but not yet joined to Azure Active Directory</span></span>|
|<span data-ttu-id="1f283-121">нидсосупдатекаунт</span><span class="sxs-lookup"><span data-stu-id="1f283-121">needsOsUpdateCount</span></span>|<span data-ttu-id="1f283-122">Int32</span><span class="sxs-lookup"><span data-stu-id="1f283-122">Int32</span></span>|<span data-ttu-id="1f283-123">Количество устройств, которые будут доступны для совместного управления после обновления ОС</span><span class="sxs-lookup"><span data-stu-id="1f283-123">Count of devices that will be eligible for Co-Management after an OS update</span></span>|
|<span data-ttu-id="1f283-124">инелигиблекаунт</span><span class="sxs-lookup"><span data-stu-id="1f283-124">ineligibleCount</span></span>|<span data-ttu-id="1f283-125">Int32</span><span class="sxs-lookup"><span data-stu-id="1f283-125">Int32</span></span>|<span data-ttu-id="1f283-126">Количество устройств, подходящих для совместного управления</span><span class="sxs-lookup"><span data-stu-id="1f283-126">Count of devices ineligible for Co-Management</span></span>|

## <a name="relationships"></a><span data-ttu-id="1f283-127">Связи</span><span class="sxs-lookup"><span data-stu-id="1f283-127">Relationships</span></span>
<span data-ttu-id="1f283-128">Нет</span><span class="sxs-lookup"><span data-stu-id="1f283-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1f283-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1f283-129">JSON Representation</span></span>
<span data-ttu-id="1f283-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1f283-130">Here is a JSON representation of the resource.</span></span>
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






