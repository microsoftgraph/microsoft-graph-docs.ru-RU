---
title: Тип ресурса excludedApps
description: Содержит свойства для исключенных приложений Office 365.
ms.openlocfilehash: 05c1ed7f4789e1a27ddacf92dbd773b2f5a21847
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077234"
---
# <a name="excludedapps-resource-type"></a><span data-ttu-id="54d49-103">Тип ресурса excludedApps</span><span class="sxs-lookup"><span data-stu-id="54d49-103">excludedApps resource type</span></span>

> <span data-ttu-id="54d49-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="54d49-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="54d49-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54d49-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="54d49-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="54d49-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="54d49-107">Содержит свойства для исключенных приложений Office 365.</span><span class="sxs-lookup"><span data-stu-id="54d49-107">Contains properties for Excluded Office365 Apps.</span></span>
## <a name="properties"></a><span data-ttu-id="54d49-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="54d49-108">Properties</span></span>
|<span data-ttu-id="54d49-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="54d49-109">Property</span></span>|<span data-ttu-id="54d49-110">Тип</span><span class="sxs-lookup"><span data-stu-id="54d49-110">Type</span></span>|<span data-ttu-id="54d49-111">Description</span><span class="sxs-lookup"><span data-stu-id="54d49-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54d49-112">Access</span><span class="sxs-lookup"><span data-stu-id="54d49-112">access</span></span>|<span data-ttu-id="54d49-113">Логический</span><span class="sxs-lookup"><span data-stu-id="54d49-113">Boolean</span></span>|<span data-ttu-id="54d49-114">Значение для Если MS Office Access следует исключить или нет.</span><span class="sxs-lookup"><span data-stu-id="54d49-114">The value for if MS Office Access should be excluded or not.</span></span>|
|<span data-ttu-id="54d49-115">в приложении Excel</span><span class="sxs-lookup"><span data-stu-id="54d49-115">excel</span></span>|<span data-ttu-id="54d49-116">Логический</span><span class="sxs-lookup"><span data-stu-id="54d49-116">Boolean</span></span>|<span data-ttu-id="54d49-117">Значение для Если MS Office Excel следует исключить или нет.</span><span class="sxs-lookup"><span data-stu-id="54d49-117">The value for if MS Office Excel should be excluded or not.</span></span>|
|<span data-ttu-id="54d49-118">Groove</span><span class="sxs-lookup"><span data-stu-id="54d49-118">groove</span></span>|<span data-ttu-id="54d49-119">Логический</span><span class="sxs-lookup"><span data-stu-id="54d49-119">Boolean</span></span>|<span data-ttu-id="54d49-120">Значение для Если MS Office OneDrive для бизнеса - Groove следует исключить или нет.</span><span class="sxs-lookup"><span data-stu-id="54d49-120">The value for if MS Office OneDrive for Business - Groove should be excluded or not.</span></span>|
|<span data-ttu-id="54d49-121">infoPath</span><span class="sxs-lookup"><span data-stu-id="54d49-121">infoPath</span></span>|<span data-ttu-id="54d49-122">Логический</span><span class="sxs-lookup"><span data-stu-id="54d49-122">Boolean</span></span>|<span data-ttu-id="54d49-123">Значение для Если MS Office InfoPath следует исключить или нет.</span><span class="sxs-lookup"><span data-stu-id="54d49-123">The value for if MS Office InfoPath should be excluded or not.</span></span>|
|<span data-ttu-id="54d49-124">Lync</span><span class="sxs-lookup"><span data-stu-id="54d49-124">lync</span></span>|<span data-ttu-id="54d49-125">Логический</span><span class="sxs-lookup"><span data-stu-id="54d49-125">Boolean</span></span>|<span data-ttu-id="54d49-126">Значение для Если Скайп MS Office для бизнес - Lync следует исключить или нет.</span><span class="sxs-lookup"><span data-stu-id="54d49-126">The value for if MS Office Skype for Business - Lync should be excluded or not.</span></span>|
|<span data-ttu-id="54d49-127">oneDrive</span><span class="sxs-lookup"><span data-stu-id="54d49-127">oneDrive</span></span>|<span data-ttu-id="54d49-128">Логический</span><span class="sxs-lookup"><span data-stu-id="54d49-128">Boolean</span></span>|<span data-ttu-id="54d49-129">Значение для Если MS Office OneDrive следует исключить или нет.</span><span class="sxs-lookup"><span data-stu-id="54d49-129">The value for if MS Office OneDrive should be excluded or not.</span></span>|
|<span data-ttu-id="54d49-130">oneNote</span><span class="sxs-lookup"><span data-stu-id="54d49-130">oneNote</span></span>|<span data-ttu-id="54d49-131">Логический</span><span class="sxs-lookup"><span data-stu-id="54d49-131">Boolean</span></span>|<span data-ttu-id="54d49-132">Значение для Если MS Office OneNote следует исключить или нет.</span><span class="sxs-lookup"><span data-stu-id="54d49-132">The value for if MS Office OneNote should be excluded or not.</span></span>|
|<span data-ttu-id="54d49-133">Outlook</span><span class="sxs-lookup"><span data-stu-id="54d49-133">outlook</span></span>|<span data-ttu-id="54d49-134">Логический</span><span class="sxs-lookup"><span data-stu-id="54d49-134">Boolean</span></span>|<span data-ttu-id="54d49-135">Значение для Если MS Office Outlook следует исключить или нет.</span><span class="sxs-lookup"><span data-stu-id="54d49-135">The value for if MS Office Outlook should be excluded or not.</span></span>|
|<span data-ttu-id="54d49-136">powerPoint</span><span class="sxs-lookup"><span data-stu-id="54d49-136">powerPoint</span></span>|<span data-ttu-id="54d49-137">Логический</span><span class="sxs-lookup"><span data-stu-id="54d49-137">Boolean</span></span>|<span data-ttu-id="54d49-138">Значение для Если MS Office PowerPoint следует исключить или нет.</span><span class="sxs-lookup"><span data-stu-id="54d49-138">The value for if MS Office PowerPoint should be excluded or not.</span></span>|
|<span data-ttu-id="54d49-139">publisher</span><span class="sxs-lookup"><span data-stu-id="54d49-139">publisher</span></span>|<span data-ttu-id="54d49-140">Логический</span><span class="sxs-lookup"><span data-stu-id="54d49-140">Boolean</span></span>|<span data-ttu-id="54d49-141">Значение для Если MS Office Publisher следует исключить или нет.</span><span class="sxs-lookup"><span data-stu-id="54d49-141">The value for if MS Office Publisher should be excluded or not.</span></span>|
|<span data-ttu-id="54d49-142">sharePointDesigner</span><span class="sxs-lookup"><span data-stu-id="54d49-142">sharePointDesigner</span></span>|<span data-ttu-id="54d49-143">Логический</span><span class="sxs-lookup"><span data-stu-id="54d49-143">Boolean</span></span>|<span data-ttu-id="54d49-144">Значение для Если MS Office SharePointDesigner следует исключить или нет.</span><span class="sxs-lookup"><span data-stu-id="54d49-144">The value for if MS Office SharePointDesigner should be excluded or not.</span></span>|
|<span data-ttu-id="54d49-145">visio</span><span class="sxs-lookup"><span data-stu-id="54d49-145">visio</span></span>|<span data-ttu-id="54d49-146">Логический</span><span class="sxs-lookup"><span data-stu-id="54d49-146">Boolean</span></span>|<span data-ttu-id="54d49-147">Значение для Если MS Office Visio следует исключить или нет.</span><span class="sxs-lookup"><span data-stu-id="54d49-147">The value for if MS Office Visio should be excluded or not.</span></span>|
|<span data-ttu-id="54d49-148">Word</span><span class="sxs-lookup"><span data-stu-id="54d49-148">word</span></span>|<span data-ttu-id="54d49-149">Логический</span><span class="sxs-lookup"><span data-stu-id="54d49-149">Boolean</span></span>|<span data-ttu-id="54d49-150">Значение для Если MS Office Word следует исключить или нет.</span><span class="sxs-lookup"><span data-stu-id="54d49-150">The value for if MS Office Word should be excluded or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="54d49-151">Связи</span><span class="sxs-lookup"><span data-stu-id="54d49-151">Relationships</span></span>
<span data-ttu-id="54d49-152">Нет</span><span class="sxs-lookup"><span data-stu-id="54d49-152">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="54d49-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="54d49-153">JSON Representation</span></span>
<span data-ttu-id="54d49-154">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="54d49-154">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.excludedApps"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.excludedApps",
  "access": true,
  "excel": true,
  "groove": true,
  "infoPath": true,
  "lync": true,
  "oneDrive": true,
  "oneNote": true,
  "outlook": true,
  "powerPoint": true,
  "publisher": true,
  "sharePointDesigner": true,
  "visio": true,
  "word": true
}
```





