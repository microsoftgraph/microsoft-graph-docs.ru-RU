---
title: Тип ресурса Конфигуратионманажерклиенсеалсстате
description: Состояние работоспособности клиента Configuration Manager
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9356a4aac345137ba93dc85914ddc1a12e44233f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35968556"
---
# <a name="configurationmanagerclienthealthstate-resource-type"></a><span data-ttu-id="1bf1e-103">Тип ресурса Конфигуратионманажерклиенсеалсстате</span><span class="sxs-lookup"><span data-stu-id="1bf1e-103">configurationManagerClientHealthState resource type</span></span>

> <span data-ttu-id="1bf1e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1bf1e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1bf1e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1bf1e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1bf1e-106">Состояние работоспособности клиента Configuration Manager</span><span class="sxs-lookup"><span data-stu-id="1bf1e-106">Configuration manager client health state</span></span>

## <a name="properties"></a><span data-ttu-id="1bf1e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1bf1e-107">Properties</span></span>
|<span data-ttu-id="1bf1e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1bf1e-108">Property</span></span>|<span data-ttu-id="1bf1e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1bf1e-109">Type</span></span>|<span data-ttu-id="1bf1e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1bf1e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1bf1e-111">state</span><span class="sxs-lookup"><span data-stu-id="1bf1e-111">state</span></span>|[<span data-ttu-id="1bf1e-112">configurationManagerClientState</span><span class="sxs-lookup"><span data-stu-id="1bf1e-112">configurationManagerClientState</span></span>](../resources/intune-devices-configurationmanagerclientstate.md)|<span data-ttu-id="1bf1e-113">Текущее состояние клиента Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="1bf1e-113">Current configuration manager client state.</span></span> <span data-ttu-id="1bf1e-114">Возможные значения: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.</span><span class="sxs-lookup"><span data-stu-id="1bf1e-114">Possible values are: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.</span></span>|
|<span data-ttu-id="1bf1e-115">errorCode</span><span class="sxs-lookup"><span data-stu-id="1bf1e-115">errorCode</span></span>|<span data-ttu-id="1bf1e-116">Int32</span><span class="sxs-lookup"><span data-stu-id="1bf1e-116">Int32</span></span>|<span data-ttu-id="1bf1e-117">Код ошибки для состояния сбоя.</span><span class="sxs-lookup"><span data-stu-id="1bf1e-117">Error code for failed state.</span></span>|
|<span data-ttu-id="1bf1e-118">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="1bf1e-118">lastSyncDateTime</span></span>|<span data-ttu-id="1bf1e-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1bf1e-119">DateTimeOffset</span></span>|<span data-ttu-id="1bf1e-120">Дата и время последней синхронизации с точкой управления Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="1bf1e-120">Datetime fo last sync with configuration manager management point.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1bf1e-121">Отношения</span><span class="sxs-lookup"><span data-stu-id="1bf1e-121">Relationships</span></span>
<span data-ttu-id="1bf1e-122">Нет</span><span class="sxs-lookup"><span data-stu-id="1bf1e-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1bf1e-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1bf1e-123">JSON Representation</span></span>
<span data-ttu-id="1bf1e-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1bf1e-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerClientHealthState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerClientHealthState",
  "state": "String",
  "errorCode": 1024,
  "lastSyncDateTime": "String (timestamp)"
}
```





