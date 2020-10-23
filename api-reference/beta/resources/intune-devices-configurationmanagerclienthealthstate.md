---
title: Тип ресурса Конфигуратионманажерклиенсеалсстате
description: Состояние работоспособности клиента Configuration Manager
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f860dd86f596983975a44762fcb5168b29bf84bf
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48690268"
---
# <a name="configurationmanagerclienthealthstate-resource-type"></a><span data-ttu-id="8d3b1-103">Тип ресурса Конфигуратионманажерклиенсеалсстате</span><span class="sxs-lookup"><span data-stu-id="8d3b1-103">configurationManagerClientHealthState resource type</span></span>

<span data-ttu-id="8d3b1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d3b1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8d3b1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d3b1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d3b1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8d3b1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d3b1-107">Состояние работоспособности клиента Configuration Manager</span><span class="sxs-lookup"><span data-stu-id="8d3b1-107">Configuration manager client health state</span></span>

## <a name="properties"></a><span data-ttu-id="8d3b1-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="8d3b1-108">Properties</span></span>
|<span data-ttu-id="8d3b1-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="8d3b1-109">Property</span></span>|<span data-ttu-id="8d3b1-110">Тип</span><span class="sxs-lookup"><span data-stu-id="8d3b1-110">Type</span></span>|<span data-ttu-id="8d3b1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8d3b1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d3b1-112">state</span><span class="sxs-lookup"><span data-stu-id="8d3b1-112">state</span></span>|[<span data-ttu-id="8d3b1-113">configurationManagerClientState</span><span class="sxs-lookup"><span data-stu-id="8d3b1-113">configurationManagerClientState</span></span>](../resources/intune-devices-configurationmanagerclientstate.md)|<span data-ttu-id="8d3b1-114">Текущее состояние клиента Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="8d3b1-114">Current configuration manager client state.</span></span> <span data-ttu-id="8d3b1-115">Возможные значения: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.</span><span class="sxs-lookup"><span data-stu-id="8d3b1-115">Possible values are: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.</span></span>|
|<span data-ttu-id="8d3b1-116">errorCode</span><span class="sxs-lookup"><span data-stu-id="8d3b1-116">errorCode</span></span>|<span data-ttu-id="8d3b1-117">Int32</span><span class="sxs-lookup"><span data-stu-id="8d3b1-117">Int32</span></span>|<span data-ttu-id="8d3b1-118">Код ошибки для состояния сбоя.</span><span class="sxs-lookup"><span data-stu-id="8d3b1-118">Error code for failed state.</span></span>|
|<span data-ttu-id="8d3b1-119">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="8d3b1-119">lastSyncDateTime</span></span>|<span data-ttu-id="8d3b1-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d3b1-120">DateTimeOffset</span></span>|<span data-ttu-id="8d3b1-121">Дата и время последней синхронизации с точкой управления Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="8d3b1-121">Datetime for last sync with configuration manager management point.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8d3b1-122">Связи</span><span class="sxs-lookup"><span data-stu-id="8d3b1-122">Relationships</span></span>
<span data-ttu-id="8d3b1-123">Нет</span><span class="sxs-lookup"><span data-stu-id="8d3b1-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8d3b1-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8d3b1-124">JSON Representation</span></span>
<span data-ttu-id="8d3b1-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8d3b1-125">Here is a JSON representation of the resource.</span></span>
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





