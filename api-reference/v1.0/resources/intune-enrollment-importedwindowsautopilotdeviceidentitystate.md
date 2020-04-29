---
title: Тип ресурса importedWindowsAutopilotDeviceIdentityState
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 696528c00f2dd82f1dd6cba6087acadaa158bbf4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439385"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="8cdc3-103">Тип ресурса importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="8cdc3-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

<span data-ttu-id="8cdc3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8cdc3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8cdc3-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8cdc3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8cdc3-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8cdc3-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="8cdc3-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="8cdc3-107">Properties</span></span>
|<span data-ttu-id="8cdc3-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="8cdc3-108">Property</span></span>|<span data-ttu-id="8cdc3-109">Тип</span><span class="sxs-lookup"><span data-stu-id="8cdc3-109">Type</span></span>|<span data-ttu-id="8cdc3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8cdc3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8cdc3-111">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="8cdc3-111">deviceImportStatus</span></span>|[<span data-ttu-id="8cdc3-112">импортедвиндовсаутопилотдевицеидентитимпортстатус</span><span class="sxs-lookup"><span data-stu-id="8cdc3-112">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="8cdc3-113">Состояние устройства, сообщаемое службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="8cdc3-113">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="8cdc3-114">Возможные значения: `unknown`, `pending`, `partial`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="8cdc3-114">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="8cdc3-115">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="8cdc3-115">deviceRegistrationId</span></span>|<span data-ttu-id="8cdc3-116">String</span><span class="sxs-lookup"><span data-stu-id="8cdc3-116">String</span></span>|<span data-ttu-id="8cdc3-117">Идентификатор регистрации устройства для успешно добавленного устройства, сообщаемый службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="8cdc3-117">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="8cdc3-118">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="8cdc3-118">deviceErrorCode</span></span>|<span data-ttu-id="8cdc3-119">Int32</span><span class="sxs-lookup"><span data-stu-id="8cdc3-119">Int32</span></span>|<span data-ttu-id="8cdc3-120">Код ошибки устройства, сообщаемый службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="8cdc3-120">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="8cdc3-121">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="8cdc3-121">deviceErrorName</span></span>|<span data-ttu-id="8cdc3-122">Строка</span><span class="sxs-lookup"><span data-stu-id="8cdc3-122">String</span></span>|<span data-ttu-id="8cdc3-123">Имя ошибки устройства, сообщаемое службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="8cdc3-123">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="8cdc3-124">Связи</span><span class="sxs-lookup"><span data-stu-id="8cdc3-124">Relationships</span></span>
<span data-ttu-id="8cdc3-125">Нет</span><span class="sxs-lookup"><span data-stu-id="8cdc3-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8cdc3-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8cdc3-126">JSON Representation</span></span>
<span data-ttu-id="8cdc3-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8cdc3-127">Here is a JSON representation of the resource.</span></span>
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







