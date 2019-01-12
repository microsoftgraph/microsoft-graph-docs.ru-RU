---
title: Тип ресурса mobileAppSupportedDeviceType
description: Свойства устройства
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b1b757e9c621f77d1a26251345ee6751eca2ca7c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980225"
---
# <a name="mobileappsupporteddevicetype-resource-type"></a><span data-ttu-id="a5be4-103">Тип ресурса mobileAppSupportedDeviceType</span><span class="sxs-lookup"><span data-stu-id="a5be4-103">mobileAppSupportedDeviceType resource type</span></span>

> <span data-ttu-id="a5be4-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a5be4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a5be4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5be4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a5be4-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a5be4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a5be4-107">Свойства устройства</span><span class="sxs-lookup"><span data-stu-id="a5be4-107">Device properties</span></span>
## <a name="properties"></a><span data-ttu-id="a5be4-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a5be4-108">Properties</span></span>
|<span data-ttu-id="a5be4-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a5be4-109">Property</span></span>|<span data-ttu-id="a5be4-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a5be4-110">Type</span></span>|<span data-ttu-id="a5be4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a5be4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5be4-112">type</span><span class="sxs-lookup"><span data-stu-id="a5be4-112">type</span></span>|[<span data-ttu-id="a5be4-113">deviceType</span><span class="sxs-lookup"><span data-stu-id="a5be4-113">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="a5be4-114">Тип устройства.</span><span class="sxs-lookup"><span data-stu-id="a5be4-114">Device type.</span></span> <span data-ttu-id="a5be4-115">Возможные значения: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="a5be4-115">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="a5be4-116">minimumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="a5be4-116">minimumOperatingSystemVersion</span></span>|<span data-ttu-id="a5be4-117">Строка</span><span class="sxs-lookup"><span data-stu-id="a5be4-117">String</span></span>|<span data-ttu-id="a5be4-118">Минимальная версия операционной системы</span><span class="sxs-lookup"><span data-stu-id="a5be4-118">Minimum OS version</span></span>|
|<span data-ttu-id="a5be4-119">maximumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="a5be4-119">maximumOperatingSystemVersion</span></span>|<span data-ttu-id="a5be4-120">Строка</span><span class="sxs-lookup"><span data-stu-id="a5be4-120">String</span></span>|<span data-ttu-id="a5be4-121">Максимальная версия ОС</span><span class="sxs-lookup"><span data-stu-id="a5be4-121">Maximum OS version</span></span>|

## <a name="relationships"></a><span data-ttu-id="a5be4-122">Связи</span><span class="sxs-lookup"><span data-stu-id="a5be4-122">Relationships</span></span>
<span data-ttu-id="a5be4-123">Нет</span><span class="sxs-lookup"><span data-stu-id="a5be4-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a5be4-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a5be4-124">JSON Representation</span></span>
<span data-ttu-id="a5be4-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a5be4-125">Here is a JSON representation of the resource.</span></span>
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





