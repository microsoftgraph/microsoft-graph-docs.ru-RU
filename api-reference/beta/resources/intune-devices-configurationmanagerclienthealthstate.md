---
title: Тип ресурса Конфигуратионманажерклиенсеалсстате
description: Состояние работоспособности клиента Configuration Manager
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b43419ee34747c154663d45c137ef19ca5ed4126
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785065"
---
# <a name="configurationmanagerclienthealthstate-resource-type"></a><span data-ttu-id="ceb4d-103">Тип ресурса Конфигуратионманажерклиенсеалсстате</span><span class="sxs-lookup"><span data-stu-id="ceb4d-103">configurationManagerClientHealthState resource type</span></span>

> <span data-ttu-id="ceb4d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ceb4d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ceb4d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ceb4d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ceb4d-106">Состояние работоспособности клиента Configuration Manager</span><span class="sxs-lookup"><span data-stu-id="ceb4d-106">Configuration manager client health state</span></span>

## <a name="properties"></a><span data-ttu-id="ceb4d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ceb4d-107">Properties</span></span>
|<span data-ttu-id="ceb4d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ceb4d-108">Property</span></span>|<span data-ttu-id="ceb4d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ceb4d-109">Type</span></span>|<span data-ttu-id="ceb4d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ceb4d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ceb4d-111">state</span><span class="sxs-lookup"><span data-stu-id="ceb4d-111">state</span></span>|[<span data-ttu-id="ceb4d-112">configurationManagerClientState</span><span class="sxs-lookup"><span data-stu-id="ceb4d-112">configurationManagerClientState</span></span>](../resources/intune-devices-configurationmanagerclientstate.md)|<span data-ttu-id="ceb4d-113">Текущее состояние клиента Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="ceb4d-113">Current configuration manager client state.</span></span> <span data-ttu-id="ceb4d-114">Возможные значения: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.</span><span class="sxs-lookup"><span data-stu-id="ceb4d-114">Possible values are: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.</span></span>|
|<span data-ttu-id="ceb4d-115">errorCode</span><span class="sxs-lookup"><span data-stu-id="ceb4d-115">errorCode</span></span>|<span data-ttu-id="ceb4d-116">Int32</span><span class="sxs-lookup"><span data-stu-id="ceb4d-116">Int32</span></span>|<span data-ttu-id="ceb4d-117">Код ошибки для состояния сбоя.</span><span class="sxs-lookup"><span data-stu-id="ceb4d-117">Error code for failed state.</span></span>|
|<span data-ttu-id="ceb4d-118">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="ceb4d-118">lastSyncDateTime</span></span>|<span data-ttu-id="ceb4d-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ceb4d-119">DateTimeOffset</span></span>|<span data-ttu-id="ceb4d-120">Дата и время последней синхронизации с точкой управления Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="ceb4d-120">Datetime for last sync with configuration manager management point.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ceb4d-121">Связи</span><span class="sxs-lookup"><span data-stu-id="ceb4d-121">Relationships</span></span>
<span data-ttu-id="ceb4d-122">Нет</span><span class="sxs-lookup"><span data-stu-id="ceb4d-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ceb4d-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ceb4d-123">JSON Representation</span></span>
<span data-ttu-id="ceb4d-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ceb4d-124">Here is a JSON representation of the resource.</span></span>
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



