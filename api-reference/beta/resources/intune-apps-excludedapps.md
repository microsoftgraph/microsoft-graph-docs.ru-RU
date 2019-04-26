---
title: Тип ресурса Excludedapps к объекту
description: Содержит свойства исключенных приложений Office365.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d90954bda8a5bd6c9bfdeb6af0d2946b48215d00
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553052"
---
# <a name="excludedapps-resource-type"></a><span data-ttu-id="f7271-103">Тип ресурса Excludedapps к объекту</span><span class="sxs-lookup"><span data-stu-id="f7271-103">excludedApps resource type</span></span>

> <span data-ttu-id="f7271-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7271-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f7271-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f7271-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7271-106">Содержит свойства исключенных приложений Office365.</span><span class="sxs-lookup"><span data-stu-id="f7271-106">Contains properties for Excluded Office365 Apps.</span></span>

## <a name="properties"></a><span data-ttu-id="f7271-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f7271-107">Properties</span></span>
|<span data-ttu-id="f7271-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f7271-108">Property</span></span>|<span data-ttu-id="f7271-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f7271-109">Type</span></span>|<span data-ttu-id="f7271-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f7271-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7271-111">обращения</span><span class="sxs-lookup"><span data-stu-id="f7271-111">access</span></span>|<span data-ttu-id="f7271-112">Логический</span><span class="sxs-lookup"><span data-stu-id="f7271-112">Boolean</span></span>|<span data-ttu-id="f7271-113">Значение, если доступ к MS Office должен быть исключен или нет.</span><span class="sxs-lookup"><span data-stu-id="f7271-113">The value for if MS Office Access should be excluded or not.</span></span>|
|<span data-ttu-id="f7271-114">невозможно</span><span class="sxs-lookup"><span data-stu-id="f7271-114">excel</span></span>|<span data-ttu-id="f7271-115">Логический</span><span class="sxs-lookup"><span data-stu-id="f7271-115">Boolean</span></span>|<span data-ttu-id="f7271-116">Значение, заДанное в поле IF MS Office Excel, не должно быть исключено.</span><span class="sxs-lookup"><span data-stu-id="f7271-116">The value for if MS Office Excel should be excluded or not.</span></span>|
|<span data-ttu-id="f7271-117">тень</span><span class="sxs-lookup"><span data-stu-id="f7271-117">groove</span></span>|<span data-ttu-id="f7271-118">Логический</span><span class="sxs-lookup"><span data-stu-id="f7271-118">Boolean</span></span>|<span data-ttu-id="f7271-119">Значение, которое должно быть исключено, если MS Office OneDrive для бизнеса — Groove.</span><span class="sxs-lookup"><span data-stu-id="f7271-119">The value for if MS Office OneDrive for Business - Groove should be excluded or not.</span></span>|
|<span data-ttu-id="f7271-120">infoPath</span><span class="sxs-lookup"><span data-stu-id="f7271-120">infoPath</span></span>|<span data-ttu-id="f7271-121">Логический</span><span class="sxs-lookup"><span data-stu-id="f7271-121">Boolean</span></span>|<span data-ttu-id="f7271-122">Значение, если MS Office InfoPath следует исключить.</span><span class="sxs-lookup"><span data-stu-id="f7271-122">The value for if MS Office InfoPath should be excluded or not.</span></span>|
|<span data-ttu-id="f7271-123">Lync</span><span class="sxs-lookup"><span data-stu-id="f7271-123">lync</span></span>|<span data-ttu-id="f7271-124">Логический</span><span class="sxs-lookup"><span data-stu-id="f7271-124">Boolean</span></span>|<span data-ttu-id="f7271-125">Значение, если MS Office Skype для бизнеса — не следует исключать.</span><span class="sxs-lookup"><span data-stu-id="f7271-125">The value for if MS Office Skype for Business - Lync should be excluded or not.</span></span>|
|<span data-ttu-id="f7271-126">oneDrive</span><span class="sxs-lookup"><span data-stu-id="f7271-126">oneDrive</span></span>|<span data-ttu-id="f7271-127">Логический</span><span class="sxs-lookup"><span data-stu-id="f7271-127">Boolean</span></span>|<span data-ttu-id="f7271-128">Значение, которое должно быть исключено, если MS Office OneDrive должен быть исключен.</span><span class="sxs-lookup"><span data-stu-id="f7271-128">The value for if MS Office OneDrive should be excluded or not.</span></span>|
|<span data-ttu-id="f7271-129">Microsoft</span><span class="sxs-lookup"><span data-stu-id="f7271-129">oneNote</span></span>|<span data-ttu-id="f7271-130">Логический</span><span class="sxs-lookup"><span data-stu-id="f7271-130">Boolean</span></span>|<span data-ttu-id="f7271-131">Значение, если MS Office OneNote должен быть исключен или нет.</span><span class="sxs-lookup"><span data-stu-id="f7271-131">The value for if MS Office OneNote should be excluded or not.</span></span>|
|<span data-ttu-id="f7271-132">outlook</span><span class="sxs-lookup"><span data-stu-id="f7271-132">outlook</span></span>|<span data-ttu-id="f7271-133">Логический</span><span class="sxs-lookup"><span data-stu-id="f7271-133">Boolean</span></span>|<span data-ttu-id="f7271-134">Значение, если MS Office Outlook следует исключить из проверки.</span><span class="sxs-lookup"><span data-stu-id="f7271-134">The value for if MS Office Outlook should be excluded or not.</span></span>|
|<span data-ttu-id="f7271-135">powerPoint</span><span class="sxs-lookup"><span data-stu-id="f7271-135">powerPoint</span></span>|<span data-ttu-id="f7271-136">Логический</span><span class="sxs-lookup"><span data-stu-id="f7271-136">Boolean</span></span>|<span data-ttu-id="f7271-137">Значение, если MS Office PowerPoint следует исключить из проверки.</span><span class="sxs-lookup"><span data-stu-id="f7271-137">The value for if MS Office PowerPoint should be excluded or not.</span></span>|
|<span data-ttu-id="f7271-138">publisher</span><span class="sxs-lookup"><span data-stu-id="f7271-138">publisher</span></span>|<span data-ttu-id="f7271-139">Логический</span><span class="sxs-lookup"><span data-stu-id="f7271-139">Boolean</span></span>|<span data-ttu-id="f7271-140">Значение, если MS Office Publisher должен быть исключен или нет.</span><span class="sxs-lookup"><span data-stu-id="f7271-140">The value for if MS Office Publisher should be excluded or not.</span></span>|
|<span data-ttu-id="f7271-141">Шарепоинтдесигнер</span><span class="sxs-lookup"><span data-stu-id="f7271-141">sharePointDesigner</span></span>|<span data-ttu-id="f7271-142">Логический</span><span class="sxs-lookup"><span data-stu-id="f7271-142">Boolean</span></span>|<span data-ttu-id="f7271-143">Значение для параметра if MS Office Шарепоинтдесигнер должно быть исключено или нет.</span><span class="sxs-lookup"><span data-stu-id="f7271-143">The value for if MS Office SharePointDesigner should be excluded or not.</span></span>|
|<span data-ttu-id="f7271-144">Teams</span><span class="sxs-lookup"><span data-stu-id="f7271-144">teams</span></span>|<span data-ttu-id="f7271-145">Логический</span><span class="sxs-lookup"><span data-stu-id="f7271-145">Boolean</span></span>|<span data-ttu-id="f7271-146">Значение, которое должно быть исключено, если MS Office Teams должен быть исключен.</span><span class="sxs-lookup"><span data-stu-id="f7271-146">The value for if MS Office Teams should be excluded or not.</span></span>|
|<span data-ttu-id="f7271-147">Visio</span><span class="sxs-lookup"><span data-stu-id="f7271-147">visio</span></span>|<span data-ttu-id="f7271-148">Логический</span><span class="sxs-lookup"><span data-stu-id="f7271-148">Boolean</span></span>|<span data-ttu-id="f7271-149">Значение, заДанное для if MS Office Visio, должно быть исключено.</span><span class="sxs-lookup"><span data-stu-id="f7271-149">The value for if MS Office Visio should be excluded or not.</span></span>|
|<span data-ttu-id="f7271-150">текстовых</span><span class="sxs-lookup"><span data-stu-id="f7271-150">word</span></span>|<span data-ttu-id="f7271-151">Логический</span><span class="sxs-lookup"><span data-stu-id="f7271-151">Boolean</span></span>|<span data-ttu-id="f7271-152">Значение, заДанное для if MS Office Word, должно быть исключено.</span><span class="sxs-lookup"><span data-stu-id="f7271-152">The value for if MS Office Word should be excluded or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f7271-153">Отношения</span><span class="sxs-lookup"><span data-stu-id="f7271-153">Relationships</span></span>
<span data-ttu-id="f7271-154">Нет</span><span class="sxs-lookup"><span data-stu-id="f7271-154">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f7271-155">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f7271-155">JSON Representation</span></span>
<span data-ttu-id="f7271-156">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f7271-156">Here is a JSON representation of the resource.</span></span>
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





