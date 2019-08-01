---
title: Тип ресурса deviceOperatingSystemSummary
description: Общие сведения об операционной системе устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9877dba58817e8c6dad3676cb6a646750408d4e4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030760"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="902fa-103">Тип ресурса deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="902fa-103">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="902fa-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="902fa-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="902fa-105">Общие сведения об операционной системе устройства.</span><span class="sxs-lookup"><span data-stu-id="902fa-105">Device operating system summary.</span></span>

## <a name="properties"></a><span data-ttu-id="902fa-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="902fa-106">Properties</span></span>
|<span data-ttu-id="902fa-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="902fa-107">Property</span></span>|<span data-ttu-id="902fa-108">Тип</span><span class="sxs-lookup"><span data-stu-id="902fa-108">Type</span></span>|<span data-ttu-id="902fa-109">Описание</span><span class="sxs-lookup"><span data-stu-id="902fa-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="902fa-110">androidCount</span><span class="sxs-lookup"><span data-stu-id="902fa-110">androidCount</span></span>|<span data-ttu-id="902fa-111">Int32</span><span class="sxs-lookup"><span data-stu-id="902fa-111">Int32</span></span>|<span data-ttu-id="902fa-112">Количество устройств с Android.</span><span class="sxs-lookup"><span data-stu-id="902fa-112">Number of android device count.</span></span>|
|<span data-ttu-id="902fa-113">iosCount</span><span class="sxs-lookup"><span data-stu-id="902fa-113">iosCount</span></span>|<span data-ttu-id="902fa-114">Int32</span><span class="sxs-lookup"><span data-stu-id="902fa-114">Int32</span></span>|<span data-ttu-id="902fa-115">Количество устройств с iOS.</span><span class="sxs-lookup"><span data-stu-id="902fa-115">Number of iOS device count.</span></span>|
|<span data-ttu-id="902fa-116">macOSCount</span><span class="sxs-lookup"><span data-stu-id="902fa-116">macOSCount</span></span>|<span data-ttu-id="902fa-117">Int32</span><span class="sxs-lookup"><span data-stu-id="902fa-117">Int32</span></span>|<span data-ttu-id="902fa-118">Количество устройств с Mac OS X.</span><span class="sxs-lookup"><span data-stu-id="902fa-118">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="902fa-119">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="902fa-119">windowsMobileCount</span></span>|<span data-ttu-id="902fa-120">Int32</span><span class="sxs-lookup"><span data-stu-id="902fa-120">Int32</span></span>|<span data-ttu-id="902fa-121">Количество мобильных устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="902fa-121">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="902fa-122">windowsCount</span><span class="sxs-lookup"><span data-stu-id="902fa-122">windowsCount</span></span>|<span data-ttu-id="902fa-123">Int32</span><span class="sxs-lookup"><span data-stu-id="902fa-123">Int32</span></span>|<span data-ttu-id="902fa-124">Количество устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="902fa-124">Number of Windows device count.</span></span>|
|<span data-ttu-id="902fa-125">unknownCount</span><span class="sxs-lookup"><span data-stu-id="902fa-125">unknownCount</span></span>|<span data-ttu-id="902fa-126">Int32</span><span class="sxs-lookup"><span data-stu-id="902fa-126">Int32</span></span>|<span data-ttu-id="902fa-127">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="902fa-127">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="902fa-128">Отношения</span><span class="sxs-lookup"><span data-stu-id="902fa-128">Relationships</span></span>
<span data-ttu-id="902fa-129">Нет</span><span class="sxs-lookup"><span data-stu-id="902fa-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="902fa-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="902fa-130">JSON Representation</span></span>
<span data-ttu-id="902fa-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="902fa-131">Here is a JSON representation of the resource.</span></span>
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



