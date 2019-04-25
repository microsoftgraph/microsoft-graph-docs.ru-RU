---
title: Тип ресурса deviceOperatingSystemSummary
description: Общие сведения об операционной системе устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 13bfc5d8d4e85f31b178801becd56e744a40c106
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32521357"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="b1590-103">Тип ресурса deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="b1590-103">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="b1590-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1590-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1590-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b1590-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1590-106">Общие сведения об операционной системе устройства.</span><span class="sxs-lookup"><span data-stu-id="b1590-106">Device operating system summary.</span></span>

## <a name="properties"></a><span data-ttu-id="b1590-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b1590-107">Properties</span></span>
|<span data-ttu-id="b1590-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b1590-108">Property</span></span>|<span data-ttu-id="b1590-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b1590-109">Type</span></span>|<span data-ttu-id="b1590-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b1590-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1590-111">androidCount</span><span class="sxs-lookup"><span data-stu-id="b1590-111">androidCount</span></span>|<span data-ttu-id="b1590-112">Int32</span><span class="sxs-lookup"><span data-stu-id="b1590-112">Int32</span></span>|<span data-ttu-id="b1590-113">Количество устройств с Android.</span><span class="sxs-lookup"><span data-stu-id="b1590-113">Number of android device count.</span></span>|
|<span data-ttu-id="b1590-114">iosCount</span><span class="sxs-lookup"><span data-stu-id="b1590-114">iosCount</span></span>|<span data-ttu-id="b1590-115">Int32</span><span class="sxs-lookup"><span data-stu-id="b1590-115">Int32</span></span>|<span data-ttu-id="b1590-116">Количество устройств с iOS.</span><span class="sxs-lookup"><span data-stu-id="b1590-116">Number of iOS device count.</span></span>|
|<span data-ttu-id="b1590-117">macOSCount</span><span class="sxs-lookup"><span data-stu-id="b1590-117">macOSCount</span></span>|<span data-ttu-id="b1590-118">Int32</span><span class="sxs-lookup"><span data-stu-id="b1590-118">Int32</span></span>|<span data-ttu-id="b1590-119">Количество устройств с Mac OS X.</span><span class="sxs-lookup"><span data-stu-id="b1590-119">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="b1590-120">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="b1590-120">windowsMobileCount</span></span>|<span data-ttu-id="b1590-121">Int32</span><span class="sxs-lookup"><span data-stu-id="b1590-121">Int32</span></span>|<span data-ttu-id="b1590-122">Количество мобильных устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="b1590-122">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="b1590-123">windowsCount</span><span class="sxs-lookup"><span data-stu-id="b1590-123">windowsCount</span></span>|<span data-ttu-id="b1590-124">Int32</span><span class="sxs-lookup"><span data-stu-id="b1590-124">Int32</span></span>|<span data-ttu-id="b1590-125">Количество устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="b1590-125">Number of Windows device count.</span></span>|
|<span data-ttu-id="b1590-126">unknownCount</span><span class="sxs-lookup"><span data-stu-id="b1590-126">unknownCount</span></span>|<span data-ttu-id="b1590-127">Int32</span><span class="sxs-lookup"><span data-stu-id="b1590-127">Int32</span></span>|<span data-ttu-id="b1590-128">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="b1590-128">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b1590-129">Отношения</span><span class="sxs-lookup"><span data-stu-id="b1590-129">Relationships</span></span>
<span data-ttu-id="b1590-130">Нет</span><span class="sxs-lookup"><span data-stu-id="b1590-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b1590-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b1590-131">JSON Representation</span></span>
<span data-ttu-id="b1590-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b1590-132">Here is a JSON representation of the resource.</span></span>
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





