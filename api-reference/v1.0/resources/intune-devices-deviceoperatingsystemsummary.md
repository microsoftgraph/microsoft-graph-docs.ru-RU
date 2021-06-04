---
title: Тип ресурса deviceOperatingSystemSummary
description: Общие сведения об операционной системе устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9dfce6c0947fffd861ae1cda205c1011a7500471
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754569"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="a0ba5-103">Тип ресурса deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="a0ba5-103">deviceOperatingSystemSummary resource type</span></span>

<span data-ttu-id="a0ba5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0ba5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a0ba5-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a0ba5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0ba5-106">Общие сведения об операционной системе устройства.</span><span class="sxs-lookup"><span data-stu-id="a0ba5-106">Device operating system summary.</span></span>

## <a name="properties"></a><span data-ttu-id="a0ba5-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a0ba5-107">Properties</span></span>
|<span data-ttu-id="a0ba5-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a0ba5-108">Property</span></span>|<span data-ttu-id="a0ba5-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a0ba5-109">Type</span></span>|<span data-ttu-id="a0ba5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a0ba5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0ba5-111">androidCount</span><span class="sxs-lookup"><span data-stu-id="a0ba5-111">androidCount</span></span>|<span data-ttu-id="a0ba5-112">Int32</span><span class="sxs-lookup"><span data-stu-id="a0ba5-112">Int32</span></span>|<span data-ttu-id="a0ba5-113">Количество устройств с Android.</span><span class="sxs-lookup"><span data-stu-id="a0ba5-113">Number of android device count.</span></span>|
|<span data-ttu-id="a0ba5-114">iosCount</span><span class="sxs-lookup"><span data-stu-id="a0ba5-114">iosCount</span></span>|<span data-ttu-id="a0ba5-115">Int32</span><span class="sxs-lookup"><span data-stu-id="a0ba5-115">Int32</span></span>|<span data-ttu-id="a0ba5-116">Количество устройств с iOS.</span><span class="sxs-lookup"><span data-stu-id="a0ba5-116">Number of iOS device count.</span></span>|
|<span data-ttu-id="a0ba5-117">macOSCount</span><span class="sxs-lookup"><span data-stu-id="a0ba5-117">macOSCount</span></span>|<span data-ttu-id="a0ba5-118">Int32</span><span class="sxs-lookup"><span data-stu-id="a0ba5-118">Int32</span></span>|<span data-ttu-id="a0ba5-119">Количество устройств с Mac OS X.</span><span class="sxs-lookup"><span data-stu-id="a0ba5-119">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="a0ba5-120">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="a0ba5-120">windowsMobileCount</span></span>|<span data-ttu-id="a0ba5-121">Int32</span><span class="sxs-lookup"><span data-stu-id="a0ba5-121">Int32</span></span>|<span data-ttu-id="a0ba5-122">Количество мобильных устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="a0ba5-122">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="a0ba5-123">windowsCount</span><span class="sxs-lookup"><span data-stu-id="a0ba5-123">windowsCount</span></span>|<span data-ttu-id="a0ba5-124">Int32</span><span class="sxs-lookup"><span data-stu-id="a0ba5-124">Int32</span></span>|<span data-ttu-id="a0ba5-125">Количество устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="a0ba5-125">Number of Windows device count.</span></span>|
|<span data-ttu-id="a0ba5-126">unknownCount</span><span class="sxs-lookup"><span data-stu-id="a0ba5-126">unknownCount</span></span>|<span data-ttu-id="a0ba5-127">Int32</span><span class="sxs-lookup"><span data-stu-id="a0ba5-127">Int32</span></span>|<span data-ttu-id="a0ba5-128">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="a0ba5-128">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a0ba5-129">Отношения</span><span class="sxs-lookup"><span data-stu-id="a0ba5-129">Relationships</span></span>
<span data-ttu-id="a0ba5-130">Нет</span><span class="sxs-lookup"><span data-stu-id="a0ba5-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a0ba5-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a0ba5-131">JSON Representation</span></span>
<span data-ttu-id="a0ba5-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a0ba5-132">Here is a JSON representation of the resource.</span></span>
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




