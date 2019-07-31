---
title: Тип ресурса importedWindowsAutopilotDeviceIdentityState
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0dbf080592462a104ba6380c6db8116498b9143e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999087"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="14834-103">Тип ресурса importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="14834-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

> <span data-ttu-id="14834-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14834-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14834-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="14834-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14834-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="14834-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="14834-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="14834-107">Properties</span></span>
|<span data-ttu-id="14834-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="14834-108">Property</span></span>|<span data-ttu-id="14834-109">Тип</span><span class="sxs-lookup"><span data-stu-id="14834-109">Type</span></span>|<span data-ttu-id="14834-110">Описание</span><span class="sxs-lookup"><span data-stu-id="14834-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14834-111">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="14834-111">deviceImportStatus</span></span>|[<span data-ttu-id="14834-112">Импортедвиндовсаутопилотдевицеидентитимпортстатус</span><span class="sxs-lookup"><span data-stu-id="14834-112">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="14834-113">Состояние устройства, сообщаемое службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="14834-113">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="14834-114">Возможные значения: `unknown`, `pending`, `partial`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="14834-114">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="14834-115">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="14834-115">deviceRegistrationId</span></span>|<span data-ttu-id="14834-116">String</span><span class="sxs-lookup"><span data-stu-id="14834-116">String</span></span>|<span data-ttu-id="14834-117">Идентификатор регистрации устройства для успешно добавленного устройства, сообщаемый службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="14834-117">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="14834-118">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="14834-118">deviceErrorCode</span></span>|<span data-ttu-id="14834-119">Int32</span><span class="sxs-lookup"><span data-stu-id="14834-119">Int32</span></span>|<span data-ttu-id="14834-120">Код ошибки устройства, сообщаемый службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="14834-120">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="14834-121">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="14834-121">deviceErrorName</span></span>|<span data-ttu-id="14834-122">Строка</span><span class="sxs-lookup"><span data-stu-id="14834-122">String</span></span>|<span data-ttu-id="14834-123">Имя ошибки устройства, сообщаемое службой каталогов устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="14834-123">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="14834-124">Отношения</span><span class="sxs-lookup"><span data-stu-id="14834-124">Relationships</span></span>
<span data-ttu-id="14834-125">Нет</span><span class="sxs-lookup"><span data-stu-id="14834-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="14834-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="14834-126">JSON Representation</span></span>
<span data-ttu-id="14834-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="14834-127">Here is a JSON representation of the resource.</span></span>
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





