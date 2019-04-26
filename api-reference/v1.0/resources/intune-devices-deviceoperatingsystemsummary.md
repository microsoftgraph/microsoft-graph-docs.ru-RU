---
title: Тип ресурса deviceOperatingSystemSummary
description: Общие сведения об операционной системе устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 53c806e250d6b201e6dfe49d90685c4144913182
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32574077"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="5f727-103">Тип ресурса deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="5f727-103">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="5f727-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5f727-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f727-105">Общие сведения об операционной системе устройства.</span><span class="sxs-lookup"><span data-stu-id="5f727-105">Device operating system summary.</span></span>

## <a name="properties"></a><span data-ttu-id="5f727-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="5f727-106">Properties</span></span>
|<span data-ttu-id="5f727-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="5f727-107">Property</span></span>|<span data-ttu-id="5f727-108">Тип</span><span class="sxs-lookup"><span data-stu-id="5f727-108">Type</span></span>|<span data-ttu-id="5f727-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5f727-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f727-110">androidCount</span><span class="sxs-lookup"><span data-stu-id="5f727-110">androidCount</span></span>|<span data-ttu-id="5f727-111">Int32</span><span class="sxs-lookup"><span data-stu-id="5f727-111">Int32</span></span>|<span data-ttu-id="5f727-112">Количество устройств с Android.</span><span class="sxs-lookup"><span data-stu-id="5f727-112">Number of android device count.</span></span>|
|<span data-ttu-id="5f727-113">iosCount</span><span class="sxs-lookup"><span data-stu-id="5f727-113">iosCount</span></span>|<span data-ttu-id="5f727-114">Int32</span><span class="sxs-lookup"><span data-stu-id="5f727-114">Int32</span></span>|<span data-ttu-id="5f727-115">Количество устройств с iOS.</span><span class="sxs-lookup"><span data-stu-id="5f727-115">Number of iOS device count.</span></span>|
|<span data-ttu-id="5f727-116">macOSCount</span><span class="sxs-lookup"><span data-stu-id="5f727-116">macOSCount</span></span>|<span data-ttu-id="5f727-117">Int32</span><span class="sxs-lookup"><span data-stu-id="5f727-117">Int32</span></span>|<span data-ttu-id="5f727-118">Количество устройств с Mac OS X.</span><span class="sxs-lookup"><span data-stu-id="5f727-118">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="5f727-119">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="5f727-119">windowsMobileCount</span></span>|<span data-ttu-id="5f727-120">Int32</span><span class="sxs-lookup"><span data-stu-id="5f727-120">Int32</span></span>|<span data-ttu-id="5f727-121">Количество мобильных устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="5f727-121">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="5f727-122">windowsCount</span><span class="sxs-lookup"><span data-stu-id="5f727-122">windowsCount</span></span>|<span data-ttu-id="5f727-123">Int32</span><span class="sxs-lookup"><span data-stu-id="5f727-123">Int32</span></span>|<span data-ttu-id="5f727-124">Количество устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="5f727-124">Number of Windows device count.</span></span>|
|<span data-ttu-id="5f727-125">unknownCount</span><span class="sxs-lookup"><span data-stu-id="5f727-125">unknownCount</span></span>|<span data-ttu-id="5f727-126">Int32</span><span class="sxs-lookup"><span data-stu-id="5f727-126">Int32</span></span>|<span data-ttu-id="5f727-127">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="5f727-127">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5f727-128">Отношения</span><span class="sxs-lookup"><span data-stu-id="5f727-128">Relationships</span></span>
<span data-ttu-id="5f727-129">Нет</span><span class="sxs-lookup"><span data-stu-id="5f727-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5f727-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5f727-130">JSON Representation</span></span>
<span data-ttu-id="5f727-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5f727-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceOperatingSystemSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceOperatingSystemSummary",
  "androidCount": 1024,
  "iosCount": 1024,
  "macOSCount": 1024,
  "windowsMobileCount": 1024,
  "windowsCount": 1024,
  "unknownCount": 1024
}
```



