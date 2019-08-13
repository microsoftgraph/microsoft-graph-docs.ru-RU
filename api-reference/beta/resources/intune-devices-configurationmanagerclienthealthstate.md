---
title: Тип ресурса Конфигуратионманажерклиенсеалсстате
description: Состояние работоспособности клиента Configuration Manager
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ab1b47ac9371c0a0806ff03e18bf9cc7eed577f0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369467"
---
# <a name="configurationmanagerclienthealthstate-resource-type"></a><span data-ttu-id="491be-103">Тип ресурса Конфигуратионманажерклиенсеалсстате</span><span class="sxs-lookup"><span data-stu-id="491be-103">configurationManagerClientHealthState resource type</span></span>

> <span data-ttu-id="491be-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="491be-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="491be-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="491be-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="491be-106">Состояние работоспособности клиента Configuration Manager</span><span class="sxs-lookup"><span data-stu-id="491be-106">Configuration manager client health state</span></span>

## <a name="properties"></a><span data-ttu-id="491be-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="491be-107">Properties</span></span>
|<span data-ttu-id="491be-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="491be-108">Property</span></span>|<span data-ttu-id="491be-109">Тип</span><span class="sxs-lookup"><span data-stu-id="491be-109">Type</span></span>|<span data-ttu-id="491be-110">Описание</span><span class="sxs-lookup"><span data-stu-id="491be-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="491be-111">state</span><span class="sxs-lookup"><span data-stu-id="491be-111">state</span></span>|[<span data-ttu-id="491be-112">configurationManagerClientState</span><span class="sxs-lookup"><span data-stu-id="491be-112">configurationManagerClientState</span></span>](../resources/intune-devices-configurationmanagerclientstate.md)|<span data-ttu-id="491be-113">Текущее состояние клиента Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="491be-113">Current configuration manager client state.</span></span> <span data-ttu-id="491be-114">Возможные значения: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.</span><span class="sxs-lookup"><span data-stu-id="491be-114">Possible values are: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.</span></span>|
|<span data-ttu-id="491be-115">errorCode</span><span class="sxs-lookup"><span data-stu-id="491be-115">errorCode</span></span>|<span data-ttu-id="491be-116">Int32</span><span class="sxs-lookup"><span data-stu-id="491be-116">Int32</span></span>|<span data-ttu-id="491be-117">Код ошибки для состояния сбоя.</span><span class="sxs-lookup"><span data-stu-id="491be-117">Error code for failed state.</span></span>|
|<span data-ttu-id="491be-118">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="491be-118">lastSyncDateTime</span></span>|<span data-ttu-id="491be-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="491be-119">DateTimeOffset</span></span>|<span data-ttu-id="491be-120">Дата и время последней синхронизации с точкой управления Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="491be-120">Datetime fo last sync with configuration manager management point.</span></span>|

## <a name="relationships"></a><span data-ttu-id="491be-121">Отношения</span><span class="sxs-lookup"><span data-stu-id="491be-121">Relationships</span></span>
<span data-ttu-id="491be-122">Нет</span><span class="sxs-lookup"><span data-stu-id="491be-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="491be-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="491be-123">JSON Representation</span></span>
<span data-ttu-id="491be-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="491be-124">Here is a JSON representation of the resource.</span></span>
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



