---
title: Тип ресурса importedWindowsAutopilotDeviceIdentityState
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 42726817395296945fc593552ee50154fa34d332
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31779771"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="163a4-103">Тип ресурса importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="163a4-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

> <span data-ttu-id="163a4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="163a4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="163a4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="163a4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="163a4-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="163a4-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="163a4-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="163a4-107">Properties</span></span>
|<span data-ttu-id="163a4-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="163a4-108">Property</span></span>|<span data-ttu-id="163a4-109">Тип</span><span class="sxs-lookup"><span data-stu-id="163a4-109">Type</span></span>|<span data-ttu-id="163a4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="163a4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="163a4-111">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="163a4-111">deviceImportStatus</span></span>|[<span data-ttu-id="163a4-112">Импортедвиндовсаутопилотдевицеидентитимпортстатус</span><span class="sxs-lookup"><span data-stu-id="163a4-112">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="163a4-113">Состояние устройства, сообщаемое службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="163a4-113">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="163a4-114">Возможные значения: `unknown`, `pending`, `partial`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="163a4-114">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="163a4-115">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="163a4-115">deviceRegistrationId</span></span>|<span data-ttu-id="163a4-116">String</span><span class="sxs-lookup"><span data-stu-id="163a4-116">String</span></span>|<span data-ttu-id="163a4-117">Идентификатор регистрации устройства для успешно добавленного устройства, сообщаемый службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="163a4-117">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="163a4-118">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="163a4-118">deviceErrorCode</span></span>|<span data-ttu-id="163a4-119">Int32</span><span class="sxs-lookup"><span data-stu-id="163a4-119">Int32</span></span>|<span data-ttu-id="163a4-120">Код ошибки устройства, сообщаемый службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="163a4-120">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="163a4-121">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="163a4-121">deviceErrorName</span></span>|<span data-ttu-id="163a4-122">Строка</span><span class="sxs-lookup"><span data-stu-id="163a4-122">String</span></span>|<span data-ttu-id="163a4-123">Имя ошибки устройства, сообщаемое службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="163a4-123">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="163a4-124">Отношения</span><span class="sxs-lookup"><span data-stu-id="163a4-124">Relationships</span></span>
<span data-ttu-id="163a4-125">Нет</span><span class="sxs-lookup"><span data-stu-id="163a4-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="163a4-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="163a4-126">JSON Representation</span></span>
<span data-ttu-id="163a4-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="163a4-127">Here is a JSON representation of the resource.</span></span>
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





