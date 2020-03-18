---
title: Тип ресурса importedWindowsAutopilotDeviceIdentityState
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e4db6d07a1388015f95f63e5d4381c47beca9f42
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783440"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="00cc1-103">Тип ресурса importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="00cc1-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

> <span data-ttu-id="00cc1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00cc1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="00cc1-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="00cc1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00cc1-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="00cc1-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="00cc1-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="00cc1-107">Properties</span></span>
|<span data-ttu-id="00cc1-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="00cc1-108">Property</span></span>|<span data-ttu-id="00cc1-109">Тип</span><span class="sxs-lookup"><span data-stu-id="00cc1-109">Type</span></span>|<span data-ttu-id="00cc1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="00cc1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00cc1-111">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="00cc1-111">deviceImportStatus</span></span>|[<span data-ttu-id="00cc1-112">импортедвиндовсаутопилотдевицеидентитимпортстатус</span><span class="sxs-lookup"><span data-stu-id="00cc1-112">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="00cc1-113">Состояние устройства, сообщаемое службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="00cc1-113">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="00cc1-114">Возможные значения: `unknown`, `pending`, `partial`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="00cc1-114">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="00cc1-115">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="00cc1-115">deviceRegistrationId</span></span>|<span data-ttu-id="00cc1-116">String</span><span class="sxs-lookup"><span data-stu-id="00cc1-116">String</span></span>|<span data-ttu-id="00cc1-117">Идентификатор регистрации устройства для успешно добавленного устройства, сообщаемый службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="00cc1-117">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="00cc1-118">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="00cc1-118">deviceErrorCode</span></span>|<span data-ttu-id="00cc1-119">Int32</span><span class="sxs-lookup"><span data-stu-id="00cc1-119">Int32</span></span>|<span data-ttu-id="00cc1-120">Код ошибки устройства, сообщаемый службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="00cc1-120">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="00cc1-121">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="00cc1-121">deviceErrorName</span></span>|<span data-ttu-id="00cc1-122">Строка</span><span class="sxs-lookup"><span data-stu-id="00cc1-122">String</span></span>|<span data-ttu-id="00cc1-123">Имя ошибки устройства, сообщаемое службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="00cc1-123">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="00cc1-124">Связи</span><span class="sxs-lookup"><span data-stu-id="00cc1-124">Relationships</span></span>
<span data-ttu-id="00cc1-125">Нет</span><span class="sxs-lookup"><span data-stu-id="00cc1-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="00cc1-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="00cc1-126">JSON Representation</span></span>
<span data-ttu-id="00cc1-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="00cc1-127">Here is a JSON representation of the resource.</span></span>
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



