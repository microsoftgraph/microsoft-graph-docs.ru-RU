---
title: activateDeviceEsimActionResult type
description: Активация результата действия eSIM устройства
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3c0a391ee52a84b49e105e90eff57510b8ae1010
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52667224"
---
# <a name="activatedeviceesimactionresult-resource-type"></a><span data-ttu-id="935a9-103">activateDeviceEsimActionResult type</span><span class="sxs-lookup"><span data-stu-id="935a9-103">activateDeviceEsimActionResult resource type</span></span>

<span data-ttu-id="935a9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="935a9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="935a9-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="935a9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="935a9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="935a9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="935a9-107">Активация результата действия eSIM устройства</span><span class="sxs-lookup"><span data-stu-id="935a9-107">Activate device eSIM action result</span></span>


<span data-ttu-id="935a9-108">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="935a9-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="935a9-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="935a9-109">Properties</span></span>
|<span data-ttu-id="935a9-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="935a9-110">Property</span></span>|<span data-ttu-id="935a9-111">Тип</span><span class="sxs-lookup"><span data-stu-id="935a9-111">Type</span></span>|<span data-ttu-id="935a9-112">Описание</span><span class="sxs-lookup"><span data-stu-id="935a9-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="935a9-113">actionName</span><span class="sxs-lookup"><span data-stu-id="935a9-113">actionName</span></span>|<span data-ttu-id="935a9-114">String</span><span class="sxs-lookup"><span data-stu-id="935a9-114">String</span></span>|<span data-ttu-id="935a9-115">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="935a9-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="935a9-116">actionState</span><span class="sxs-lookup"><span data-stu-id="935a9-116">actionState</span></span>|[<span data-ttu-id="935a9-117">actionState</span><span class="sxs-lookup"><span data-stu-id="935a9-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="935a9-118">Состояние действия, унаследованной от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="935a9-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="935a9-119">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="935a9-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="935a9-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="935a9-120">startDateTime</span></span>|<span data-ttu-id="935a9-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="935a9-121">DateTimeOffset</span></span>|<span data-ttu-id="935a9-122">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="935a9-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="935a9-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="935a9-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="935a9-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="935a9-124">DateTimeOffset</span></span>|<span data-ttu-id="935a9-125">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="935a9-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="935a9-126">carrierUrl</span><span class="sxs-lookup"><span data-stu-id="935a9-126">carrierUrl</span></span>|<span data-ttu-id="935a9-127">Строка</span><span class="sxs-lookup"><span data-stu-id="935a9-127">String</span></span>|<span data-ttu-id="935a9-128">Url-адрес carrier для активации eSIM устройства</span><span class="sxs-lookup"><span data-stu-id="935a9-128">Carrier Url to activate the device eSIM</span></span> |

## <a name="relationships"></a><span data-ttu-id="935a9-129">Связи</span><span class="sxs-lookup"><span data-stu-id="935a9-129">Relationships</span></span>
<span data-ttu-id="935a9-130">Нет</span><span class="sxs-lookup"><span data-stu-id="935a9-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="935a9-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="935a9-131">JSON Representation</span></span>
<span data-ttu-id="935a9-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="935a9-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.activateDeviceEsimActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.activateDeviceEsimActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "carrierUrl": "String"
}
```




