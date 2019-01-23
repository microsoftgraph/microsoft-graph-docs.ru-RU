---
title: Тип ресурса mobileAppSupportedDeviceType
description: Свойства устройства
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c01691b3f6fcb2ed5838c1c9103c99ad6fbe792f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399754"
---
# <a name="mobileappsupporteddevicetype-resource-type"></a><span data-ttu-id="7420c-103">Тип ресурса mobileAppSupportedDeviceType</span><span class="sxs-lookup"><span data-stu-id="7420c-103">mobileAppSupportedDeviceType resource type</span></span>

> <span data-ttu-id="7420c-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7420c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7420c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7420c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7420c-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7420c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7420c-107">Свойства устройства</span><span class="sxs-lookup"><span data-stu-id="7420c-107">Device properties</span></span>

## <a name="properties"></a><span data-ttu-id="7420c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="7420c-108">Properties</span></span>
|<span data-ttu-id="7420c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="7420c-109">Property</span></span>|<span data-ttu-id="7420c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="7420c-110">Type</span></span>|<span data-ttu-id="7420c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7420c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7420c-112">type</span><span class="sxs-lookup"><span data-stu-id="7420c-112">type</span></span>|[<span data-ttu-id="7420c-113">deviceType</span><span class="sxs-lookup"><span data-stu-id="7420c-113">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="7420c-114">Тип устройства.</span><span class="sxs-lookup"><span data-stu-id="7420c-114">Device type.</span></span> <span data-ttu-id="7420c-115">Возможные значения: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="7420c-115">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="7420c-116">minimumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="7420c-116">minimumOperatingSystemVersion</span></span>|<span data-ttu-id="7420c-117">String</span><span class="sxs-lookup"><span data-stu-id="7420c-117">String</span></span>|<span data-ttu-id="7420c-118">Минимальная версия операционной системы</span><span class="sxs-lookup"><span data-stu-id="7420c-118">Minimum OS version</span></span>|
|<span data-ttu-id="7420c-119">maximumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="7420c-119">maximumOperatingSystemVersion</span></span>|<span data-ttu-id="7420c-120">String</span><span class="sxs-lookup"><span data-stu-id="7420c-120">String</span></span>|<span data-ttu-id="7420c-121">Максимальная версия ОС</span><span class="sxs-lookup"><span data-stu-id="7420c-121">Maximum OS version</span></span>|

## <a name="relationships"></a><span data-ttu-id="7420c-122">Отношения</span><span class="sxs-lookup"><span data-stu-id="7420c-122">Relationships</span></span>
<span data-ttu-id="7420c-123">Нет</span><span class="sxs-lookup"><span data-stu-id="7420c-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7420c-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7420c-124">JSON Representation</span></span>
<span data-ttu-id="7420c-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7420c-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppSupportedDeviceType",
  "type": "String",
  "minimumOperatingSystemVersion": "String",
  "maximumOperatingSystemVersion": "String"
}
```




