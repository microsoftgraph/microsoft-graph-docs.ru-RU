---
title: Тип ресурса configurationManagerClientHealthState
description: Состояние работоспособности клиента диспетчер конфигурации
author: tfitzmac
ms.openlocfilehash: 8361d74f675cf1eaf70b78e2350aae2fc6e83554
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302788"
---
# <a name="configurationmanagerclienthealthstate-resource-type"></a><span data-ttu-id="2eb08-103">Тип ресурса configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="2eb08-103">configurationManagerClientHealthState resource type</span></span>

> <span data-ttu-id="2eb08-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2eb08-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2eb08-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2eb08-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2eb08-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2eb08-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2eb08-107">Состояние работоспособности клиента диспетчер конфигурации</span><span class="sxs-lookup"><span data-stu-id="2eb08-107">Configuration manager client health state</span></span>
## <a name="properties"></a><span data-ttu-id="2eb08-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="2eb08-108">Properties</span></span>
|<span data-ttu-id="2eb08-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="2eb08-109">Property</span></span>|<span data-ttu-id="2eb08-110">Тип</span><span class="sxs-lookup"><span data-stu-id="2eb08-110">Type</span></span>|<span data-ttu-id="2eb08-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2eb08-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2eb08-112">state</span><span class="sxs-lookup"><span data-stu-id="2eb08-112">state</span></span>|[<span data-ttu-id="2eb08-113">configurationManagerClientState</span><span class="sxs-lookup"><span data-stu-id="2eb08-113">configurationManagerClientState</span></span>](../resources/intune-devices-configurationmanagerclientstate.md)|<span data-ttu-id="2eb08-114">Текущее состояние клиента диспетчер конфигурации.</span><span class="sxs-lookup"><span data-stu-id="2eb08-114">Current configuration manager client state.</span></span> <span data-ttu-id="2eb08-115">Возможные значения: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.</span><span class="sxs-lookup"><span data-stu-id="2eb08-115">Possible values are: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.</span></span>|
|<span data-ttu-id="2eb08-116">errorCode</span><span class="sxs-lookup"><span data-stu-id="2eb08-116">errorCode</span></span>|<span data-ttu-id="2eb08-117">Int32</span><span class="sxs-lookup"><span data-stu-id="2eb08-117">Int32</span></span>|<span data-ttu-id="2eb08-118">Код ошибки для неудачных состояния.</span><span class="sxs-lookup"><span data-stu-id="2eb08-118">Error code for failed state.</span></span>|
|<span data-ttu-id="2eb08-119">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="2eb08-119">lastSyncDateTime</span></span>|<span data-ttu-id="2eb08-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2eb08-120">DateTimeOffset</span></span>|<span data-ttu-id="2eb08-121">Выберите пункт опубликованные даты и времени последней синхронизации с помощью диспетчера управления конфигурацией.</span><span class="sxs-lookup"><span data-stu-id="2eb08-121">Datetime fo last sync with configuration manager management point.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2eb08-122">Связи</span><span class="sxs-lookup"><span data-stu-id="2eb08-122">Relationships</span></span>
<span data-ttu-id="2eb08-123">Нет</span><span class="sxs-lookup"><span data-stu-id="2eb08-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2eb08-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2eb08-124">JSON Representation</span></span>
<span data-ttu-id="2eb08-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2eb08-125">Here is a JSON representation of the resource.</span></span>
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





