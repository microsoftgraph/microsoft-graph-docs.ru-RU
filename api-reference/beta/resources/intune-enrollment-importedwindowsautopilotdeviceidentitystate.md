---
title: Тип ресурса importedWindowsAutopilotDeviceIdentityState
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ec21d554010982508776cfbef8cafe32e61a8c51
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43460785"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="9c2af-103">Тип ресурса importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="9c2af-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

<span data-ttu-id="9c2af-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c2af-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9c2af-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c2af-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9c2af-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9c2af-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c2af-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="9c2af-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="9c2af-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="9c2af-108">Properties</span></span>
|<span data-ttu-id="9c2af-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="9c2af-109">Property</span></span>|<span data-ttu-id="9c2af-110">Тип</span><span class="sxs-lookup"><span data-stu-id="9c2af-110">Type</span></span>|<span data-ttu-id="9c2af-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9c2af-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c2af-112">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="9c2af-112">deviceImportStatus</span></span>|[<span data-ttu-id="9c2af-113">импортедвиндовсаутопилотдевицеидентитимпортстатус</span><span class="sxs-lookup"><span data-stu-id="9c2af-113">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="9c2af-114">Состояние устройства, сообщаемое службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="9c2af-114">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="9c2af-115">Возможные значения: `unknown`, `pending`, `partial`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="9c2af-115">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="9c2af-116">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="9c2af-116">deviceRegistrationId</span></span>|<span data-ttu-id="9c2af-117">String</span><span class="sxs-lookup"><span data-stu-id="9c2af-117">String</span></span>|<span data-ttu-id="9c2af-118">Идентификатор регистрации устройства для успешно добавленного устройства, сообщаемый службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="9c2af-118">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="9c2af-119">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="9c2af-119">deviceErrorCode</span></span>|<span data-ttu-id="9c2af-120">Int32</span><span class="sxs-lookup"><span data-stu-id="9c2af-120">Int32</span></span>|<span data-ttu-id="9c2af-121">Код ошибки устройства, сообщаемый службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="9c2af-121">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="9c2af-122">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="9c2af-122">deviceErrorName</span></span>|<span data-ttu-id="9c2af-123">Строка</span><span class="sxs-lookup"><span data-stu-id="9c2af-123">String</span></span>|<span data-ttu-id="9c2af-124">Имя ошибки устройства, сообщаемое службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="9c2af-124">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="9c2af-125">Отношения</span><span class="sxs-lookup"><span data-stu-id="9c2af-125">Relationships</span></span>
<span data-ttu-id="9c2af-126">Нет</span><span class="sxs-lookup"><span data-stu-id="9c2af-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9c2af-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9c2af-127">JSON Representation</span></span>
<span data-ttu-id="9c2af-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9c2af-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
  "deviceImportStatus": "String",
  "deviceRegistrationId": "String",
  "deviceErrorCode": 1024,
  "deviceErrorName": "String"
}
```



