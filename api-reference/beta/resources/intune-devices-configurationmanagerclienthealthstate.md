---
title: Тип ресурса configurationManagerClientHealthState
description: Состояние работоспособности клиента диспетчер конфигурации
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 55ba2b24df0d1d4c278f4785a310237c9c32cd9b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425829"
---
# <a name="configurationmanagerclienthealthstate-resource-type"></a><span data-ttu-id="d377e-103">Тип ресурса configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="d377e-103">configurationManagerClientHealthState resource type</span></span>

> <span data-ttu-id="d377e-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d377e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d377e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d377e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d377e-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d377e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d377e-107">Состояние работоспособности клиента диспетчер конфигурации</span><span class="sxs-lookup"><span data-stu-id="d377e-107">Configuration manager client health state</span></span>

## <a name="properties"></a><span data-ttu-id="d377e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d377e-108">Properties</span></span>
|<span data-ttu-id="d377e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d377e-109">Property</span></span>|<span data-ttu-id="d377e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d377e-110">Type</span></span>|<span data-ttu-id="d377e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d377e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d377e-112">state</span><span class="sxs-lookup"><span data-stu-id="d377e-112">state</span></span>|[<span data-ttu-id="d377e-113">configurationManagerClientState</span><span class="sxs-lookup"><span data-stu-id="d377e-113">configurationManagerClientState</span></span>](../resources/intune-devices-configurationmanagerclientstate.md)|<span data-ttu-id="d377e-114">Текущее состояние клиента диспетчер конфигурации.</span><span class="sxs-lookup"><span data-stu-id="d377e-114">Current configuration manager client state.</span></span> <span data-ttu-id="d377e-115">Возможные значения: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.</span><span class="sxs-lookup"><span data-stu-id="d377e-115">Possible values are: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.</span></span>|
|<span data-ttu-id="d377e-116">errorCode</span><span class="sxs-lookup"><span data-stu-id="d377e-116">errorCode</span></span>|<span data-ttu-id="d377e-117">Int32</span><span class="sxs-lookup"><span data-stu-id="d377e-117">Int32</span></span>|<span data-ttu-id="d377e-118">Код ошибки для неудачных состояния.</span><span class="sxs-lookup"><span data-stu-id="d377e-118">Error code for failed state.</span></span>|
|<span data-ttu-id="d377e-119">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="d377e-119">lastSyncDateTime</span></span>|<span data-ttu-id="d377e-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d377e-120">DateTimeOffset</span></span>|<span data-ttu-id="d377e-121">Выберите пункт опубликованные даты и времени последней синхронизации с помощью диспетчера управления конфигурацией.</span><span class="sxs-lookup"><span data-stu-id="d377e-121">Datetime fo last sync with configuration manager management point.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d377e-122">Отношения</span><span class="sxs-lookup"><span data-stu-id="d377e-122">Relationships</span></span>
<span data-ttu-id="d377e-123">Нет</span><span class="sxs-lookup"><span data-stu-id="d377e-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d377e-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d377e-124">JSON Representation</span></span>
<span data-ttu-id="d377e-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d377e-125">Here is a JSON representation of the resource.</span></span>
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




