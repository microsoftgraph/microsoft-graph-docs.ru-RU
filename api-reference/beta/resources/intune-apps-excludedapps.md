---
title: Тип ресурса Excludedapps к объекту
description: Содержит свойства исключенных приложений Office365.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d566cd8ba088568e27c9a7e4878eda54cd7f1252
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36366093"
---
# <a name="excludedapps-resource-type"></a><span data-ttu-id="f34ba-103">Тип ресурса Excludedapps к объекту</span><span class="sxs-lookup"><span data-stu-id="f34ba-103">excludedApps resource type</span></span>

> <span data-ttu-id="f34ba-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f34ba-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f34ba-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f34ba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f34ba-106">Содержит свойства исключенных приложений Office365.</span><span class="sxs-lookup"><span data-stu-id="f34ba-106">Contains properties for Excluded Office365 Apps.</span></span>

## <a name="properties"></a><span data-ttu-id="f34ba-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f34ba-107">Properties</span></span>
|<span data-ttu-id="f34ba-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f34ba-108">Property</span></span>|<span data-ttu-id="f34ba-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f34ba-109">Type</span></span>|<span data-ttu-id="f34ba-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f34ba-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f34ba-111">обращения</span><span class="sxs-lookup"><span data-stu-id="f34ba-111">access</span></span>|<span data-ttu-id="f34ba-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="f34ba-112">Boolean</span></span>|<span data-ttu-id="f34ba-113">Значение, если доступ к MS Office должен быть исключен или нет.</span><span class="sxs-lookup"><span data-stu-id="f34ba-113">The value for if MS Office Access should be excluded or not.</span></span>|
|<span data-ttu-id="f34ba-114">невозможно</span><span class="sxs-lookup"><span data-stu-id="f34ba-114">excel</span></span>|<span data-ttu-id="f34ba-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="f34ba-115">Boolean</span></span>|<span data-ttu-id="f34ba-116">Значение, заданное в поле IF MS Office Excel, не должно быть исключено.</span><span class="sxs-lookup"><span data-stu-id="f34ba-116">The value for if MS Office Excel should be excluded or not.</span></span>|
|<span data-ttu-id="f34ba-117">тень</span><span class="sxs-lookup"><span data-stu-id="f34ba-117">groove</span></span>|<span data-ttu-id="f34ba-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="f34ba-118">Boolean</span></span>|<span data-ttu-id="f34ba-119">Значение, которое должно быть исключено, если MS Office OneDrive для бизнеса — Groove.</span><span class="sxs-lookup"><span data-stu-id="f34ba-119">The value for if MS Office OneDrive for Business - Groove should be excluded or not.</span></span>|
|<span data-ttu-id="f34ba-120">infoPath</span><span class="sxs-lookup"><span data-stu-id="f34ba-120">infoPath</span></span>|<span data-ttu-id="f34ba-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="f34ba-121">Boolean</span></span>|<span data-ttu-id="f34ba-122">Значение, если MS Office InfoPath следует исключить.</span><span class="sxs-lookup"><span data-stu-id="f34ba-122">The value for if MS Office InfoPath should be excluded or not.</span></span>|
|<span data-ttu-id="f34ba-123">Lync</span><span class="sxs-lookup"><span data-stu-id="f34ba-123">lync</span></span>|<span data-ttu-id="f34ba-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="f34ba-124">Boolean</span></span>|<span data-ttu-id="f34ba-125">Значение, если MS Office Skype для бизнеса — не следует исключать.</span><span class="sxs-lookup"><span data-stu-id="f34ba-125">The value for if MS Office Skype for Business - Lync should be excluded or not.</span></span>|
|<span data-ttu-id="f34ba-126">oneDrive</span><span class="sxs-lookup"><span data-stu-id="f34ba-126">oneDrive</span></span>|<span data-ttu-id="f34ba-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="f34ba-127">Boolean</span></span>|<span data-ttu-id="f34ba-128">Значение, которое должно быть исключено, если MS Office OneDrive должен быть исключен.</span><span class="sxs-lookup"><span data-stu-id="f34ba-128">The value for if MS Office OneDrive should be excluded or not.</span></span>|
|<span data-ttu-id="f34ba-129">Microsoft</span><span class="sxs-lookup"><span data-stu-id="f34ba-129">oneNote</span></span>|<span data-ttu-id="f34ba-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="f34ba-130">Boolean</span></span>|<span data-ttu-id="f34ba-131">Значение, если MS Office OneNote должен быть исключен или нет.</span><span class="sxs-lookup"><span data-stu-id="f34ba-131">The value for if MS Office OneNote should be excluded or not.</span></span>|
|<span data-ttu-id="f34ba-132">outlook</span><span class="sxs-lookup"><span data-stu-id="f34ba-132">outlook</span></span>|<span data-ttu-id="f34ba-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="f34ba-133">Boolean</span></span>|<span data-ttu-id="f34ba-134">Значение, если MS Office Outlook следует исключить из проверки.</span><span class="sxs-lookup"><span data-stu-id="f34ba-134">The value for if MS Office Outlook should be excluded or not.</span></span>|
|<span data-ttu-id="f34ba-135">powerPoint</span><span class="sxs-lookup"><span data-stu-id="f34ba-135">powerPoint</span></span>|<span data-ttu-id="f34ba-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="f34ba-136">Boolean</span></span>|<span data-ttu-id="f34ba-137">Значение, если MS Office PowerPoint следует исключить из проверки.</span><span class="sxs-lookup"><span data-stu-id="f34ba-137">The value for if MS Office PowerPoint should be excluded or not.</span></span>|
|<span data-ttu-id="f34ba-138">publisher</span><span class="sxs-lookup"><span data-stu-id="f34ba-138">publisher</span></span>|<span data-ttu-id="f34ba-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="f34ba-139">Boolean</span></span>|<span data-ttu-id="f34ba-140">Значение, если MS Office Publisher должен быть исключен или нет.</span><span class="sxs-lookup"><span data-stu-id="f34ba-140">The value for if MS Office Publisher should be excluded or not.</span></span>|
|<span data-ttu-id="f34ba-141">шарепоинтдесигнер</span><span class="sxs-lookup"><span data-stu-id="f34ba-141">sharePointDesigner</span></span>|<span data-ttu-id="f34ba-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="f34ba-142">Boolean</span></span>|<span data-ttu-id="f34ba-143">Значение для параметра if MS Office Шарепоинтдесигнер должно быть исключено или нет.</span><span class="sxs-lookup"><span data-stu-id="f34ba-143">The value for if MS Office SharePointDesigner should be excluded or not.</span></span>|
|<span data-ttu-id="f34ba-144">Teams</span><span class="sxs-lookup"><span data-stu-id="f34ba-144">teams</span></span>|<span data-ttu-id="f34ba-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="f34ba-145">Boolean</span></span>|<span data-ttu-id="f34ba-146">Значение, которое должно быть исключено, если MS Office Teams должен быть исключен.</span><span class="sxs-lookup"><span data-stu-id="f34ba-146">The value for if MS Office Teams should be excluded or not.</span></span>|
|<span data-ttu-id="f34ba-147">Visio</span><span class="sxs-lookup"><span data-stu-id="f34ba-147">visio</span></span>|<span data-ttu-id="f34ba-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="f34ba-148">Boolean</span></span>|<span data-ttu-id="f34ba-149">Значение, заданное для if MS Office Visio, должно быть исключено.</span><span class="sxs-lookup"><span data-stu-id="f34ba-149">The value for if MS Office Visio should be excluded or not.</span></span>|
|<span data-ttu-id="f34ba-150">текстовых</span><span class="sxs-lookup"><span data-stu-id="f34ba-150">word</span></span>|<span data-ttu-id="f34ba-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="f34ba-151">Boolean</span></span>|<span data-ttu-id="f34ba-152">Значение, заданное для if MS Office Word, должно быть исключено.</span><span class="sxs-lookup"><span data-stu-id="f34ba-152">The value for if MS Office Word should be excluded or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f34ba-153">Отношения</span><span class="sxs-lookup"><span data-stu-id="f34ba-153">Relationships</span></span>
<span data-ttu-id="f34ba-154">Нет</span><span class="sxs-lookup"><span data-stu-id="f34ba-154">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f34ba-155">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f34ba-155">JSON Representation</span></span>
<span data-ttu-id="f34ba-156">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f34ba-156">Here is a JSON representation of the resource.</span></span>
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



