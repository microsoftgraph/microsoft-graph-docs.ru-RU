---
title: Тип ресурса importedWindowsAutopilotDeviceIdentityState
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 72ed544a7b4f9e4ddf003104b191ee064b884f76
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159012"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="f4d55-103">Тип ресурса importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="f4d55-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

> <span data-ttu-id="f4d55-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4d55-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4d55-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f4d55-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4d55-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="f4d55-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="f4d55-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f4d55-107">Properties</span></span>
|<span data-ttu-id="f4d55-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f4d55-108">Property</span></span>|<span data-ttu-id="f4d55-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f4d55-109">Type</span></span>|<span data-ttu-id="f4d55-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f4d55-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4d55-111">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="f4d55-111">deviceImportStatus</span></span>|[<span data-ttu-id="f4d55-112">Импортедвиндовсаутопилотдевицеидентитимпортстатус</span><span class="sxs-lookup"><span data-stu-id="f4d55-112">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="f4d55-113">Состояние устройства, сообщаемое службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="f4d55-113">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="f4d55-114">Возможные значения: `unknown`, `pending`, `partial`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="f4d55-114">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="f4d55-115">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="f4d55-115">deviceRegistrationId</span></span>|<span data-ttu-id="f4d55-116">String</span><span class="sxs-lookup"><span data-stu-id="f4d55-116">String</span></span>|<span data-ttu-id="f4d55-117">Идентификатор регистрации устройства для успешно добавленного устройства, сообщаемый службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="f4d55-117">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="f4d55-118">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="f4d55-118">deviceErrorCode</span></span>|<span data-ttu-id="f4d55-119">Int32</span><span class="sxs-lookup"><span data-stu-id="f4d55-119">Int32</span></span>|<span data-ttu-id="f4d55-120">Код ошибки устройства, сообщаемый службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="f4d55-120">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="f4d55-121">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="f4d55-121">deviceErrorName</span></span>|<span data-ttu-id="f4d55-122">Строка</span><span class="sxs-lookup"><span data-stu-id="f4d55-122">String</span></span>|<span data-ttu-id="f4d55-123">Имя ошибки устройства, сообщаемое службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="f4d55-123">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="f4d55-124">Связи</span><span class="sxs-lookup"><span data-stu-id="f4d55-124">Relationships</span></span>
<span data-ttu-id="f4d55-125">Нет</span><span class="sxs-lookup"><span data-stu-id="f4d55-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f4d55-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f4d55-126">JSON Representation</span></span>
<span data-ttu-id="f4d55-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f4d55-127">Here is a JSON representation of the resource.</span></span>
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




