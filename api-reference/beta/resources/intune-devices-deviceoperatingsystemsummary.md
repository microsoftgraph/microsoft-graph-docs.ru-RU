---
title: Тип ресурса deviceOperatingSystemSummary
description: Общие сведения об операционной системе устройства.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0a9e628a52a90f72dbf67495c8e6745bd4072ca2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369985"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="a890f-103">Тип ресурса deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="a890f-103">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="a890f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a890f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a890f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a890f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a890f-106">Общие сведения об операционной системе устройства.</span><span class="sxs-lookup"><span data-stu-id="a890f-106">Device operating system summary.</span></span>

## <a name="properties"></a><span data-ttu-id="a890f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a890f-107">Properties</span></span>
|<span data-ttu-id="a890f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a890f-108">Property</span></span>|<span data-ttu-id="a890f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a890f-109">Type</span></span>|<span data-ttu-id="a890f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a890f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a890f-111">androidCount</span><span class="sxs-lookup"><span data-stu-id="a890f-111">androidCount</span></span>|<span data-ttu-id="a890f-112">Int32</span><span class="sxs-lookup"><span data-stu-id="a890f-112">Int32</span></span>|<span data-ttu-id="a890f-113">Количество устройств с Android.</span><span class="sxs-lookup"><span data-stu-id="a890f-113">Number of android device count.</span></span>|
|<span data-ttu-id="a890f-114">iosCount</span><span class="sxs-lookup"><span data-stu-id="a890f-114">iosCount</span></span>|<span data-ttu-id="a890f-115">Int32</span><span class="sxs-lookup"><span data-stu-id="a890f-115">Int32</span></span>|<span data-ttu-id="a890f-116">Количество устройств с iOS.</span><span class="sxs-lookup"><span data-stu-id="a890f-116">Number of iOS device count.</span></span>|
|<span data-ttu-id="a890f-117">macOSCount</span><span class="sxs-lookup"><span data-stu-id="a890f-117">macOSCount</span></span>|<span data-ttu-id="a890f-118">Int32</span><span class="sxs-lookup"><span data-stu-id="a890f-118">Int32</span></span>|<span data-ttu-id="a890f-119">Количество устройств с Mac OS X.</span><span class="sxs-lookup"><span data-stu-id="a890f-119">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="a890f-120">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="a890f-120">windowsMobileCount</span></span>|<span data-ttu-id="a890f-121">Int32</span><span class="sxs-lookup"><span data-stu-id="a890f-121">Int32</span></span>|<span data-ttu-id="a890f-122">Количество мобильных устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="a890f-122">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="a890f-123">windowsCount</span><span class="sxs-lookup"><span data-stu-id="a890f-123">windowsCount</span></span>|<span data-ttu-id="a890f-124">Int32</span><span class="sxs-lookup"><span data-stu-id="a890f-124">Int32</span></span>|<span data-ttu-id="a890f-125">Количество устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="a890f-125">Number of Windows device count.</span></span>|
|<span data-ttu-id="a890f-126">unknownCount</span><span class="sxs-lookup"><span data-stu-id="a890f-126">unknownCount</span></span>|<span data-ttu-id="a890f-127">Int32</span><span class="sxs-lookup"><span data-stu-id="a890f-127">Int32</span></span>|<span data-ttu-id="a890f-128">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="a890f-128">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a890f-129">Отношения</span><span class="sxs-lookup"><span data-stu-id="a890f-129">Relationships</span></span>
<span data-ttu-id="a890f-130">Нет</span><span class="sxs-lookup"><span data-stu-id="a890f-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a890f-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a890f-131">JSON Representation</span></span>
<span data-ttu-id="a890f-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a890f-132">Here is a JSON representation of the resource.</span></span>
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



