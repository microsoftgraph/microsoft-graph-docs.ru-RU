---
title: Тип ресурса deviceOperatingSystemSummary
description: Общие сведения об операционной системе устройства.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 62fe2496e505ac0d281381b9d53604aa98094f3c
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356941"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="0f1ee-103">Тип ресурса deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="0f1ee-103">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="0f1ee-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0f1ee-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f1ee-105">Общие сведения об операционной системе устройства.</span><span class="sxs-lookup"><span data-stu-id="0f1ee-105">Device operating system summary.</span></span>

## <a name="properties"></a><span data-ttu-id="0f1ee-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="0f1ee-106">Properties</span></span>
|<span data-ttu-id="0f1ee-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="0f1ee-107">Property</span></span>|<span data-ttu-id="0f1ee-108">Тип</span><span class="sxs-lookup"><span data-stu-id="0f1ee-108">Type</span></span>|<span data-ttu-id="0f1ee-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0f1ee-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f1ee-110">androidCount</span><span class="sxs-lookup"><span data-stu-id="0f1ee-110">androidCount</span></span>|<span data-ttu-id="0f1ee-111">Int32</span><span class="sxs-lookup"><span data-stu-id="0f1ee-111">Int32</span></span>|<span data-ttu-id="0f1ee-112">Количество устройств с Android.</span><span class="sxs-lookup"><span data-stu-id="0f1ee-112">Number of android device count.</span></span>|
|<span data-ttu-id="0f1ee-113">iosCount</span><span class="sxs-lookup"><span data-stu-id="0f1ee-113">iosCount</span></span>|<span data-ttu-id="0f1ee-114">Int32</span><span class="sxs-lookup"><span data-stu-id="0f1ee-114">Int32</span></span>|<span data-ttu-id="0f1ee-115">Количество устройств с iOS.</span><span class="sxs-lookup"><span data-stu-id="0f1ee-115">Number of iOS device count.</span></span>|
|<span data-ttu-id="0f1ee-116">macOSCount</span><span class="sxs-lookup"><span data-stu-id="0f1ee-116">macOSCount</span></span>|<span data-ttu-id="0f1ee-117">Int32</span><span class="sxs-lookup"><span data-stu-id="0f1ee-117">Int32</span></span>|<span data-ttu-id="0f1ee-118">Количество устройств с Mac OS X.</span><span class="sxs-lookup"><span data-stu-id="0f1ee-118">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="0f1ee-119">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="0f1ee-119">windowsMobileCount</span></span>|<span data-ttu-id="0f1ee-120">Int32</span><span class="sxs-lookup"><span data-stu-id="0f1ee-120">Int32</span></span>|<span data-ttu-id="0f1ee-121">Количество мобильных устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="0f1ee-121">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="0f1ee-122">windowsCount</span><span class="sxs-lookup"><span data-stu-id="0f1ee-122">windowsCount</span></span>|<span data-ttu-id="0f1ee-123">Int32</span><span class="sxs-lookup"><span data-stu-id="0f1ee-123">Int32</span></span>|<span data-ttu-id="0f1ee-124">Количество устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="0f1ee-124">Number of Windows device count.</span></span>|
|<span data-ttu-id="0f1ee-125">unknownCount</span><span class="sxs-lookup"><span data-stu-id="0f1ee-125">unknownCount</span></span>|<span data-ttu-id="0f1ee-126">Int32</span><span class="sxs-lookup"><span data-stu-id="0f1ee-126">Int32</span></span>|<span data-ttu-id="0f1ee-127">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="0f1ee-127">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f1ee-128">Связи</span><span class="sxs-lookup"><span data-stu-id="0f1ee-128">Relationships</span></span>
<span data-ttu-id="0f1ee-129">Нет</span><span class="sxs-lookup"><span data-stu-id="0f1ee-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0f1ee-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0f1ee-130">JSON Representation</span></span>
<span data-ttu-id="0f1ee-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0f1ee-131">Here is a JSON representation of the resource.</span></span>
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




