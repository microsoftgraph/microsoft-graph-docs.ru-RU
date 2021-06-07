---
title: Тип ресурса importedWindowsAutopilotDeviceIdentityState
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d402e7902c3f7ed213ccff9e81c1d179bf3128cf
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753080"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="689bc-103">Тип ресурса importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="689bc-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

<span data-ttu-id="689bc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="689bc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="689bc-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="689bc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="689bc-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="689bc-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="689bc-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="689bc-107">Properties</span></span>
|<span data-ttu-id="689bc-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="689bc-108">Property</span></span>|<span data-ttu-id="689bc-109">Тип</span><span class="sxs-lookup"><span data-stu-id="689bc-109">Type</span></span>|<span data-ttu-id="689bc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="689bc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="689bc-111">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="689bc-111">deviceImportStatus</span></span>|[<span data-ttu-id="689bc-112">importedWindowsAutopilotDeviceIdentityImportStatus</span><span class="sxs-lookup"><span data-stu-id="689bc-112">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="689bc-113">Состояние устройства, сообщаемое службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="689bc-113">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="689bc-114">Возможные значения: `unknown`, `pending`, `partial`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="689bc-114">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="689bc-115">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="689bc-115">deviceRegistrationId</span></span>|<span data-ttu-id="689bc-116">Строка</span><span class="sxs-lookup"><span data-stu-id="689bc-116">String</span></span>|<span data-ttu-id="689bc-117">Идентификатор регистрации устройства для успешно добавленного устройства, сообщаемый службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="689bc-117">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="689bc-118">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="689bc-118">deviceErrorCode</span></span>|<span data-ttu-id="689bc-119">Int32</span><span class="sxs-lookup"><span data-stu-id="689bc-119">Int32</span></span>|<span data-ttu-id="689bc-120">Код ошибки устройства, сообщаемый службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="689bc-120">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="689bc-121">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="689bc-121">deviceErrorName</span></span>|<span data-ttu-id="689bc-122">Строка</span><span class="sxs-lookup"><span data-stu-id="689bc-122">String</span></span>|<span data-ttu-id="689bc-123">Имя ошибки устройства, сообщаемое службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="689bc-123">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="689bc-124">Связи</span><span class="sxs-lookup"><span data-stu-id="689bc-124">Relationships</span></span>
<span data-ttu-id="689bc-125">Нет</span><span class="sxs-lookup"><span data-stu-id="689bc-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="689bc-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="689bc-126">JSON Representation</span></span>
<span data-ttu-id="689bc-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="689bc-127">Here is a JSON representation of the resource.</span></span>
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




