---
title: Тип ресурса Excludedapps к объекту
description: Содержит свойства исключенных приложений Office365.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 24813edf732d73905a6b45b9e4fe584b6312a13c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42798142"
---
# <a name="excludedapps-resource-type"></a><span data-ttu-id="36d90-103">Тип ресурса Excludedapps к объекту</span><span class="sxs-lookup"><span data-stu-id="36d90-103">excludedApps resource type</span></span>

> <span data-ttu-id="36d90-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36d90-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="36d90-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="36d90-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36d90-106">Содержит свойства исключенных приложений Office365.</span><span class="sxs-lookup"><span data-stu-id="36d90-106">Contains properties for Excluded Office365 Apps.</span></span>

## <a name="properties"></a><span data-ttu-id="36d90-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="36d90-107">Properties</span></span>
|<span data-ttu-id="36d90-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="36d90-108">Property</span></span>|<span data-ttu-id="36d90-109">Тип</span><span class="sxs-lookup"><span data-stu-id="36d90-109">Type</span></span>|<span data-ttu-id="36d90-110">Описание</span><span class="sxs-lookup"><span data-stu-id="36d90-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36d90-111">обращения</span><span class="sxs-lookup"><span data-stu-id="36d90-111">access</span></span>|<span data-ttu-id="36d90-112">Логический</span><span class="sxs-lookup"><span data-stu-id="36d90-112">Boolean</span></span>|<span data-ttu-id="36d90-113">Значение, если доступ к MS Office должен быть исключен или нет.</span><span class="sxs-lookup"><span data-stu-id="36d90-113">The value for if MS Office Access should be excluded or not.</span></span>|
|<span data-ttu-id="36d90-114">невозможно</span><span class="sxs-lookup"><span data-stu-id="36d90-114">excel</span></span>|<span data-ttu-id="36d90-115">Логический</span><span class="sxs-lookup"><span data-stu-id="36d90-115">Boolean</span></span>|<span data-ttu-id="36d90-116">Значение, заданное в поле IF MS Office Excel, не должно быть исключено.</span><span class="sxs-lookup"><span data-stu-id="36d90-116">The value for if MS Office Excel should be excluded or not.</span></span>|
|<span data-ttu-id="36d90-117">тень</span><span class="sxs-lookup"><span data-stu-id="36d90-117">groove</span></span>|<span data-ttu-id="36d90-118">Логический</span><span class="sxs-lookup"><span data-stu-id="36d90-118">Boolean</span></span>|<span data-ttu-id="36d90-119">Значение, которое должно быть исключено, если MS Office OneDrive для бизнеса — Groove.</span><span class="sxs-lookup"><span data-stu-id="36d90-119">The value for if MS Office OneDrive for Business - Groove should be excluded or not.</span></span>|
|<span data-ttu-id="36d90-120">infoPath</span><span class="sxs-lookup"><span data-stu-id="36d90-120">infoPath</span></span>|<span data-ttu-id="36d90-121">Логический</span><span class="sxs-lookup"><span data-stu-id="36d90-121">Boolean</span></span>|<span data-ttu-id="36d90-122">Значение, если MS Office InfoPath следует исключить.</span><span class="sxs-lookup"><span data-stu-id="36d90-122">The value for if MS Office InfoPath should be excluded or not.</span></span>|
|<span data-ttu-id="36d90-123">Lync</span><span class="sxs-lookup"><span data-stu-id="36d90-123">lync</span></span>|<span data-ttu-id="36d90-124">Логический</span><span class="sxs-lookup"><span data-stu-id="36d90-124">Boolean</span></span>|<span data-ttu-id="36d90-125">Значение, если MS Office Skype для бизнеса — не следует исключать.</span><span class="sxs-lookup"><span data-stu-id="36d90-125">The value for if MS Office Skype for Business - Lync should be excluded or not.</span></span>|
|<span data-ttu-id="36d90-126">oneDrive</span><span class="sxs-lookup"><span data-stu-id="36d90-126">oneDrive</span></span>|<span data-ttu-id="36d90-127">Логический</span><span class="sxs-lookup"><span data-stu-id="36d90-127">Boolean</span></span>|<span data-ttu-id="36d90-128">Значение, которое должно быть исключено, если MS Office OneDrive должен быть исключен.</span><span class="sxs-lookup"><span data-stu-id="36d90-128">The value for if MS Office OneDrive should be excluded or not.</span></span>|
|<span data-ttu-id="36d90-129">Microsoft</span><span class="sxs-lookup"><span data-stu-id="36d90-129">oneNote</span></span>|<span data-ttu-id="36d90-130">Логический</span><span class="sxs-lookup"><span data-stu-id="36d90-130">Boolean</span></span>|<span data-ttu-id="36d90-131">Значение, если MS Office OneNote должен быть исключен или нет.</span><span class="sxs-lookup"><span data-stu-id="36d90-131">The value for if MS Office OneNote should be excluded or not.</span></span>|
|<span data-ttu-id="36d90-132">outlook</span><span class="sxs-lookup"><span data-stu-id="36d90-132">outlook</span></span>|<span data-ttu-id="36d90-133">Логический</span><span class="sxs-lookup"><span data-stu-id="36d90-133">Boolean</span></span>|<span data-ttu-id="36d90-134">Значение, если MS Office Outlook следует исключить из проверки.</span><span class="sxs-lookup"><span data-stu-id="36d90-134">The value for if MS Office Outlook should be excluded or not.</span></span>|
|<span data-ttu-id="36d90-135">powerPoint</span><span class="sxs-lookup"><span data-stu-id="36d90-135">powerPoint</span></span>|<span data-ttu-id="36d90-136">Логический</span><span class="sxs-lookup"><span data-stu-id="36d90-136">Boolean</span></span>|<span data-ttu-id="36d90-137">Значение, если MS Office PowerPoint следует исключить из проверки.</span><span class="sxs-lookup"><span data-stu-id="36d90-137">The value for if MS Office PowerPoint should be excluded or not.</span></span>|
|<span data-ttu-id="36d90-138">publisher</span><span class="sxs-lookup"><span data-stu-id="36d90-138">publisher</span></span>|<span data-ttu-id="36d90-139">Логический</span><span class="sxs-lookup"><span data-stu-id="36d90-139">Boolean</span></span>|<span data-ttu-id="36d90-140">Значение, если MS Office Publisher должен быть исключен или нет.</span><span class="sxs-lookup"><span data-stu-id="36d90-140">The value for if MS Office Publisher should be excluded or not.</span></span>|
|<span data-ttu-id="36d90-141">шарепоинтдесигнер</span><span class="sxs-lookup"><span data-stu-id="36d90-141">sharePointDesigner</span></span>|<span data-ttu-id="36d90-142">Логический</span><span class="sxs-lookup"><span data-stu-id="36d90-142">Boolean</span></span>|<span data-ttu-id="36d90-143">Значение для параметра if MS Office Шарепоинтдесигнер должно быть исключено или нет.</span><span class="sxs-lookup"><span data-stu-id="36d90-143">The value for if MS Office SharePointDesigner should be excluded or not.</span></span>|
|<span data-ttu-id="36d90-144">Teams</span><span class="sxs-lookup"><span data-stu-id="36d90-144">teams</span></span>|<span data-ttu-id="36d90-145">Логический</span><span class="sxs-lookup"><span data-stu-id="36d90-145">Boolean</span></span>|<span data-ttu-id="36d90-146">Значение, которое должно быть исключено, если MS Office Teams должен быть исключен.</span><span class="sxs-lookup"><span data-stu-id="36d90-146">The value for if MS Office Teams should be excluded or not.</span></span>|
|<span data-ttu-id="36d90-147">Visio</span><span class="sxs-lookup"><span data-stu-id="36d90-147">visio</span></span>|<span data-ttu-id="36d90-148">Логический</span><span class="sxs-lookup"><span data-stu-id="36d90-148">Boolean</span></span>|<span data-ttu-id="36d90-149">Значение, заданное для if MS Office Visio, должно быть исключено.</span><span class="sxs-lookup"><span data-stu-id="36d90-149">The value for if MS Office Visio should be excluded or not.</span></span>|
|<span data-ttu-id="36d90-150">текстовых</span><span class="sxs-lookup"><span data-stu-id="36d90-150">word</span></span>|<span data-ttu-id="36d90-151">Логический</span><span class="sxs-lookup"><span data-stu-id="36d90-151">Boolean</span></span>|<span data-ttu-id="36d90-152">Значение, заданное для if MS Office Word, должно быть исключено.</span><span class="sxs-lookup"><span data-stu-id="36d90-152">The value for if MS Office Word should be excluded or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="36d90-153">Связи</span><span class="sxs-lookup"><span data-stu-id="36d90-153">Relationships</span></span>
<span data-ttu-id="36d90-154">Нет</span><span class="sxs-lookup"><span data-stu-id="36d90-154">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="36d90-155">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="36d90-155">JSON Representation</span></span>
<span data-ttu-id="36d90-156">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="36d90-156">Here is a JSON representation of the resource.</span></span>
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
  "teams": true,
  "visio": true,
  "word": true
}
```



