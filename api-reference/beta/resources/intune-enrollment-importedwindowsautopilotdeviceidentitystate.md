---
title: Тип ресурса importedWindowsAutopilotDeviceIdentityState
description: Н/Д
ms.openlocfilehash: cdb13df520d109ddcc49e2637652499186ac9f24
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079646"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="f0f62-103">Тип ресурса importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="f0f62-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

> <span data-ttu-id="f0f62-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f0f62-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f0f62-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0f62-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f0f62-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f0f62-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f0f62-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="f0f62-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="f0f62-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f0f62-108">Properties</span></span>
|<span data-ttu-id="f0f62-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f0f62-109">Property</span></span>|<span data-ttu-id="f0f62-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f0f62-110">Type</span></span>|<span data-ttu-id="f0f62-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f0f62-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0f62-112">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="f0f62-112">deviceImportStatus</span></span>|[<span data-ttu-id="f0f62-113">importedWindowsAutopilotDeviceIdentityImportStatus</span><span class="sxs-lookup"><span data-stu-id="f0f62-113">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="f0f62-114">Состояние устройства, сообщаемое службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="f0f62-114">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="f0f62-115">Возможные значения: `unknown`, `pending`, `partial`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="f0f62-115">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="f0f62-116">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="f0f62-116">deviceRegistrationId</span></span>|<span data-ttu-id="f0f62-117">Строка</span><span class="sxs-lookup"><span data-stu-id="f0f62-117">String</span></span>|<span data-ttu-id="f0f62-118">Идентификатор регистрации устройства для успешно добавленного устройства, сообщаемый службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="f0f62-118">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="f0f62-119">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="f0f62-119">deviceErrorCode</span></span>|<span data-ttu-id="f0f62-120">Int32</span><span class="sxs-lookup"><span data-stu-id="f0f62-120">Int32</span></span>|<span data-ttu-id="f0f62-121">Код ошибки устройства, сообщаемый службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="f0f62-121">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="f0f62-122">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="f0f62-122">deviceErrorName</span></span>|<span data-ttu-id="f0f62-123">Строка</span><span class="sxs-lookup"><span data-stu-id="f0f62-123">String</span></span>|<span data-ttu-id="f0f62-124">Имя ошибки устройства, сообщаемое службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="f0f62-124">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="f0f62-125">Связи</span><span class="sxs-lookup"><span data-stu-id="f0f62-125">Relationships</span></span>
<span data-ttu-id="f0f62-126">Нет</span><span class="sxs-lookup"><span data-stu-id="f0f62-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f0f62-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f0f62-127">JSON Representation</span></span>
<span data-ttu-id="f0f62-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f0f62-128">Here is a JSON representation of the resource.</span></span>
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





