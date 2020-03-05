---
title: Тип ресурса importedWindowsAutopilotDeviceIdentityState
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c1af3f40e4e128272558b6fec75d5194ef48a9f6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528276"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="1db38-103">Тип ресурса importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="1db38-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

<span data-ttu-id="1db38-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1db38-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1db38-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1db38-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1db38-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1db38-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1db38-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="1db38-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="1db38-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="1db38-108">Properties</span></span>
|<span data-ttu-id="1db38-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="1db38-109">Property</span></span>|<span data-ttu-id="1db38-110">Тип</span><span class="sxs-lookup"><span data-stu-id="1db38-110">Type</span></span>|<span data-ttu-id="1db38-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1db38-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1db38-112">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="1db38-112">deviceImportStatus</span></span>|[<span data-ttu-id="1db38-113">импортедвиндовсаутопилотдевицеидентитимпортстатус</span><span class="sxs-lookup"><span data-stu-id="1db38-113">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="1db38-114">Состояние устройства, сообщаемое службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="1db38-114">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="1db38-115">Возможные значения: `unknown`, `pending`, `partial`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="1db38-115">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="1db38-116">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="1db38-116">deviceRegistrationId</span></span>|<span data-ttu-id="1db38-117">String</span><span class="sxs-lookup"><span data-stu-id="1db38-117">String</span></span>|<span data-ttu-id="1db38-118">Идентификатор регистрации устройства для успешно добавленного устройства, сообщаемый службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="1db38-118">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="1db38-119">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="1db38-119">deviceErrorCode</span></span>|<span data-ttu-id="1db38-120">Int32</span><span class="sxs-lookup"><span data-stu-id="1db38-120">Int32</span></span>|<span data-ttu-id="1db38-121">Код ошибки устройства, сообщаемый службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="1db38-121">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="1db38-122">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="1db38-122">deviceErrorName</span></span>|<span data-ttu-id="1db38-123">Строка</span><span class="sxs-lookup"><span data-stu-id="1db38-123">String</span></span>|<span data-ttu-id="1db38-124">Имя ошибки устройства, сообщаемое службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="1db38-124">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="1db38-125">Связи</span><span class="sxs-lookup"><span data-stu-id="1db38-125">Relationships</span></span>
<span data-ttu-id="1db38-126">Нет</span><span class="sxs-lookup"><span data-stu-id="1db38-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1db38-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1db38-127">JSON Representation</span></span>
<span data-ttu-id="1db38-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1db38-128">Here is a JSON representation of the resource.</span></span>
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



