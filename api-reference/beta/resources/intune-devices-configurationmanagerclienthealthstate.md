---
title: Тип ресурса Конфигуратионманажерклиенсеалсстате
description: Состояние работоспособности клиента Configuration Manager
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b672eedb8b8efad168f59d54938322f81ef11977
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525140"
---
# <a name="configurationmanagerclienthealthstate-resource-type"></a><span data-ttu-id="82b1e-103">Тип ресурса Конфигуратионманажерклиенсеалсстате</span><span class="sxs-lookup"><span data-stu-id="82b1e-103">configurationManagerClientHealthState resource type</span></span>

<span data-ttu-id="82b1e-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="82b1e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="82b1e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82b1e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82b1e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="82b1e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82b1e-107">Состояние работоспособности клиента Configuration Manager</span><span class="sxs-lookup"><span data-stu-id="82b1e-107">Configuration manager client health state</span></span>

## <a name="properties"></a><span data-ttu-id="82b1e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="82b1e-108">Properties</span></span>
|<span data-ttu-id="82b1e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="82b1e-109">Property</span></span>|<span data-ttu-id="82b1e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="82b1e-110">Type</span></span>|<span data-ttu-id="82b1e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="82b1e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82b1e-112">state</span><span class="sxs-lookup"><span data-stu-id="82b1e-112">state</span></span>|[<span data-ttu-id="82b1e-113">configurationManagerClientState</span><span class="sxs-lookup"><span data-stu-id="82b1e-113">configurationManagerClientState</span></span>](../resources/intune-devices-configurationmanagerclientstate.md)|<span data-ttu-id="82b1e-114">Текущее состояние клиента Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="82b1e-114">Current configuration manager client state.</span></span> <span data-ttu-id="82b1e-115">Возможные значения: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.</span><span class="sxs-lookup"><span data-stu-id="82b1e-115">Possible values are: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.</span></span>|
|<span data-ttu-id="82b1e-116">errorCode</span><span class="sxs-lookup"><span data-stu-id="82b1e-116">errorCode</span></span>|<span data-ttu-id="82b1e-117">Int32</span><span class="sxs-lookup"><span data-stu-id="82b1e-117">Int32</span></span>|<span data-ttu-id="82b1e-118">Код ошибки для состояния сбоя.</span><span class="sxs-lookup"><span data-stu-id="82b1e-118">Error code for failed state.</span></span>|
|<span data-ttu-id="82b1e-119">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="82b1e-119">lastSyncDateTime</span></span>|<span data-ttu-id="82b1e-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82b1e-120">DateTimeOffset</span></span>|<span data-ttu-id="82b1e-121">Дата и время последней синхронизации с точкой управления Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="82b1e-121">Datetime fo last sync with configuration manager management point.</span></span>|

## <a name="relationships"></a><span data-ttu-id="82b1e-122">Связи</span><span class="sxs-lookup"><span data-stu-id="82b1e-122">Relationships</span></span>
<span data-ttu-id="82b1e-123">Нет</span><span class="sxs-lookup"><span data-stu-id="82b1e-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="82b1e-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="82b1e-124">JSON Representation</span></span>
<span data-ttu-id="82b1e-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="82b1e-125">Here is a JSON representation of the resource.</span></span>
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



