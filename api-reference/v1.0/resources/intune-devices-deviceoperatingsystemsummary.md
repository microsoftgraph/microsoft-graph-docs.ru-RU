---
title: Тип ресурса deviceOperatingSystemSummary
description: Общие сведения об операционной системе устройства.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 82eb7fe0feb0f410a0ef80ab6756aa499f73b71d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533265"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="d03f9-103">Тип ресурса deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="d03f9-103">deviceOperatingSystemSummary resource type</span></span>

<span data-ttu-id="d03f9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d03f9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d03f9-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d03f9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d03f9-106">Общие сведения об операционной системе устройства.</span><span class="sxs-lookup"><span data-stu-id="d03f9-106">Device operating system summary.</span></span>

## <a name="properties"></a><span data-ttu-id="d03f9-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d03f9-107">Properties</span></span>
|<span data-ttu-id="d03f9-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d03f9-108">Property</span></span>|<span data-ttu-id="d03f9-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d03f9-109">Type</span></span>|<span data-ttu-id="d03f9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d03f9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d03f9-111">androidCount</span><span class="sxs-lookup"><span data-stu-id="d03f9-111">androidCount</span></span>|<span data-ttu-id="d03f9-112">Int32</span><span class="sxs-lookup"><span data-stu-id="d03f9-112">Int32</span></span>|<span data-ttu-id="d03f9-113">Количество устройств с Android.</span><span class="sxs-lookup"><span data-stu-id="d03f9-113">Number of android device count.</span></span>|
|<span data-ttu-id="d03f9-114">iosCount</span><span class="sxs-lookup"><span data-stu-id="d03f9-114">iosCount</span></span>|<span data-ttu-id="d03f9-115">Int32</span><span class="sxs-lookup"><span data-stu-id="d03f9-115">Int32</span></span>|<span data-ttu-id="d03f9-116">Количество устройств с iOS.</span><span class="sxs-lookup"><span data-stu-id="d03f9-116">Number of iOS device count.</span></span>|
|<span data-ttu-id="d03f9-117">macOSCount</span><span class="sxs-lookup"><span data-stu-id="d03f9-117">macOSCount</span></span>|<span data-ttu-id="d03f9-118">Int32</span><span class="sxs-lookup"><span data-stu-id="d03f9-118">Int32</span></span>|<span data-ttu-id="d03f9-119">Количество устройств с Mac OS X.</span><span class="sxs-lookup"><span data-stu-id="d03f9-119">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="d03f9-120">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="d03f9-120">windowsMobileCount</span></span>|<span data-ttu-id="d03f9-121">Int32</span><span class="sxs-lookup"><span data-stu-id="d03f9-121">Int32</span></span>|<span data-ttu-id="d03f9-122">Количество мобильных устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="d03f9-122">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="d03f9-123">windowsCount</span><span class="sxs-lookup"><span data-stu-id="d03f9-123">windowsCount</span></span>|<span data-ttu-id="d03f9-124">Int32</span><span class="sxs-lookup"><span data-stu-id="d03f9-124">Int32</span></span>|<span data-ttu-id="d03f9-125">Количество устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="d03f9-125">Number of Windows device count.</span></span>|
|<span data-ttu-id="d03f9-126">unknownCount</span><span class="sxs-lookup"><span data-stu-id="d03f9-126">unknownCount</span></span>|<span data-ttu-id="d03f9-127">Int32</span><span class="sxs-lookup"><span data-stu-id="d03f9-127">Int32</span></span>|<span data-ttu-id="d03f9-128">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="d03f9-128">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d03f9-129">Связи</span><span class="sxs-lookup"><span data-stu-id="d03f9-129">Relationships</span></span>
<span data-ttu-id="d03f9-130">Нет</span><span class="sxs-lookup"><span data-stu-id="d03f9-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d03f9-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d03f9-131">JSON Representation</span></span>
<span data-ttu-id="d03f9-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d03f9-132">Here is a JSON representation of the resource.</span></span>
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




