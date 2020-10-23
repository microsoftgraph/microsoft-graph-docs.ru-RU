---
title: Тип ресурса importedWindowsAutopilotDeviceIdentityState
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b14b632e03160e9b56de1ad2ba0c2e32a1b74179
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728979"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="e0074-103">Тип ресурса importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="e0074-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

<span data-ttu-id="e0074-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0074-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e0074-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0074-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e0074-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e0074-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0074-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e0074-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="e0074-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e0074-108">Properties</span></span>
|<span data-ttu-id="e0074-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e0074-109">Property</span></span>|<span data-ttu-id="e0074-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e0074-110">Type</span></span>|<span data-ttu-id="e0074-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e0074-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0074-112">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="e0074-112">deviceImportStatus</span></span>|[<span data-ttu-id="e0074-113">импортедвиндовсаутопилотдевицеидентитимпортстатус</span><span class="sxs-lookup"><span data-stu-id="e0074-113">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="e0074-114">Состояние устройства, сообщаемое службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="e0074-114">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="e0074-115">Возможные значения: `unknown`, `pending`, `partial`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="e0074-115">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="e0074-116">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="e0074-116">deviceRegistrationId</span></span>|<span data-ttu-id="e0074-117">Строка</span><span class="sxs-lookup"><span data-stu-id="e0074-117">String</span></span>|<span data-ttu-id="e0074-118">Идентификатор регистрации устройства для успешно добавленного устройства, сообщаемый службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="e0074-118">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="e0074-119">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="e0074-119">deviceErrorCode</span></span>|<span data-ttu-id="e0074-120">Int32</span><span class="sxs-lookup"><span data-stu-id="e0074-120">Int32</span></span>|<span data-ttu-id="e0074-121">Код ошибки устройства, сообщаемый службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="e0074-121">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="e0074-122">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="e0074-122">deviceErrorName</span></span>|<span data-ttu-id="e0074-123">Строка</span><span class="sxs-lookup"><span data-stu-id="e0074-123">String</span></span>|<span data-ttu-id="e0074-124">Имя ошибки устройства, сообщаемое службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="e0074-124">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="e0074-125">Связи</span><span class="sxs-lookup"><span data-stu-id="e0074-125">Relationships</span></span>
<span data-ttu-id="e0074-126">Нет</span><span class="sxs-lookup"><span data-stu-id="e0074-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e0074-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e0074-127">JSON Representation</span></span>
<span data-ttu-id="e0074-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e0074-128">Here is a JSON representation of the resource.</span></span>
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





