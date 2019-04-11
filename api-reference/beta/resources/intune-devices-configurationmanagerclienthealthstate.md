---
title: Тип ресурса Конфигуратионманажерклиенсеалсстате
description: Состояние работоспособности клиента Configuration Manager
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e2a04b8cf7520425527e118fcc9db00461c4edda
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31797741"
---
# <a name="configurationmanagerclienthealthstate-resource-type"></a><span data-ttu-id="c0255-103">Тип ресурса Конфигуратионманажерклиенсеалсстате</span><span class="sxs-lookup"><span data-stu-id="c0255-103">configurationManagerClientHealthState resource type</span></span>

> <span data-ttu-id="c0255-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0255-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0255-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c0255-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0255-106">Состояние работоспособности клиента Configuration Manager</span><span class="sxs-lookup"><span data-stu-id="c0255-106">Configuration manager client health state</span></span>

## <a name="properties"></a><span data-ttu-id="c0255-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c0255-107">Properties</span></span>
|<span data-ttu-id="c0255-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c0255-108">Property</span></span>|<span data-ttu-id="c0255-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c0255-109">Type</span></span>|<span data-ttu-id="c0255-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c0255-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0255-111">state</span><span class="sxs-lookup"><span data-stu-id="c0255-111">state</span></span>|[<span data-ttu-id="c0255-112">configurationManagerClientState</span><span class="sxs-lookup"><span data-stu-id="c0255-112">configurationManagerClientState</span></span>](../resources/intune-devices-configurationmanagerclientstate.md)|<span data-ttu-id="c0255-113">Текущее состояние клиента Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="c0255-113">Current configuration manager client state.</span></span> <span data-ttu-id="c0255-114">Возможные значения: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.</span><span class="sxs-lookup"><span data-stu-id="c0255-114">Possible values are: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.</span></span>|
|<span data-ttu-id="c0255-115">errorCode</span><span class="sxs-lookup"><span data-stu-id="c0255-115">errorCode</span></span>|<span data-ttu-id="c0255-116">Int32</span><span class="sxs-lookup"><span data-stu-id="c0255-116">Int32</span></span>|<span data-ttu-id="c0255-117">Код ошибки для состояния сбоя.</span><span class="sxs-lookup"><span data-stu-id="c0255-117">Error code for failed state.</span></span>|
|<span data-ttu-id="c0255-118">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="c0255-118">lastSyncDateTime</span></span>|<span data-ttu-id="c0255-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0255-119">DateTimeOffset</span></span>|<span data-ttu-id="c0255-120">Дата и время последней синхронизации с точкой управления Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="c0255-120">Datetime fo last sync with configuration manager management point.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c0255-121">Отношения</span><span class="sxs-lookup"><span data-stu-id="c0255-121">Relationships</span></span>
<span data-ttu-id="c0255-122">Нет</span><span class="sxs-lookup"><span data-stu-id="c0255-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c0255-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c0255-123">JSON Representation</span></span>
<span data-ttu-id="c0255-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c0255-124">Here is a JSON representation of the resource.</span></span>
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





