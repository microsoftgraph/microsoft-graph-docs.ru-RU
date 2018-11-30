---
title: Тип ресурса deviceOperatingSystemSummary
description: Общие сведения об операционной системе устройства.
ms.openlocfilehash: 13224e18f117f13a6f7c7090d1aa9cb2686350c4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082582"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="e2e3c-103">Тип ресурса deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="e2e3c-103">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="e2e3c-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e2e3c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e2e3c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2e3c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e2e3c-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e2e3c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e2e3c-107">Общие сведения об операционной системе устройства.</span><span class="sxs-lookup"><span data-stu-id="e2e3c-107">Device operating system summary.</span></span>
## <a name="properties"></a><span data-ttu-id="e2e3c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e2e3c-108">Properties</span></span>
|<span data-ttu-id="e2e3c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e2e3c-109">Property</span></span>|<span data-ttu-id="e2e3c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e2e3c-110">Type</span></span>|<span data-ttu-id="e2e3c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e2e3c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2e3c-112">androidCount</span><span class="sxs-lookup"><span data-stu-id="e2e3c-112">androidCount</span></span>|<span data-ttu-id="e2e3c-113">Int32</span><span class="sxs-lookup"><span data-stu-id="e2e3c-113">Int32</span></span>|<span data-ttu-id="e2e3c-114">Количество устройств с Android.</span><span class="sxs-lookup"><span data-stu-id="e2e3c-114">Number of android device count.</span></span>|
|<span data-ttu-id="e2e3c-115">iosCount</span><span class="sxs-lookup"><span data-stu-id="e2e3c-115">iosCount</span></span>|<span data-ttu-id="e2e3c-116">Int32</span><span class="sxs-lookup"><span data-stu-id="e2e3c-116">Int32</span></span>|<span data-ttu-id="e2e3c-117">Количество устройств с iOS.</span><span class="sxs-lookup"><span data-stu-id="e2e3c-117">Number of iOS device count.</span></span>|
|<span data-ttu-id="e2e3c-118">macOSCount</span><span class="sxs-lookup"><span data-stu-id="e2e3c-118">macOSCount</span></span>|<span data-ttu-id="e2e3c-119">Int32</span><span class="sxs-lookup"><span data-stu-id="e2e3c-119">Int32</span></span>|<span data-ttu-id="e2e3c-120">Количество устройств с Mac OS X.</span><span class="sxs-lookup"><span data-stu-id="e2e3c-120">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="e2e3c-121">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="e2e3c-121">windowsMobileCount</span></span>|<span data-ttu-id="e2e3c-122">Int32</span><span class="sxs-lookup"><span data-stu-id="e2e3c-122">Int32</span></span>|<span data-ttu-id="e2e3c-123">Количество мобильных устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="e2e3c-123">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="e2e3c-124">windowsCount</span><span class="sxs-lookup"><span data-stu-id="e2e3c-124">windowsCount</span></span>|<span data-ttu-id="e2e3c-125">Int32</span><span class="sxs-lookup"><span data-stu-id="e2e3c-125">Int32</span></span>|<span data-ttu-id="e2e3c-126">Количество устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="e2e3c-126">Number of Windows device count.</span></span>|
|<span data-ttu-id="e2e3c-127">unknownCount</span><span class="sxs-lookup"><span data-stu-id="e2e3c-127">unknownCount</span></span>|<span data-ttu-id="e2e3c-128">Int32</span><span class="sxs-lookup"><span data-stu-id="e2e3c-128">Int32</span></span>|<span data-ttu-id="e2e3c-129">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="e2e3c-129">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2e3c-130">Связи</span><span class="sxs-lookup"><span data-stu-id="e2e3c-130">Relationships</span></span>
<span data-ttu-id="e2e3c-131">Нет</span><span class="sxs-lookup"><span data-stu-id="e2e3c-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e2e3c-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e2e3c-132">JSON Representation</span></span>
<span data-ttu-id="e2e3c-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e2e3c-133">Here is a JSON representation of the resource.</span></span>
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





