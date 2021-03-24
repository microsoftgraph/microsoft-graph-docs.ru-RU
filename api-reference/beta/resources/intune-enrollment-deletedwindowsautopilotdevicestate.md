---
title: удаленный тип ресурсаWindowsAutopilotDeviceState
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 87113449f0c00722f3aa1d3a1e614873524d43a6
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146818"
---
# <a name="deletedwindowsautopilotdevicestate-resource-type"></a><span data-ttu-id="1bc87-103">удаленный тип ресурсаWindowsAutopilotDeviceState</span><span class="sxs-lookup"><span data-stu-id="1bc87-103">deletedWindowsAutopilotDeviceState resource type</span></span>

<span data-ttu-id="1bc87-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1bc87-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1bc87-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1bc87-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1bc87-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1bc87-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1bc87-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="1bc87-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="1bc87-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="1bc87-108">Properties</span></span>
|<span data-ttu-id="1bc87-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="1bc87-109">Property</span></span>|<span data-ttu-id="1bc87-110">Тип</span><span class="sxs-lookup"><span data-stu-id="1bc87-110">Type</span></span>|<span data-ttu-id="1bc87-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1bc87-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1bc87-112">serialNumber</span><span class="sxs-lookup"><span data-stu-id="1bc87-112">serialNumber</span></span>|<span data-ttu-id="1bc87-113">String</span><span class="sxs-lookup"><span data-stu-id="1bc87-113">String</span></span>|<span data-ttu-id="1bc87-114">Серийный номер устройства автопилота</span><span class="sxs-lookup"><span data-stu-id="1bc87-114">Autopilot Device Serial Number</span></span>|
|<span data-ttu-id="1bc87-115">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="1bc87-115">deviceRegistrationId</span></span>|<span data-ttu-id="1bc87-116">Строка</span><span class="sxs-lookup"><span data-stu-id="1bc87-116">String</span></span>|<span data-ttu-id="1bc87-117">Регистрационный номер устройства ZTD .</span><span class="sxs-lookup"><span data-stu-id="1bc87-117">ZTD Device Registration ID .</span></span>|
|<span data-ttu-id="1bc87-118">deletionState</span><span class="sxs-lookup"><span data-stu-id="1bc87-118">deletionState</span></span>|[<span data-ttu-id="1bc87-119">windowsAutopilotDeviceDeletionState</span><span class="sxs-lookup"><span data-stu-id="1bc87-119">windowsAutopilotDeviceDeletionState</span></span>](../resources/intune-enrollment-windowsautopilotdevicedeletionstate.md)|<span data-ttu-id="1bc87-120">Состояние удаления устройства.</span><span class="sxs-lookup"><span data-stu-id="1bc87-120">Device deletion state.</span></span> <span data-ttu-id="1bc87-121">Возможные значения: `unknown`, `failed`, `accepted`, `error`.</span><span class="sxs-lookup"><span data-stu-id="1bc87-121">Possible values are: `unknown`, `failed`, `accepted`, `error`.</span></span>|
|<span data-ttu-id="1bc87-122">errorMessage</span><span class="sxs-lookup"><span data-stu-id="1bc87-122">errorMessage</span></span>|<span data-ttu-id="1bc87-123">Строка</span><span class="sxs-lookup"><span data-stu-id="1bc87-123">String</span></span>|<span data-ttu-id="1bc87-124">Сообщение об ошибке удаления устройства.</span><span class="sxs-lookup"><span data-stu-id="1bc87-124">Device deletion error message.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1bc87-125">Отношения</span><span class="sxs-lookup"><span data-stu-id="1bc87-125">Relationships</span></span>
<span data-ttu-id="1bc87-126">Нет</span><span class="sxs-lookup"><span data-stu-id="1bc87-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1bc87-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1bc87-127">JSON Representation</span></span>
<span data-ttu-id="1bc87-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1bc87-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deletedWindowsAutopilotDeviceState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deletedWindowsAutopilotDeviceState",
  "serialNumber": "String",
  "deviceRegistrationId": "String",
  "deletionState": "String",
  "errorMessage": "String"
}
```




