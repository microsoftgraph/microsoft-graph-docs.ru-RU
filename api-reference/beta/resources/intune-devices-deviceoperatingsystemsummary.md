---
title: Тип ресурса deviceOperatingSystemSummary
description: Общие сведения об операционной системе устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: fbb82189e9d8153cef28e516169351272195fa30
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918464"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="207f1-103">Тип ресурса deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="207f1-103">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="207f1-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="207f1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="207f1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="207f1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="207f1-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="207f1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="207f1-107">Общие сведения об операционной системе устройства.</span><span class="sxs-lookup"><span data-stu-id="207f1-107">Device operating system summary.</span></span>
## <a name="properties"></a><span data-ttu-id="207f1-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="207f1-108">Properties</span></span>
|<span data-ttu-id="207f1-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="207f1-109">Property</span></span>|<span data-ttu-id="207f1-110">Тип</span><span class="sxs-lookup"><span data-stu-id="207f1-110">Type</span></span>|<span data-ttu-id="207f1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="207f1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="207f1-112">androidCount</span><span class="sxs-lookup"><span data-stu-id="207f1-112">androidCount</span></span>|<span data-ttu-id="207f1-113">Int32</span><span class="sxs-lookup"><span data-stu-id="207f1-113">Int32</span></span>|<span data-ttu-id="207f1-114">Количество устройств с Android.</span><span class="sxs-lookup"><span data-stu-id="207f1-114">Number of android device count.</span></span>|
|<span data-ttu-id="207f1-115">iosCount</span><span class="sxs-lookup"><span data-stu-id="207f1-115">iosCount</span></span>|<span data-ttu-id="207f1-116">Int32</span><span class="sxs-lookup"><span data-stu-id="207f1-116">Int32</span></span>|<span data-ttu-id="207f1-117">Количество устройств с iOS.</span><span class="sxs-lookup"><span data-stu-id="207f1-117">Number of iOS device count.</span></span>|
|<span data-ttu-id="207f1-118">macOSCount</span><span class="sxs-lookup"><span data-stu-id="207f1-118">macOSCount</span></span>|<span data-ttu-id="207f1-119">Int32</span><span class="sxs-lookup"><span data-stu-id="207f1-119">Int32</span></span>|<span data-ttu-id="207f1-120">Количество устройств с Mac OS X.</span><span class="sxs-lookup"><span data-stu-id="207f1-120">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="207f1-121">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="207f1-121">windowsMobileCount</span></span>|<span data-ttu-id="207f1-122">Int32</span><span class="sxs-lookup"><span data-stu-id="207f1-122">Int32</span></span>|<span data-ttu-id="207f1-123">Количество мобильных устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="207f1-123">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="207f1-124">windowsCount</span><span class="sxs-lookup"><span data-stu-id="207f1-124">windowsCount</span></span>|<span data-ttu-id="207f1-125">Int32</span><span class="sxs-lookup"><span data-stu-id="207f1-125">Int32</span></span>|<span data-ttu-id="207f1-126">Количество устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="207f1-126">Number of Windows device count.</span></span>|
|<span data-ttu-id="207f1-127">unknownCount</span><span class="sxs-lookup"><span data-stu-id="207f1-127">unknownCount</span></span>|<span data-ttu-id="207f1-128">Int32</span><span class="sxs-lookup"><span data-stu-id="207f1-128">Int32</span></span>|<span data-ttu-id="207f1-129">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="207f1-129">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="207f1-130">Связи</span><span class="sxs-lookup"><span data-stu-id="207f1-130">Relationships</span></span>
<span data-ttu-id="207f1-131">Нет</span><span class="sxs-lookup"><span data-stu-id="207f1-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="207f1-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="207f1-132">JSON Representation</span></span>
<span data-ttu-id="207f1-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="207f1-133">Here is a JSON representation of the resource.</span></span>
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





