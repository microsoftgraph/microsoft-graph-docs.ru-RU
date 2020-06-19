---
title: Тип ресурса Excludedapps к объекту
description: Содержит свойства исключенных приложений Office365.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 92a86a9b875caf47d5c06145716642bb3d6a7e81
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44790903"
---
# <a name="excludedapps-resource-type"></a><span data-ttu-id="8717e-103">Тип ресурса Excludedapps к объекту</span><span class="sxs-lookup"><span data-stu-id="8717e-103">excludedApps resource type</span></span>

<span data-ttu-id="8717e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8717e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8717e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8717e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8717e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8717e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8717e-107">Содержит свойства исключенных приложений Office365.</span><span class="sxs-lookup"><span data-stu-id="8717e-107">Contains properties for Excluded Office365 Apps.</span></span>

## <a name="properties"></a><span data-ttu-id="8717e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="8717e-108">Properties</span></span>
|<span data-ttu-id="8717e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="8717e-109">Property</span></span>|<span data-ttu-id="8717e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="8717e-110">Type</span></span>|<span data-ttu-id="8717e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8717e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8717e-112">обращения</span><span class="sxs-lookup"><span data-stu-id="8717e-112">access</span></span>|<span data-ttu-id="8717e-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="8717e-113">Boolean</span></span>|<span data-ttu-id="8717e-114">Значение, если доступ к MS Office должен быть исключен или нет.</span><span class="sxs-lookup"><span data-stu-id="8717e-114">The value for if MS Office Access should be excluded or not.</span></span>|
|<span data-ttu-id="8717e-115">Bing</span><span class="sxs-lookup"><span data-stu-id="8717e-115">bing</span></span>|<span data-ttu-id="8717e-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="8717e-116">Boolean</span></span>|<span data-ttu-id="8717e-117">Значение, если Microsoft Search по умолчанию следует исключить.</span><span class="sxs-lookup"><span data-stu-id="8717e-117">The value for if Microsoft Search as default should be excluded or not.</span></span>|
|<span data-ttu-id="8717e-118">невозможно</span><span class="sxs-lookup"><span data-stu-id="8717e-118">excel</span></span>|<span data-ttu-id="8717e-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="8717e-119">Boolean</span></span>|<span data-ttu-id="8717e-120">Значение, заданное в поле IF MS Office Excel, не должно быть исключено.</span><span class="sxs-lookup"><span data-stu-id="8717e-120">The value for if MS Office Excel should be excluded or not.</span></span>|
|<span data-ttu-id="8717e-121">тень</span><span class="sxs-lookup"><span data-stu-id="8717e-121">groove</span></span>|<span data-ttu-id="8717e-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="8717e-122">Boolean</span></span>|<span data-ttu-id="8717e-123">Значение, которое должно быть исключено, если MS Office OneDrive для бизнеса — Groove.</span><span class="sxs-lookup"><span data-stu-id="8717e-123">The value for if MS Office OneDrive for Business - Groove should be excluded or not.</span></span>|
|<span data-ttu-id="8717e-124">infoPath</span><span class="sxs-lookup"><span data-stu-id="8717e-124">infoPath</span></span>|<span data-ttu-id="8717e-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="8717e-125">Boolean</span></span>|<span data-ttu-id="8717e-126">Значение, если MS Office InfoPath следует исключить.</span><span class="sxs-lookup"><span data-stu-id="8717e-126">The value for if MS Office InfoPath should be excluded or not.</span></span>|
|<span data-ttu-id="8717e-127">Lync</span><span class="sxs-lookup"><span data-stu-id="8717e-127">lync</span></span>|<span data-ttu-id="8717e-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="8717e-128">Boolean</span></span>|<span data-ttu-id="8717e-129">Значение, если MS Office Skype для бизнеса — не следует исключать.</span><span class="sxs-lookup"><span data-stu-id="8717e-129">The value for if MS Office Skype for Business - Lync should be excluded or not.</span></span>|
|<span data-ttu-id="8717e-130">oneDrive</span><span class="sxs-lookup"><span data-stu-id="8717e-130">oneDrive</span></span>|<span data-ttu-id="8717e-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="8717e-131">Boolean</span></span>|<span data-ttu-id="8717e-132">Значение, которое должно быть исключено, если MS Office OneDrive должен быть исключен.</span><span class="sxs-lookup"><span data-stu-id="8717e-132">The value for if MS Office OneDrive should be excluded or not.</span></span>|
|<span data-ttu-id="8717e-133">Microsoft</span><span class="sxs-lookup"><span data-stu-id="8717e-133">oneNote</span></span>|<span data-ttu-id="8717e-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="8717e-134">Boolean</span></span>|<span data-ttu-id="8717e-135">Значение, если MS Office OneNote должен быть исключен или нет.</span><span class="sxs-lookup"><span data-stu-id="8717e-135">The value for if MS Office OneNote should be excluded or not.</span></span>|
|<span data-ttu-id="8717e-136">outlook</span><span class="sxs-lookup"><span data-stu-id="8717e-136">outlook</span></span>|<span data-ttu-id="8717e-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="8717e-137">Boolean</span></span>|<span data-ttu-id="8717e-138">Значение, если MS Office Outlook следует исключить из проверки.</span><span class="sxs-lookup"><span data-stu-id="8717e-138">The value for if MS Office Outlook should be excluded or not.</span></span>|
|<span data-ttu-id="8717e-139">powerPoint</span><span class="sxs-lookup"><span data-stu-id="8717e-139">powerPoint</span></span>|<span data-ttu-id="8717e-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="8717e-140">Boolean</span></span>|<span data-ttu-id="8717e-141">Значение, если MS Office PowerPoint следует исключить из проверки.</span><span class="sxs-lookup"><span data-stu-id="8717e-141">The value for if MS Office PowerPoint should be excluded or not.</span></span>|
|<span data-ttu-id="8717e-142">publisher</span><span class="sxs-lookup"><span data-stu-id="8717e-142">publisher</span></span>|<span data-ttu-id="8717e-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="8717e-143">Boolean</span></span>|<span data-ttu-id="8717e-144">Значение, если MS Office Publisher должен быть исключен или нет.</span><span class="sxs-lookup"><span data-stu-id="8717e-144">The value for if MS Office Publisher should be excluded or not.</span></span>|
|<span data-ttu-id="8717e-145">шарепоинтдесигнер</span><span class="sxs-lookup"><span data-stu-id="8717e-145">sharePointDesigner</span></span>|<span data-ttu-id="8717e-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="8717e-146">Boolean</span></span>|<span data-ttu-id="8717e-147">Значение для параметра if MS Office Шарепоинтдесигнер должно быть исключено или нет.</span><span class="sxs-lookup"><span data-stu-id="8717e-147">The value for if MS Office SharePointDesigner should be excluded or not.</span></span>|
|<span data-ttu-id="8717e-148">Teams</span><span class="sxs-lookup"><span data-stu-id="8717e-148">teams</span></span>|<span data-ttu-id="8717e-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="8717e-149">Boolean</span></span>|<span data-ttu-id="8717e-150">Значение, которое должно быть исключено, если MS Office Teams должен быть исключен.</span><span class="sxs-lookup"><span data-stu-id="8717e-150">The value for if MS Office Teams should be excluded or not.</span></span>|
|<span data-ttu-id="8717e-151">Visio</span><span class="sxs-lookup"><span data-stu-id="8717e-151">visio</span></span>|<span data-ttu-id="8717e-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="8717e-152">Boolean</span></span>|<span data-ttu-id="8717e-153">Значение, заданное для if MS Office Visio, должно быть исключено.</span><span class="sxs-lookup"><span data-stu-id="8717e-153">The value for if MS Office Visio should be excluded or not.</span></span>|
|<span data-ttu-id="8717e-154">текстовых</span><span class="sxs-lookup"><span data-stu-id="8717e-154">word</span></span>|<span data-ttu-id="8717e-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="8717e-155">Boolean</span></span>|<span data-ttu-id="8717e-156">Значение, заданное для if MS Office Word, должно быть исключено.</span><span class="sxs-lookup"><span data-stu-id="8717e-156">The value for if MS Office Word should be excluded or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8717e-157">Связи</span><span class="sxs-lookup"><span data-stu-id="8717e-157">Relationships</span></span>
<span data-ttu-id="8717e-158">Нет</span><span class="sxs-lookup"><span data-stu-id="8717e-158">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8717e-159">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8717e-159">JSON Representation</span></span>
<span data-ttu-id="8717e-160">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8717e-160">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.excludedApps"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.excludedApps",
  "access": true,
  "bing": true,
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



