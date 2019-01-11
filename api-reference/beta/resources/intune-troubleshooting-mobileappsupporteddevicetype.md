---
title: Тип ресурса mobileAppSupportedDeviceType
description: Свойства устройства
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1d261b35b5de64057ca2dcdbe516081909523548
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858550"
---
# <a name="mobileappsupporteddevicetype-resource-type"></a><span data-ttu-id="d2767-103">Тип ресурса mobileAppSupportedDeviceType</span><span class="sxs-lookup"><span data-stu-id="d2767-103">mobileAppSupportedDeviceType resource type</span></span>

> <span data-ttu-id="d2767-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d2767-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d2767-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2767-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d2767-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d2767-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d2767-107">Свойства устройства</span><span class="sxs-lookup"><span data-stu-id="d2767-107">Device properties</span></span>
## <a name="properties"></a><span data-ttu-id="d2767-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d2767-108">Properties</span></span>
|<span data-ttu-id="d2767-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d2767-109">Property</span></span>|<span data-ttu-id="d2767-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d2767-110">Type</span></span>|<span data-ttu-id="d2767-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d2767-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2767-112">type</span><span class="sxs-lookup"><span data-stu-id="d2767-112">type</span></span>|[<span data-ttu-id="d2767-113">deviceType</span><span class="sxs-lookup"><span data-stu-id="d2767-113">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="d2767-114">Тип устройства.</span><span class="sxs-lookup"><span data-stu-id="d2767-114">Device type.</span></span> <span data-ttu-id="d2767-115">Возможные значения: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="d2767-115">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="d2767-116">minimumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="d2767-116">minimumOperatingSystemVersion</span></span>|<span data-ttu-id="d2767-117">Строка</span><span class="sxs-lookup"><span data-stu-id="d2767-117">String</span></span>|<span data-ttu-id="d2767-118">Минимальная версия операционной системы</span><span class="sxs-lookup"><span data-stu-id="d2767-118">Minimum OS version</span></span>|
|<span data-ttu-id="d2767-119">maximumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="d2767-119">maximumOperatingSystemVersion</span></span>|<span data-ttu-id="d2767-120">Строка</span><span class="sxs-lookup"><span data-stu-id="d2767-120">String</span></span>|<span data-ttu-id="d2767-121">Максимальная версия ОС</span><span class="sxs-lookup"><span data-stu-id="d2767-121">Maximum OS version</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2767-122">Связи</span><span class="sxs-lookup"><span data-stu-id="d2767-122">Relationships</span></span>
<span data-ttu-id="d2767-123">Нет</span><span class="sxs-lookup"><span data-stu-id="d2767-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d2767-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d2767-124">JSON Representation</span></span>
<span data-ttu-id="d2767-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d2767-125">Here is a JSON representation of the resource.</span></span>
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





