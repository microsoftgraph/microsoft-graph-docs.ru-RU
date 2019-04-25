---
title: Тип ресурса importedWindowsAutopilotDeviceIdentityState
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7e65de1501bb0480daf195ce910001624cabff98
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523366"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="95a10-103">Тип ресурса importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="95a10-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

> <span data-ttu-id="95a10-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="95a10-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95a10-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="95a10-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="95a10-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="95a10-106">Properties</span></span>
|<span data-ttu-id="95a10-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="95a10-107">Property</span></span>|<span data-ttu-id="95a10-108">Тип</span><span class="sxs-lookup"><span data-stu-id="95a10-108">Type</span></span>|<span data-ttu-id="95a10-109">Описание</span><span class="sxs-lookup"><span data-stu-id="95a10-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95a10-110">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="95a10-110">deviceImportStatus</span></span>|[<span data-ttu-id="95a10-111">Импортедвиндовсаутопилотдевицеидентитимпортстатус</span><span class="sxs-lookup"><span data-stu-id="95a10-111">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="95a10-112">Состояние устройства, сообщаемое службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="95a10-112">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="95a10-113">Возможные значения: `unknown`, `pending`, `partial`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="95a10-113">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="95a10-114">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="95a10-114">deviceRegistrationId</span></span>|<span data-ttu-id="95a10-115">String</span><span class="sxs-lookup"><span data-stu-id="95a10-115">String</span></span>|<span data-ttu-id="95a10-116">Идентификатор регистрации устройства для успешно добавленного устройства, сообщаемый службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="95a10-116">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="95a10-117">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="95a10-117">deviceErrorCode</span></span>|<span data-ttu-id="95a10-118">Int32</span><span class="sxs-lookup"><span data-stu-id="95a10-118">Int32</span></span>|<span data-ttu-id="95a10-119">Код ошибки устройства, сообщаемый службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="95a10-119">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="95a10-120">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="95a10-120">deviceErrorName</span></span>|<span data-ttu-id="95a10-121">Строка</span><span class="sxs-lookup"><span data-stu-id="95a10-121">String</span></span>|<span data-ttu-id="95a10-122">Имя ошибки устройства, сообщаемое службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="95a10-122">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="95a10-123">Отношения</span><span class="sxs-lookup"><span data-stu-id="95a10-123">Relationships</span></span>
<span data-ttu-id="95a10-124">Нет</span><span class="sxs-lookup"><span data-stu-id="95a10-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="95a10-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="95a10-125">JSON Representation</span></span>
<span data-ttu-id="95a10-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="95a10-126">Here is a JSON representation of the resource.</span></span>
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



