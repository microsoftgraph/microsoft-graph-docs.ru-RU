---
title: Тип ресурса importedWindowsAutopilotDeviceIdentityState
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f6bb27b603669da82a42501563ad4be3220c7249
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870765"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="140cb-103">Тип ресурса importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="140cb-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

> <span data-ttu-id="140cb-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="140cb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="140cb-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="140cb-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="140cb-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="140cb-106">Properties</span></span>
|<span data-ttu-id="140cb-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="140cb-107">Property</span></span>|<span data-ttu-id="140cb-108">Тип</span><span class="sxs-lookup"><span data-stu-id="140cb-108">Type</span></span>|<span data-ttu-id="140cb-109">Описание</span><span class="sxs-lookup"><span data-stu-id="140cb-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="140cb-110">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="140cb-110">deviceImportStatus</span></span>|[<span data-ttu-id="140cb-111">importedWindowsAutopilotDeviceIdentityImportStatus</span><span class="sxs-lookup"><span data-stu-id="140cb-111">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="140cb-112">Состояние устройства, сообщаемое службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="140cb-112">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="140cb-113">Возможные значения: `unknown`, `pending`, `partial`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="140cb-113">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="140cb-114">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="140cb-114">deviceRegistrationId</span></span>|<span data-ttu-id="140cb-115">Строка</span><span class="sxs-lookup"><span data-stu-id="140cb-115">String</span></span>|<span data-ttu-id="140cb-116">Идентификатор регистрации устройства для успешно добавленного устройства, сообщаемый службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="140cb-116">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="140cb-117">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="140cb-117">deviceErrorCode</span></span>|<span data-ttu-id="140cb-118">Int32</span><span class="sxs-lookup"><span data-stu-id="140cb-118">Int32</span></span>|<span data-ttu-id="140cb-119">Код ошибки устройства, сообщаемый службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="140cb-119">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="140cb-120">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="140cb-120">deviceErrorName</span></span>|<span data-ttu-id="140cb-121">Строка</span><span class="sxs-lookup"><span data-stu-id="140cb-121">String</span></span>|<span data-ttu-id="140cb-122">Имя ошибки устройства, сообщаемое службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="140cb-122">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="140cb-123">Связи</span><span class="sxs-lookup"><span data-stu-id="140cb-123">Relationships</span></span>
<span data-ttu-id="140cb-124">Нет</span><span class="sxs-lookup"><span data-stu-id="140cb-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="140cb-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="140cb-125">JSON Representation</span></span>
<span data-ttu-id="140cb-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="140cb-126">Here is a JSON representation of the resource.</span></span>
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



