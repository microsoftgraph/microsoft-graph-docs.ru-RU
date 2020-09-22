---
title: Тип ресурса deviceOperatingSystemSummary
description: Общие сведения об операционной системе устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b076a49036a3f438e93af5472a0ab9fe1bcb59a0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091182"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="575c8-103">Тип ресурса deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="575c8-103">deviceOperatingSystemSummary resource type</span></span>

<span data-ttu-id="575c8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="575c8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="575c8-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="575c8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="575c8-106">Общие сведения об операционной системе устройства.</span><span class="sxs-lookup"><span data-stu-id="575c8-106">Device operating system summary.</span></span>

## <a name="properties"></a><span data-ttu-id="575c8-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="575c8-107">Properties</span></span>
|<span data-ttu-id="575c8-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="575c8-108">Property</span></span>|<span data-ttu-id="575c8-109">Тип</span><span class="sxs-lookup"><span data-stu-id="575c8-109">Type</span></span>|<span data-ttu-id="575c8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="575c8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="575c8-111">androidCount</span><span class="sxs-lookup"><span data-stu-id="575c8-111">androidCount</span></span>|<span data-ttu-id="575c8-112">Int32</span><span class="sxs-lookup"><span data-stu-id="575c8-112">Int32</span></span>|<span data-ttu-id="575c8-113">Количество устройств с Android.</span><span class="sxs-lookup"><span data-stu-id="575c8-113">Number of android device count.</span></span>|
|<span data-ttu-id="575c8-114">iosCount</span><span class="sxs-lookup"><span data-stu-id="575c8-114">iosCount</span></span>|<span data-ttu-id="575c8-115">Int32</span><span class="sxs-lookup"><span data-stu-id="575c8-115">Int32</span></span>|<span data-ttu-id="575c8-116">Количество устройств с iOS.</span><span class="sxs-lookup"><span data-stu-id="575c8-116">Number of iOS device count.</span></span>|
|<span data-ttu-id="575c8-117">macOSCount</span><span class="sxs-lookup"><span data-stu-id="575c8-117">macOSCount</span></span>|<span data-ttu-id="575c8-118">Int32</span><span class="sxs-lookup"><span data-stu-id="575c8-118">Int32</span></span>|<span data-ttu-id="575c8-119">Количество устройств с Mac OS X.</span><span class="sxs-lookup"><span data-stu-id="575c8-119">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="575c8-120">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="575c8-120">windowsMobileCount</span></span>|<span data-ttu-id="575c8-121">Int32</span><span class="sxs-lookup"><span data-stu-id="575c8-121">Int32</span></span>|<span data-ttu-id="575c8-122">Количество мобильных устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="575c8-122">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="575c8-123">windowsCount</span><span class="sxs-lookup"><span data-stu-id="575c8-123">windowsCount</span></span>|<span data-ttu-id="575c8-124">Int32</span><span class="sxs-lookup"><span data-stu-id="575c8-124">Int32</span></span>|<span data-ttu-id="575c8-125">Количество устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="575c8-125">Number of Windows device count.</span></span>|
|<span data-ttu-id="575c8-126">unknownCount</span><span class="sxs-lookup"><span data-stu-id="575c8-126">unknownCount</span></span>|<span data-ttu-id="575c8-127">Int32</span><span class="sxs-lookup"><span data-stu-id="575c8-127">Int32</span></span>|<span data-ttu-id="575c8-128">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="575c8-128">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="575c8-129">Связи</span><span class="sxs-lookup"><span data-stu-id="575c8-129">Relationships</span></span>
<span data-ttu-id="575c8-130">Нет</span><span class="sxs-lookup"><span data-stu-id="575c8-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="575c8-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="575c8-131">JSON Representation</span></span>
<span data-ttu-id="575c8-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="575c8-132">Here is a JSON representation of the resource.</span></span>
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









