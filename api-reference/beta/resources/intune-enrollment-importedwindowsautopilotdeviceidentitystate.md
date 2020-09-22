---
title: Тип ресурса importedWindowsAutopilotDeviceIdentityState
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 20a5d4ef3fe2dc79c3843d86c525086940a8d78c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48079937"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="b0274-103">Тип ресурса importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="b0274-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

<span data-ttu-id="b0274-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0274-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b0274-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0274-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0274-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b0274-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0274-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="b0274-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="b0274-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b0274-108">Properties</span></span>
|<span data-ttu-id="b0274-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b0274-109">Property</span></span>|<span data-ttu-id="b0274-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b0274-110">Type</span></span>|<span data-ttu-id="b0274-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b0274-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0274-112">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="b0274-112">deviceImportStatus</span></span>|[<span data-ttu-id="b0274-113">импортедвиндовсаутопилотдевицеидентитимпортстатус</span><span class="sxs-lookup"><span data-stu-id="b0274-113">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="b0274-114">Состояние устройства, сообщаемое службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="b0274-114">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="b0274-115">Возможные значения: `unknown`, `pending`, `partial`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="b0274-115">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="b0274-116">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="b0274-116">deviceRegistrationId</span></span>|<span data-ttu-id="b0274-117">Строка</span><span class="sxs-lookup"><span data-stu-id="b0274-117">String</span></span>|<span data-ttu-id="b0274-118">Идентификатор регистрации устройства для успешно добавленного устройства, сообщаемый службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="b0274-118">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="b0274-119">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="b0274-119">deviceErrorCode</span></span>|<span data-ttu-id="b0274-120">Int32</span><span class="sxs-lookup"><span data-stu-id="b0274-120">Int32</span></span>|<span data-ttu-id="b0274-121">Код ошибки устройства, сообщаемый службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="b0274-121">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="b0274-122">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="b0274-122">deviceErrorName</span></span>|<span data-ttu-id="b0274-123">Строка</span><span class="sxs-lookup"><span data-stu-id="b0274-123">String</span></span>|<span data-ttu-id="b0274-124">Имя ошибки устройства, сообщаемое службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="b0274-124">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0274-125">Отношения</span><span class="sxs-lookup"><span data-stu-id="b0274-125">Relationships</span></span>
<span data-ttu-id="b0274-126">Нет</span><span class="sxs-lookup"><span data-stu-id="b0274-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0274-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b0274-127">JSON Representation</span></span>
<span data-ttu-id="b0274-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b0274-128">Here is a JSON representation of the resource.</span></span>
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






