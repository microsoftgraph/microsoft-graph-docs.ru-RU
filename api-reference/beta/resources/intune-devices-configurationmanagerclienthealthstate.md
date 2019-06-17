---
title: Тип ресурса Конфигуратионманажерклиенсеалсстате
description: Состояние работоспособности клиента Configuration Manager
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 618282f2a061ec8327ff93d1af441e088523260b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983241"
---
# <a name="configurationmanagerclienthealthstate-resource-type"></a><span data-ttu-id="d76d7-103">Тип ресурса Конфигуратионманажерклиенсеалсстате</span><span class="sxs-lookup"><span data-stu-id="d76d7-103">configurationManagerClientHealthState resource type</span></span>

> <span data-ttu-id="d76d7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d76d7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d76d7-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d76d7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d76d7-106">Состояние работоспособности клиента Configuration Manager</span><span class="sxs-lookup"><span data-stu-id="d76d7-106">Configuration manager client health state</span></span>

## <a name="properties"></a><span data-ttu-id="d76d7-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d76d7-107">Properties</span></span>
|<span data-ttu-id="d76d7-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d76d7-108">Property</span></span>|<span data-ttu-id="d76d7-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d76d7-109">Type</span></span>|<span data-ttu-id="d76d7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d76d7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d76d7-111">state</span><span class="sxs-lookup"><span data-stu-id="d76d7-111">state</span></span>|[<span data-ttu-id="d76d7-112">configurationManagerClientState</span><span class="sxs-lookup"><span data-stu-id="d76d7-112">configurationManagerClientState</span></span>](../resources/intune-devices-configurationmanagerclientstate.md)|<span data-ttu-id="d76d7-113">Текущее состояние клиента Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="d76d7-113">Current configuration manager client state.</span></span> <span data-ttu-id="d76d7-114">Возможные значения: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.</span><span class="sxs-lookup"><span data-stu-id="d76d7-114">Possible values are: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.</span></span>|
|<span data-ttu-id="d76d7-115">errorCode</span><span class="sxs-lookup"><span data-stu-id="d76d7-115">errorCode</span></span>|<span data-ttu-id="d76d7-116">Int32</span><span class="sxs-lookup"><span data-stu-id="d76d7-116">Int32</span></span>|<span data-ttu-id="d76d7-117">Код ошибки для состояния сбоя.</span><span class="sxs-lookup"><span data-stu-id="d76d7-117">Error code for failed state.</span></span>|
|<span data-ttu-id="d76d7-118">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="d76d7-118">lastSyncDateTime</span></span>|<span data-ttu-id="d76d7-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d76d7-119">DateTimeOffset</span></span>|<span data-ttu-id="d76d7-120">Дата и время последней синхронизации с точкой управления Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="d76d7-120">Datetime fo last sync with configuration manager management point.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d76d7-121">Отношения</span><span class="sxs-lookup"><span data-stu-id="d76d7-121">Relationships</span></span>
<span data-ttu-id="d76d7-122">Нет</span><span class="sxs-lookup"><span data-stu-id="d76d7-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d76d7-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d76d7-123">JSON Representation</span></span>
<span data-ttu-id="d76d7-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d76d7-124">Here is a JSON representation of the resource.</span></span>
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





