---
title: Тип ресурса mobileAppSupportedDeviceType
description: Свойства устройства
ms.openlocfilehash: 7bea84a009d8940608c82bbb551c2d3c8be750ce
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077178"
---
# <a name="mobileappsupporteddevicetype-resource-type"></a><span data-ttu-id="2abb9-103">Тип ресурса mobileAppSupportedDeviceType</span><span class="sxs-lookup"><span data-stu-id="2abb9-103">mobileAppSupportedDeviceType resource type</span></span>

> <span data-ttu-id="2abb9-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2abb9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2abb9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2abb9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2abb9-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2abb9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2abb9-107">Свойства устройства</span><span class="sxs-lookup"><span data-stu-id="2abb9-107">Device properties</span></span>
## <a name="properties"></a><span data-ttu-id="2abb9-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="2abb9-108">Properties</span></span>
|<span data-ttu-id="2abb9-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="2abb9-109">Property</span></span>|<span data-ttu-id="2abb9-110">Тип</span><span class="sxs-lookup"><span data-stu-id="2abb9-110">Type</span></span>|<span data-ttu-id="2abb9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2abb9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2abb9-112">type</span><span class="sxs-lookup"><span data-stu-id="2abb9-112">type</span></span>|[<span data-ttu-id="2abb9-113">deviceType</span><span class="sxs-lookup"><span data-stu-id="2abb9-113">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="2abb9-114">Тип устройства.</span><span class="sxs-lookup"><span data-stu-id="2abb9-114">Device type.</span></span> <span data-ttu-id="2abb9-115">Возможные значения: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="2abb9-115">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="2abb9-116">minimumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="2abb9-116">minimumOperatingSystemVersion</span></span>|<span data-ttu-id="2abb9-117">String</span><span class="sxs-lookup"><span data-stu-id="2abb9-117">String</span></span>|<span data-ttu-id="2abb9-118">Минимальная версия операционной системы</span><span class="sxs-lookup"><span data-stu-id="2abb9-118">Minimum OS version</span></span>|
|<span data-ttu-id="2abb9-119">maximumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="2abb9-119">maximumOperatingSystemVersion</span></span>|<span data-ttu-id="2abb9-120">String</span><span class="sxs-lookup"><span data-stu-id="2abb9-120">String</span></span>|<span data-ttu-id="2abb9-121">Максимальная версия ОС</span><span class="sxs-lookup"><span data-stu-id="2abb9-121">Maximum OS version</span></span>|

## <a name="relationships"></a><span data-ttu-id="2abb9-122">Связи</span><span class="sxs-lookup"><span data-stu-id="2abb9-122">Relationships</span></span>
<span data-ttu-id="2abb9-123">Нет</span><span class="sxs-lookup"><span data-stu-id="2abb9-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2abb9-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2abb9-124">JSON Representation</span></span>
<span data-ttu-id="2abb9-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2abb9-125">Here is a JSON representation of the resource.</span></span>
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





