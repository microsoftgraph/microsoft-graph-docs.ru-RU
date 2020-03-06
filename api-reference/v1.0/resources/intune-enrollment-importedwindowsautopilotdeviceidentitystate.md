---
title: Тип ресурса importedWindowsAutopilotDeviceIdentityState
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fe8ae3addc2d4b74323471bc39fd8d5569d4df99
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530246"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="5a0b8-103">Тип ресурса importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="5a0b8-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

<span data-ttu-id="5a0b8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a0b8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5a0b8-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5a0b8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a0b8-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="5a0b8-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="5a0b8-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5a0b8-107">Properties</span></span>
|<span data-ttu-id="5a0b8-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="5a0b8-108">Property</span></span>|<span data-ttu-id="5a0b8-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5a0b8-109">Type</span></span>|<span data-ttu-id="5a0b8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5a0b8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a0b8-111">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="5a0b8-111">deviceImportStatus</span></span>|[<span data-ttu-id="5a0b8-112">импортедвиндовсаутопилотдевицеидентитимпортстатус</span><span class="sxs-lookup"><span data-stu-id="5a0b8-112">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="5a0b8-113">Состояние устройства, сообщаемое службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="5a0b8-113">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="5a0b8-114">Возможные значения: `unknown`, `pending`, `partial`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="5a0b8-114">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="5a0b8-115">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="5a0b8-115">deviceRegistrationId</span></span>|<span data-ttu-id="5a0b8-116">Строка</span><span class="sxs-lookup"><span data-stu-id="5a0b8-116">String</span></span>|<span data-ttu-id="5a0b8-117">Идентификатор регистрации устройства для успешно добавленного устройства, сообщаемый службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="5a0b8-117">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="5a0b8-118">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="5a0b8-118">deviceErrorCode</span></span>|<span data-ttu-id="5a0b8-119">Int32</span><span class="sxs-lookup"><span data-stu-id="5a0b8-119">Int32</span></span>|<span data-ttu-id="5a0b8-120">Код ошибки устройства, сообщаемый службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="5a0b8-120">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="5a0b8-121">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="5a0b8-121">deviceErrorName</span></span>|<span data-ttu-id="5a0b8-122">Строка</span><span class="sxs-lookup"><span data-stu-id="5a0b8-122">String</span></span>|<span data-ttu-id="5a0b8-123">Имя ошибки устройства, сообщаемое службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="5a0b8-123">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="5a0b8-124">Связи</span><span class="sxs-lookup"><span data-stu-id="5a0b8-124">Relationships</span></span>
<span data-ttu-id="5a0b8-125">Нет</span><span class="sxs-lookup"><span data-stu-id="5a0b8-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5a0b8-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5a0b8-126">JSON Representation</span></span>
<span data-ttu-id="5a0b8-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5a0b8-127">Here is a JSON representation of the resource.</span></span>
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




