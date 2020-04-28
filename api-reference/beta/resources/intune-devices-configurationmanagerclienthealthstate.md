---
title: Тип ресурса Конфигуратионманажерклиенсеалсстате
description: Состояние работоспособности клиента Configuration Manager
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1c1c707d118b666f52e8a898cd0ad258c5cc8308
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465039"
---
# <a name="configurationmanagerclienthealthstate-resource-type"></a><span data-ttu-id="83366-103">Тип ресурса Конфигуратионманажерклиенсеалсстате</span><span class="sxs-lookup"><span data-stu-id="83366-103">configurationManagerClientHealthState resource type</span></span>

<span data-ttu-id="83366-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83366-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="83366-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83366-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83366-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="83366-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83366-107">Состояние работоспособности клиента Configuration Manager</span><span class="sxs-lookup"><span data-stu-id="83366-107">Configuration manager client health state</span></span>

## <a name="properties"></a><span data-ttu-id="83366-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="83366-108">Properties</span></span>
|<span data-ttu-id="83366-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="83366-109">Property</span></span>|<span data-ttu-id="83366-110">Тип</span><span class="sxs-lookup"><span data-stu-id="83366-110">Type</span></span>|<span data-ttu-id="83366-111">Описание</span><span class="sxs-lookup"><span data-stu-id="83366-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83366-112">state</span><span class="sxs-lookup"><span data-stu-id="83366-112">state</span></span>|[<span data-ttu-id="83366-113">configurationManagerClientState</span><span class="sxs-lookup"><span data-stu-id="83366-113">configurationManagerClientState</span></span>](../resources/intune-devices-configurationmanagerclientstate.md)|<span data-ttu-id="83366-114">Текущее состояние клиента Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="83366-114">Current configuration manager client state.</span></span> <span data-ttu-id="83366-115">Возможные значения: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.</span><span class="sxs-lookup"><span data-stu-id="83366-115">Possible values are: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.</span></span>|
|<span data-ttu-id="83366-116">errorCode</span><span class="sxs-lookup"><span data-stu-id="83366-116">errorCode</span></span>|<span data-ttu-id="83366-117">Int32</span><span class="sxs-lookup"><span data-stu-id="83366-117">Int32</span></span>|<span data-ttu-id="83366-118">Код ошибки для состояния сбоя.</span><span class="sxs-lookup"><span data-stu-id="83366-118">Error code for failed state.</span></span>|
|<span data-ttu-id="83366-119">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="83366-119">lastSyncDateTime</span></span>|<span data-ttu-id="83366-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83366-120">DateTimeOffset</span></span>|<span data-ttu-id="83366-121">Дата и время последней синхронизации с точкой управления Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="83366-121">Datetime for last sync with configuration manager management point.</span></span>|

## <a name="relationships"></a><span data-ttu-id="83366-122">Связи</span><span class="sxs-lookup"><span data-stu-id="83366-122">Relationships</span></span>
<span data-ttu-id="83366-123">Нет</span><span class="sxs-lookup"><span data-stu-id="83366-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="83366-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="83366-124">JSON Representation</span></span>
<span data-ttu-id="83366-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="83366-125">Here is a JSON representation of the resource.</span></span>
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



