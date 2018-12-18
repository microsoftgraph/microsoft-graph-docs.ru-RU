---
title: Тип ресурса excludedApps
description: Содержит свойства для исключенных приложений Office 365.
author: tfitzmac
ms.openlocfilehash: b8c9eff985783c953ff099dbf4d5ba00826652c4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344627"
---
# <a name="excludedapps-resource-type"></a><span data-ttu-id="c6687-103">Тип ресурса excludedApps</span><span class="sxs-lookup"><span data-stu-id="c6687-103">excludedApps resource type</span></span>

> <span data-ttu-id="c6687-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c6687-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c6687-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6687-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c6687-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c6687-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c6687-107">Содержит свойства для исключенных приложений Office 365.</span><span class="sxs-lookup"><span data-stu-id="c6687-107">Contains properties for Excluded Office365 Apps.</span></span>
## <a name="properties"></a><span data-ttu-id="c6687-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c6687-108">Properties</span></span>
|<span data-ttu-id="c6687-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c6687-109">Property</span></span>|<span data-ttu-id="c6687-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c6687-110">Type</span></span>|<span data-ttu-id="c6687-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c6687-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6687-112">Access</span><span class="sxs-lookup"><span data-stu-id="c6687-112">access</span></span>|<span data-ttu-id="c6687-113">Boolean.</span><span class="sxs-lookup"><span data-stu-id="c6687-113">Boolean</span></span>|<span data-ttu-id="c6687-114">Значение для Если MS Office Access следует исключить или нет.</span><span class="sxs-lookup"><span data-stu-id="c6687-114">The value for if MS Office Access should be excluded or not.</span></span>|
|<span data-ttu-id="c6687-115">в приложении Excel</span><span class="sxs-lookup"><span data-stu-id="c6687-115">excel</span></span>|<span data-ttu-id="c6687-116">Boolean.</span><span class="sxs-lookup"><span data-stu-id="c6687-116">Boolean</span></span>|<span data-ttu-id="c6687-117">Значение для Если MS Office Excel следует исключить или нет.</span><span class="sxs-lookup"><span data-stu-id="c6687-117">The value for if MS Office Excel should be excluded or not.</span></span>|
|<span data-ttu-id="c6687-118">Groove</span><span class="sxs-lookup"><span data-stu-id="c6687-118">groove</span></span>|<span data-ttu-id="c6687-119">Boolean.</span><span class="sxs-lookup"><span data-stu-id="c6687-119">Boolean</span></span>|<span data-ttu-id="c6687-120">Значение для Если MS Office OneDrive для бизнеса - Groove следует исключить или нет.</span><span class="sxs-lookup"><span data-stu-id="c6687-120">The value for if MS Office OneDrive for Business - Groove should be excluded or not.</span></span>|
|<span data-ttu-id="c6687-121">infoPath</span><span class="sxs-lookup"><span data-stu-id="c6687-121">infoPath</span></span>|<span data-ttu-id="c6687-122">Boolean.</span><span class="sxs-lookup"><span data-stu-id="c6687-122">Boolean</span></span>|<span data-ttu-id="c6687-123">Значение для Если MS Office InfoPath следует исключить или нет.</span><span class="sxs-lookup"><span data-stu-id="c6687-123">The value for if MS Office InfoPath should be excluded or not.</span></span>|
|<span data-ttu-id="c6687-124">Lync</span><span class="sxs-lookup"><span data-stu-id="c6687-124">lync</span></span>|<span data-ttu-id="c6687-125">Boolean.</span><span class="sxs-lookup"><span data-stu-id="c6687-125">Boolean</span></span>|<span data-ttu-id="c6687-126">Значение для Если Скайп MS Office для бизнес - Lync следует исключить или нет.</span><span class="sxs-lookup"><span data-stu-id="c6687-126">The value for if MS Office Skype for Business - Lync should be excluded or not.</span></span>|
|<span data-ttu-id="c6687-127">oneDrive</span><span class="sxs-lookup"><span data-stu-id="c6687-127">oneDrive</span></span>|<span data-ttu-id="c6687-128">Boolean.</span><span class="sxs-lookup"><span data-stu-id="c6687-128">Boolean</span></span>|<span data-ttu-id="c6687-129">Значение для Если MS Office OneDrive следует исключить или нет.</span><span class="sxs-lookup"><span data-stu-id="c6687-129">The value for if MS Office OneDrive should be excluded or not.</span></span>|
|<span data-ttu-id="c6687-130">oneNote</span><span class="sxs-lookup"><span data-stu-id="c6687-130">oneNote</span></span>|<span data-ttu-id="c6687-131">Boolean.</span><span class="sxs-lookup"><span data-stu-id="c6687-131">Boolean</span></span>|<span data-ttu-id="c6687-132">Значение для Если MS Office OneNote следует исключить или нет.</span><span class="sxs-lookup"><span data-stu-id="c6687-132">The value for if MS Office OneNote should be excluded or not.</span></span>|
|<span data-ttu-id="c6687-133">Outlook</span><span class="sxs-lookup"><span data-stu-id="c6687-133">outlook</span></span>|<span data-ttu-id="c6687-134">Boolean.</span><span class="sxs-lookup"><span data-stu-id="c6687-134">Boolean</span></span>|<span data-ttu-id="c6687-135">Значение для Если MS Office Outlook следует исключить или нет.</span><span class="sxs-lookup"><span data-stu-id="c6687-135">The value for if MS Office Outlook should be excluded or not.</span></span>|
|<span data-ttu-id="c6687-136">powerPoint</span><span class="sxs-lookup"><span data-stu-id="c6687-136">powerPoint</span></span>|<span data-ttu-id="c6687-137">Boolean.</span><span class="sxs-lookup"><span data-stu-id="c6687-137">Boolean</span></span>|<span data-ttu-id="c6687-138">Значение для Если MS Office PowerPoint следует исключить или нет.</span><span class="sxs-lookup"><span data-stu-id="c6687-138">The value for if MS Office PowerPoint should be excluded or not.</span></span>|
|<span data-ttu-id="c6687-139">publisher</span><span class="sxs-lookup"><span data-stu-id="c6687-139">publisher</span></span>|<span data-ttu-id="c6687-140">Boolean.</span><span class="sxs-lookup"><span data-stu-id="c6687-140">Boolean</span></span>|<span data-ttu-id="c6687-141">Значение для Если MS Office Publisher следует исключить или нет.</span><span class="sxs-lookup"><span data-stu-id="c6687-141">The value for if MS Office Publisher should be excluded or not.</span></span>|
|<span data-ttu-id="c6687-142">sharePointDesigner</span><span class="sxs-lookup"><span data-stu-id="c6687-142">sharePointDesigner</span></span>|<span data-ttu-id="c6687-143">Boolean.</span><span class="sxs-lookup"><span data-stu-id="c6687-143">Boolean</span></span>|<span data-ttu-id="c6687-144">Значение для Если MS Office SharePointDesigner следует исключить или нет.</span><span class="sxs-lookup"><span data-stu-id="c6687-144">The value for if MS Office SharePointDesigner should be excluded or not.</span></span>|
|<span data-ttu-id="c6687-145">visio</span><span class="sxs-lookup"><span data-stu-id="c6687-145">visio</span></span>|<span data-ttu-id="c6687-146">Boolean.</span><span class="sxs-lookup"><span data-stu-id="c6687-146">Boolean</span></span>|<span data-ttu-id="c6687-147">Значение для Если MS Office Visio следует исключить или нет.</span><span class="sxs-lookup"><span data-stu-id="c6687-147">The value for if MS Office Visio should be excluded or not.</span></span>|
|<span data-ttu-id="c6687-148">Word</span><span class="sxs-lookup"><span data-stu-id="c6687-148">word</span></span>|<span data-ttu-id="c6687-149">Boolean.</span><span class="sxs-lookup"><span data-stu-id="c6687-149">Boolean</span></span>|<span data-ttu-id="c6687-150">Значение для Если MS Office Word следует исключить или нет.</span><span class="sxs-lookup"><span data-stu-id="c6687-150">The value for if MS Office Word should be excluded or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c6687-151">Связи</span><span class="sxs-lookup"><span data-stu-id="c6687-151">Relationships</span></span>
<span data-ttu-id="c6687-152">Нет</span><span class="sxs-lookup"><span data-stu-id="c6687-152">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c6687-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c6687-153">JSON Representation</span></span>
<span data-ttu-id="c6687-154">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c6687-154">Here is a JSON representation of the resource.</span></span>
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





