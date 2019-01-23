---
title: Тип ресурса importedWindowsAutopilotDeviceIdentityState
description: Н/Д
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0f4e76b23d4d970a9fb873326dc84f278aa2ed2b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410968"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="467f9-103">Тип ресурса importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="467f9-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

> <span data-ttu-id="467f9-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="467f9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="467f9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="467f9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="467f9-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="467f9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="467f9-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="467f9-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="467f9-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="467f9-108">Properties</span></span>
|<span data-ttu-id="467f9-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="467f9-109">Property</span></span>|<span data-ttu-id="467f9-110">Тип</span><span class="sxs-lookup"><span data-stu-id="467f9-110">Type</span></span>|<span data-ttu-id="467f9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="467f9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="467f9-112">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="467f9-112">deviceImportStatus</span></span>|[<span data-ttu-id="467f9-113">importedWindowsAutopilotDeviceIdentityImportStatus</span><span class="sxs-lookup"><span data-stu-id="467f9-113">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="467f9-114">Состояние устройства, сообщаемое службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="467f9-114">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="467f9-115">Возможные значения: `unknown`, `pending`, `partial`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="467f9-115">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="467f9-116">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="467f9-116">deviceRegistrationId</span></span>|<span data-ttu-id="467f9-117">Строка</span><span class="sxs-lookup"><span data-stu-id="467f9-117">String</span></span>|<span data-ttu-id="467f9-118">Идентификатор регистрации устройства для успешно добавленного устройства, сообщаемый службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="467f9-118">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="467f9-119">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="467f9-119">deviceErrorCode</span></span>|<span data-ttu-id="467f9-120">Int32</span><span class="sxs-lookup"><span data-stu-id="467f9-120">Int32</span></span>|<span data-ttu-id="467f9-121">Код ошибки устройства, сообщаемый службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="467f9-121">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="467f9-122">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="467f9-122">deviceErrorName</span></span>|<span data-ttu-id="467f9-123">Строка</span><span class="sxs-lookup"><span data-stu-id="467f9-123">String</span></span>|<span data-ttu-id="467f9-124">Имя ошибки устройства, сообщаемое службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="467f9-124">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="467f9-125">Связи</span><span class="sxs-lookup"><span data-stu-id="467f9-125">Relationships</span></span>
<span data-ttu-id="467f9-126">Нет</span><span class="sxs-lookup"><span data-stu-id="467f9-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="467f9-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="467f9-127">JSON Representation</span></span>
<span data-ttu-id="467f9-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="467f9-128">Here is a JSON representation of the resource.</span></span>
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




