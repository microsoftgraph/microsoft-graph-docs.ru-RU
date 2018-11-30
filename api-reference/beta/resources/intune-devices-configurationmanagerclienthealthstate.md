---
title: Тип ресурса configurationManagerClientHealthState
description: Состояние работоспособности клиента диспетчер конфигурации
ms.openlocfilehash: f2724f5d230ee539720e105daf1758bf727bee26
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076186"
---
# <a name="configurationmanagerclienthealthstate-resource-type"></a><span data-ttu-id="b3fa2-103">Тип ресурса configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="b3fa2-103">configurationManagerClientHealthState resource type</span></span>

> <span data-ttu-id="b3fa2-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b3fa2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b3fa2-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b3fa2-107">Состояние работоспособности клиента диспетчер конфигурации</span><span class="sxs-lookup"><span data-stu-id="b3fa2-107">Configuration manager client health state</span></span>
## <a name="properties"></a><span data-ttu-id="b3fa2-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b3fa2-108">Properties</span></span>
|<span data-ttu-id="b3fa2-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b3fa2-109">Property</span></span>|<span data-ttu-id="b3fa2-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b3fa2-110">Type</span></span>|<span data-ttu-id="b3fa2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b3fa2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3fa2-112">state</span><span class="sxs-lookup"><span data-stu-id="b3fa2-112">state</span></span>|[<span data-ttu-id="b3fa2-113">configurationManagerClientState</span><span class="sxs-lookup"><span data-stu-id="b3fa2-113">configurationManagerClientState</span></span>](../resources/intune-devices-configurationmanagerclientstate.md)|<span data-ttu-id="b3fa2-114">Текущее состояние клиента диспетчер конфигурации.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-114">Current configuration manager client state.</span></span> <span data-ttu-id="b3fa2-115">Возможные значения: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-115">Possible values are: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.</span></span>|
|<span data-ttu-id="b3fa2-116">errorCode</span><span class="sxs-lookup"><span data-stu-id="b3fa2-116">errorCode</span></span>|<span data-ttu-id="b3fa2-117">Int32</span><span class="sxs-lookup"><span data-stu-id="b3fa2-117">Int32</span></span>|<span data-ttu-id="b3fa2-118">Код ошибки для неудачных состояния.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-118">Error code for failed state.</span></span>|
|<span data-ttu-id="b3fa2-119">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="b3fa2-119">lastSyncDateTime</span></span>|<span data-ttu-id="b3fa2-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3fa2-120">DateTimeOffset</span></span>|<span data-ttu-id="b3fa2-121">Выберите пункт опубликованные даты и времени последней синхронизации с помощью диспетчера управления конфигурацией.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-121">Datetime fo last sync with configuration manager management point.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b3fa2-122">Связи</span><span class="sxs-lookup"><span data-stu-id="b3fa2-122">Relationships</span></span>
<span data-ttu-id="b3fa2-123">Нет</span><span class="sxs-lookup"><span data-stu-id="b3fa2-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b3fa2-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b3fa2-124">JSON Representation</span></span>
<span data-ttu-id="b3fa2-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-125">Here is a JSON representation of the resource.</span></span>
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





