---
title: Тип ресурса importedWindowsAutopilotDeviceIdentityState
description: Н/Д
ms.openlocfilehash: 6891c95a6c25c31c496c53520a22d5522995e29f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026690"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="36f83-103">Тип ресурса importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="36f83-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

> <span data-ttu-id="36f83-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="36f83-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="36f83-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="36f83-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="36f83-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="36f83-106">Properties</span></span>
|<span data-ttu-id="36f83-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="36f83-107">Property</span></span>|<span data-ttu-id="36f83-108">Тип</span><span class="sxs-lookup"><span data-stu-id="36f83-108">Type</span></span>|<span data-ttu-id="36f83-109">Описание</span><span class="sxs-lookup"><span data-stu-id="36f83-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36f83-110">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="36f83-110">deviceImportStatus</span></span>|[<span data-ttu-id="36f83-111">importedWindowsAutopilotDeviceIdentityImportStatus</span><span class="sxs-lookup"><span data-stu-id="36f83-111">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="36f83-112">Состояние устройства, сообщаемое службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="36f83-112">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="36f83-113">Возможные значения: `unknown`, `pending`, `partial`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="36f83-113">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="36f83-114">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="36f83-114">deviceRegistrationId</span></span>|<span data-ttu-id="36f83-115">Строка</span><span class="sxs-lookup"><span data-stu-id="36f83-115">String</span></span>|<span data-ttu-id="36f83-116">Идентификатор регистрации устройства для успешно добавленного устройства, сообщаемый службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="36f83-116">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="36f83-117">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="36f83-117">deviceErrorCode</span></span>|<span data-ttu-id="36f83-118">Int32</span><span class="sxs-lookup"><span data-stu-id="36f83-118">Int32</span></span>|<span data-ttu-id="36f83-119">Код ошибки устройства, сообщаемый службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="36f83-119">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="36f83-120">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="36f83-120">deviceErrorName</span></span>|<span data-ttu-id="36f83-121">Строка</span><span class="sxs-lookup"><span data-stu-id="36f83-121">String</span></span>|<span data-ttu-id="36f83-122">Имя ошибки устройства, сообщаемое службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="36f83-122">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="36f83-123">Связи</span><span class="sxs-lookup"><span data-stu-id="36f83-123">Relationships</span></span>
<span data-ttu-id="36f83-124">Нет</span><span class="sxs-lookup"><span data-stu-id="36f83-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="36f83-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="36f83-125">JSON Representation</span></span>
<span data-ttu-id="36f83-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="36f83-126">Here is a JSON representation of the resource.</span></span>
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



