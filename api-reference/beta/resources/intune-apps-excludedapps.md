---
title: Тип ресурса excludedApps
description: Содержит свойства для исключенных приложений Office 365.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1d3cd9a159597689a64070181640415a6ce2fc61
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395680"
---
# <a name="excludedapps-resource-type"></a><span data-ttu-id="81cf6-103">Тип ресурса excludedApps</span><span class="sxs-lookup"><span data-stu-id="81cf6-103">excludedApps resource type</span></span>

> <span data-ttu-id="81cf6-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="81cf6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="81cf6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81cf6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="81cf6-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="81cf6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81cf6-107">Содержит свойства для исключенных приложений Office 365.</span><span class="sxs-lookup"><span data-stu-id="81cf6-107">Contains properties for Excluded Office365 Apps.</span></span>

## <a name="properties"></a><span data-ttu-id="81cf6-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="81cf6-108">Properties</span></span>
|<span data-ttu-id="81cf6-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="81cf6-109">Property</span></span>|<span data-ttu-id="81cf6-110">Тип</span><span class="sxs-lookup"><span data-stu-id="81cf6-110">Type</span></span>|<span data-ttu-id="81cf6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="81cf6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81cf6-112">Access</span><span class="sxs-lookup"><span data-stu-id="81cf6-112">access</span></span>|<span data-ttu-id="81cf6-113">Логический</span><span class="sxs-lookup"><span data-stu-id="81cf6-113">Boolean</span></span>|<span data-ttu-id="81cf6-114">Значение для Если MS Office Access следует исключить или нет.</span><span class="sxs-lookup"><span data-stu-id="81cf6-114">The value for if MS Office Access should be excluded or not.</span></span>|
|<span data-ttu-id="81cf6-115">в приложении Excel</span><span class="sxs-lookup"><span data-stu-id="81cf6-115">excel</span></span>|<span data-ttu-id="81cf6-116">Логический</span><span class="sxs-lookup"><span data-stu-id="81cf6-116">Boolean</span></span>|<span data-ttu-id="81cf6-117">Значение для Если MS Office Excel следует исключить или нет.</span><span class="sxs-lookup"><span data-stu-id="81cf6-117">The value for if MS Office Excel should be excluded or not.</span></span>|
|<span data-ttu-id="81cf6-118">Groove</span><span class="sxs-lookup"><span data-stu-id="81cf6-118">groove</span></span>|<span data-ttu-id="81cf6-119">Логический</span><span class="sxs-lookup"><span data-stu-id="81cf6-119">Boolean</span></span>|<span data-ttu-id="81cf6-120">Значение для Если MS Office OneDrive для бизнеса - Groove следует исключить или нет.</span><span class="sxs-lookup"><span data-stu-id="81cf6-120">The value for if MS Office OneDrive for Business - Groove should be excluded or not.</span></span>|
|<span data-ttu-id="81cf6-121">infoPath</span><span class="sxs-lookup"><span data-stu-id="81cf6-121">infoPath</span></span>|<span data-ttu-id="81cf6-122">Логический</span><span class="sxs-lookup"><span data-stu-id="81cf6-122">Boolean</span></span>|<span data-ttu-id="81cf6-123">Значение для Если MS Office InfoPath следует исключить или нет.</span><span class="sxs-lookup"><span data-stu-id="81cf6-123">The value for if MS Office InfoPath should be excluded or not.</span></span>|
|<span data-ttu-id="81cf6-124">Lync</span><span class="sxs-lookup"><span data-stu-id="81cf6-124">lync</span></span>|<span data-ttu-id="81cf6-125">Логический</span><span class="sxs-lookup"><span data-stu-id="81cf6-125">Boolean</span></span>|<span data-ttu-id="81cf6-126">Значение для Если Скайп MS Office для бизнес - Lync следует исключить или нет.</span><span class="sxs-lookup"><span data-stu-id="81cf6-126">The value for if MS Office Skype for Business - Lync should be excluded or not.</span></span>|
|<span data-ttu-id="81cf6-127">oneDrive</span><span class="sxs-lookup"><span data-stu-id="81cf6-127">oneDrive</span></span>|<span data-ttu-id="81cf6-128">Логический</span><span class="sxs-lookup"><span data-stu-id="81cf6-128">Boolean</span></span>|<span data-ttu-id="81cf6-129">Значение для Если MS Office OneDrive следует исключить или нет.</span><span class="sxs-lookup"><span data-stu-id="81cf6-129">The value for if MS Office OneDrive should be excluded or not.</span></span>|
|<span data-ttu-id="81cf6-130">oneNote</span><span class="sxs-lookup"><span data-stu-id="81cf6-130">oneNote</span></span>|<span data-ttu-id="81cf6-131">Логический</span><span class="sxs-lookup"><span data-stu-id="81cf6-131">Boolean</span></span>|<span data-ttu-id="81cf6-132">Значение для Если MS Office OneNote следует исключить или нет.</span><span class="sxs-lookup"><span data-stu-id="81cf6-132">The value for if MS Office OneNote should be excluded or not.</span></span>|
|<span data-ttu-id="81cf6-133">Outlook</span><span class="sxs-lookup"><span data-stu-id="81cf6-133">outlook</span></span>|<span data-ttu-id="81cf6-134">Логический</span><span class="sxs-lookup"><span data-stu-id="81cf6-134">Boolean</span></span>|<span data-ttu-id="81cf6-135">Значение для Если MS Office Outlook следует исключить или нет.</span><span class="sxs-lookup"><span data-stu-id="81cf6-135">The value for if MS Office Outlook should be excluded or not.</span></span>|
|<span data-ttu-id="81cf6-136">powerPoint</span><span class="sxs-lookup"><span data-stu-id="81cf6-136">powerPoint</span></span>|<span data-ttu-id="81cf6-137">Логический</span><span class="sxs-lookup"><span data-stu-id="81cf6-137">Boolean</span></span>|<span data-ttu-id="81cf6-138">Значение для Если MS Office PowerPoint следует исключить или нет.</span><span class="sxs-lookup"><span data-stu-id="81cf6-138">The value for if MS Office PowerPoint should be excluded or not.</span></span>|
|<span data-ttu-id="81cf6-139">publisher</span><span class="sxs-lookup"><span data-stu-id="81cf6-139">publisher</span></span>|<span data-ttu-id="81cf6-140">Логический</span><span class="sxs-lookup"><span data-stu-id="81cf6-140">Boolean</span></span>|<span data-ttu-id="81cf6-141">Значение для Если MS Office Publisher следует исключить или нет.</span><span class="sxs-lookup"><span data-stu-id="81cf6-141">The value for if MS Office Publisher should be excluded or not.</span></span>|
|<span data-ttu-id="81cf6-142">sharePointDesigner</span><span class="sxs-lookup"><span data-stu-id="81cf6-142">sharePointDesigner</span></span>|<span data-ttu-id="81cf6-143">Логический</span><span class="sxs-lookup"><span data-stu-id="81cf6-143">Boolean</span></span>|<span data-ttu-id="81cf6-144">Значение для Если MS Office SharePointDesigner следует исключить или нет.</span><span class="sxs-lookup"><span data-stu-id="81cf6-144">The value for if MS Office SharePointDesigner should be excluded or not.</span></span>|
|<span data-ttu-id="81cf6-145">visio</span><span class="sxs-lookup"><span data-stu-id="81cf6-145">visio</span></span>|<span data-ttu-id="81cf6-146">Логический</span><span class="sxs-lookup"><span data-stu-id="81cf6-146">Boolean</span></span>|<span data-ttu-id="81cf6-147">Значение для Если MS Office Visio следует исключить или нет.</span><span class="sxs-lookup"><span data-stu-id="81cf6-147">The value for if MS Office Visio should be excluded or not.</span></span>|
|<span data-ttu-id="81cf6-148">Word</span><span class="sxs-lookup"><span data-stu-id="81cf6-148">word</span></span>|<span data-ttu-id="81cf6-149">Логический</span><span class="sxs-lookup"><span data-stu-id="81cf6-149">Boolean</span></span>|<span data-ttu-id="81cf6-150">Значение для Если MS Office Word следует исключить или нет.</span><span class="sxs-lookup"><span data-stu-id="81cf6-150">The value for if MS Office Word should be excluded or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="81cf6-151">Отношения</span><span class="sxs-lookup"><span data-stu-id="81cf6-151">Relationships</span></span>
<span data-ttu-id="81cf6-152">Нет</span><span class="sxs-lookup"><span data-stu-id="81cf6-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="81cf6-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="81cf6-153">JSON Representation</span></span>
<span data-ttu-id="81cf6-154">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="81cf6-154">Here is a JSON representation of the resource.</span></span>
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




