---
title: Тип ресурса Excludedapps к объекту
description: Содержит свойства исключенных приложений Office365.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4f4a481d52b06c59d9d79df439b41152600af989
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49274287"
---
# <a name="excludedapps-resource-type"></a><span data-ttu-id="11b08-103">Тип ресурса Excludedapps к объекту</span><span class="sxs-lookup"><span data-stu-id="11b08-103">excludedApps resource type</span></span>

<span data-ttu-id="11b08-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11b08-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="11b08-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11b08-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="11b08-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="11b08-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11b08-107">Содержит свойства исключенных приложений Office365.</span><span class="sxs-lookup"><span data-stu-id="11b08-107">Contains properties for Excluded Office365 Apps.</span></span>

## <a name="properties"></a><span data-ttu-id="11b08-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="11b08-108">Properties</span></span>
|<span data-ttu-id="11b08-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="11b08-109">Property</span></span>|<span data-ttu-id="11b08-110">Тип</span><span class="sxs-lookup"><span data-stu-id="11b08-110">Type</span></span>|<span data-ttu-id="11b08-111">Описание</span><span class="sxs-lookup"><span data-stu-id="11b08-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11b08-112">обращения</span><span class="sxs-lookup"><span data-stu-id="11b08-112">access</span></span>|<span data-ttu-id="11b08-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="11b08-113">Boolean</span></span>|<span data-ttu-id="11b08-114">Значение, если доступ к MS Office должен быть исключен или нет.</span><span class="sxs-lookup"><span data-stu-id="11b08-114">The value for if MS Office Access should be excluded or not.</span></span>|
|<span data-ttu-id="11b08-115">Bing</span><span class="sxs-lookup"><span data-stu-id="11b08-115">bing</span></span>|<span data-ttu-id="11b08-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="11b08-116">Boolean</span></span>|<span data-ttu-id="11b08-117">Значение, если Microsoft Search по умолчанию следует исключить.</span><span class="sxs-lookup"><span data-stu-id="11b08-117">The value for if Microsoft Search as default should be excluded or not.</span></span>|
|<span data-ttu-id="11b08-118">невозможно</span><span class="sxs-lookup"><span data-stu-id="11b08-118">excel</span></span>|<span data-ttu-id="11b08-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="11b08-119">Boolean</span></span>|<span data-ttu-id="11b08-120">Значение, заданное в поле IF MS Office Excel, не должно быть исключено.</span><span class="sxs-lookup"><span data-stu-id="11b08-120">The value for if MS Office Excel should be excluded or not.</span></span>|
|<span data-ttu-id="11b08-121">тень</span><span class="sxs-lookup"><span data-stu-id="11b08-121">groove</span></span>|<span data-ttu-id="11b08-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="11b08-122">Boolean</span></span>|<span data-ttu-id="11b08-123">Значение, которое должно быть исключено, если MS Office OneDrive для бизнеса — Groove.</span><span class="sxs-lookup"><span data-stu-id="11b08-123">The value for if MS Office OneDrive for Business - Groove should be excluded or not.</span></span>|
|<span data-ttu-id="11b08-124">infoPath</span><span class="sxs-lookup"><span data-stu-id="11b08-124">infoPath</span></span>|<span data-ttu-id="11b08-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="11b08-125">Boolean</span></span>|<span data-ttu-id="11b08-126">Значение, если MS Office InfoPath следует исключить.</span><span class="sxs-lookup"><span data-stu-id="11b08-126">The value for if MS Office InfoPath should be excluded or not.</span></span>|
|<span data-ttu-id="11b08-127">Lync</span><span class="sxs-lookup"><span data-stu-id="11b08-127">lync</span></span>|<span data-ttu-id="11b08-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="11b08-128">Boolean</span></span>|<span data-ttu-id="11b08-129">Значение, если MS Office Skype для бизнеса — не следует исключать.</span><span class="sxs-lookup"><span data-stu-id="11b08-129">The value for if MS Office Skype for Business - Lync should be excluded or not.</span></span>|
|<span data-ttu-id="11b08-130">oneDrive</span><span class="sxs-lookup"><span data-stu-id="11b08-130">oneDrive</span></span>|<span data-ttu-id="11b08-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="11b08-131">Boolean</span></span>|<span data-ttu-id="11b08-132">Значение, которое должно быть исключено, если MS Office OneDrive должен быть исключен.</span><span class="sxs-lookup"><span data-stu-id="11b08-132">The value for if MS Office OneDrive should be excluded or not.</span></span>|
|<span data-ttu-id="11b08-133">Microsoft</span><span class="sxs-lookup"><span data-stu-id="11b08-133">oneNote</span></span>|<span data-ttu-id="11b08-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="11b08-134">Boolean</span></span>|<span data-ttu-id="11b08-135">Значение, если MS Office OneNote должен быть исключен или нет.</span><span class="sxs-lookup"><span data-stu-id="11b08-135">The value for if MS Office OneNote should be excluded or not.</span></span>|
|<span data-ttu-id="11b08-136">outlook</span><span class="sxs-lookup"><span data-stu-id="11b08-136">outlook</span></span>|<span data-ttu-id="11b08-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="11b08-137">Boolean</span></span>|<span data-ttu-id="11b08-138">Значение, если MS Office Outlook следует исключить из проверки.</span><span class="sxs-lookup"><span data-stu-id="11b08-138">The value for if MS Office Outlook should be excluded or not.</span></span>|
|<span data-ttu-id="11b08-139">powerPoint</span><span class="sxs-lookup"><span data-stu-id="11b08-139">powerPoint</span></span>|<span data-ttu-id="11b08-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="11b08-140">Boolean</span></span>|<span data-ttu-id="11b08-141">Значение, если MS Office PowerPoint следует исключить из проверки.</span><span class="sxs-lookup"><span data-stu-id="11b08-141">The value for if MS Office PowerPoint should be excluded or not.</span></span>|
|<span data-ttu-id="11b08-142">publisher</span><span class="sxs-lookup"><span data-stu-id="11b08-142">publisher</span></span>|<span data-ttu-id="11b08-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="11b08-143">Boolean</span></span>|<span data-ttu-id="11b08-144">Значение, если MS Office Publisher должен быть исключен или нет.</span><span class="sxs-lookup"><span data-stu-id="11b08-144">The value for if MS Office Publisher should be excluded or not.</span></span>|
|<span data-ttu-id="11b08-145">шарепоинтдесигнер</span><span class="sxs-lookup"><span data-stu-id="11b08-145">sharePointDesigner</span></span>|<span data-ttu-id="11b08-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="11b08-146">Boolean</span></span>|<span data-ttu-id="11b08-147">Значение для параметра if MS Office Шарепоинтдесигнер должно быть исключено или нет.</span><span class="sxs-lookup"><span data-stu-id="11b08-147">The value for if MS Office SharePointDesigner should be excluded or not.</span></span>|
|<span data-ttu-id="11b08-148">Teams</span><span class="sxs-lookup"><span data-stu-id="11b08-148">teams</span></span>|<span data-ttu-id="11b08-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="11b08-149">Boolean</span></span>|<span data-ttu-id="11b08-150">Значение, которое должно быть исключено, если MS Office Teams должен быть исключен.</span><span class="sxs-lookup"><span data-stu-id="11b08-150">The value for if MS Office Teams should be excluded or not.</span></span>|
|<span data-ttu-id="11b08-151">Visio</span><span class="sxs-lookup"><span data-stu-id="11b08-151">visio</span></span>|<span data-ttu-id="11b08-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="11b08-152">Boolean</span></span>|<span data-ttu-id="11b08-153">Значение, заданное для if MS Office Visio, должно быть исключено.</span><span class="sxs-lookup"><span data-stu-id="11b08-153">The value for if MS Office Visio should be excluded or not.</span></span>|
|<span data-ttu-id="11b08-154">текстовых</span><span class="sxs-lookup"><span data-stu-id="11b08-154">word</span></span>|<span data-ttu-id="11b08-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="11b08-155">Boolean</span></span>|<span data-ttu-id="11b08-156">Значение, заданное для if MS Office Word, должно быть исключено.</span><span class="sxs-lookup"><span data-stu-id="11b08-156">The value for if MS Office Word should be excluded or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="11b08-157">Связи</span><span class="sxs-lookup"><span data-stu-id="11b08-157">Relationships</span></span>
<span data-ttu-id="11b08-158">Нет</span><span class="sxs-lookup"><span data-stu-id="11b08-158">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="11b08-159">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="11b08-159">JSON Representation</span></span>
<span data-ttu-id="11b08-160">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="11b08-160">Here is a JSON representation of the resource.</span></span>
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




