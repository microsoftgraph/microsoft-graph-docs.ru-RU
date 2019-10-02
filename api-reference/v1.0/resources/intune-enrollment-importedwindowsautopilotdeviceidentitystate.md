---
title: Тип ресурса importedWindowsAutopilotDeviceIdentityState
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 841855ca7fb9de734fd685efa0d2382087256beb
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356837"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="603d9-103">Тип ресурса importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="603d9-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

> <span data-ttu-id="603d9-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="603d9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="603d9-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="603d9-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="603d9-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="603d9-106">Properties</span></span>
|<span data-ttu-id="603d9-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="603d9-107">Property</span></span>|<span data-ttu-id="603d9-108">Тип</span><span class="sxs-lookup"><span data-stu-id="603d9-108">Type</span></span>|<span data-ttu-id="603d9-109">Описание</span><span class="sxs-lookup"><span data-stu-id="603d9-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="603d9-110">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="603d9-110">deviceImportStatus</span></span>|[<span data-ttu-id="603d9-111">импортедвиндовсаутопилотдевицеидентитимпортстатус</span><span class="sxs-lookup"><span data-stu-id="603d9-111">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="603d9-112">Состояние устройства, сообщаемое службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="603d9-112">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="603d9-113">Возможные значения: `unknown`, `pending`, `partial`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="603d9-113">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="603d9-114">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="603d9-114">deviceRegistrationId</span></span>|<span data-ttu-id="603d9-115">String</span><span class="sxs-lookup"><span data-stu-id="603d9-115">String</span></span>|<span data-ttu-id="603d9-116">Идентификатор регистрации устройства для успешно добавленного устройства, сообщаемый службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="603d9-116">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="603d9-117">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="603d9-117">deviceErrorCode</span></span>|<span data-ttu-id="603d9-118">Int32</span><span class="sxs-lookup"><span data-stu-id="603d9-118">Int32</span></span>|<span data-ttu-id="603d9-119">Код ошибки устройства, сообщаемый службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="603d9-119">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="603d9-120">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="603d9-120">deviceErrorName</span></span>|<span data-ttu-id="603d9-121">Строка</span><span class="sxs-lookup"><span data-stu-id="603d9-121">String</span></span>|<span data-ttu-id="603d9-122">Имя ошибки устройства, сообщаемое службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="603d9-122">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="603d9-123">Связи</span><span class="sxs-lookup"><span data-stu-id="603d9-123">Relationships</span></span>
<span data-ttu-id="603d9-124">Нет</span><span class="sxs-lookup"><span data-stu-id="603d9-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="603d9-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="603d9-125">JSON Representation</span></span>
<span data-ttu-id="603d9-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="603d9-126">Here is a JSON representation of the resource.</span></span>
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




