---
title: Тип ресурса Excludedapps к объекту
description: Содержит свойства исключенных приложений Office365.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 47954bb18ad7ac1ec517038f9861818418e6aabd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42493799"
---
# <a name="excludedapps-resource-type"></a><span data-ttu-id="9fd84-103">Тип ресурса Excludedapps к объекту</span><span class="sxs-lookup"><span data-stu-id="9fd84-103">excludedApps resource type</span></span>

<span data-ttu-id="9fd84-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9fd84-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9fd84-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9fd84-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9fd84-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9fd84-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9fd84-107">Содержит свойства исключенных приложений Office365.</span><span class="sxs-lookup"><span data-stu-id="9fd84-107">Contains properties for Excluded Office365 Apps.</span></span>

## <a name="properties"></a><span data-ttu-id="9fd84-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="9fd84-108">Properties</span></span>
|<span data-ttu-id="9fd84-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="9fd84-109">Property</span></span>|<span data-ttu-id="9fd84-110">Тип</span><span class="sxs-lookup"><span data-stu-id="9fd84-110">Type</span></span>|<span data-ttu-id="9fd84-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9fd84-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fd84-112">обращения</span><span class="sxs-lookup"><span data-stu-id="9fd84-112">access</span></span>|<span data-ttu-id="9fd84-113">Логический</span><span class="sxs-lookup"><span data-stu-id="9fd84-113">Boolean</span></span>|<span data-ttu-id="9fd84-114">Значение, если доступ к MS Office должен быть исключен или нет.</span><span class="sxs-lookup"><span data-stu-id="9fd84-114">The value for if MS Office Access should be excluded or not.</span></span>|
|<span data-ttu-id="9fd84-115">невозможно</span><span class="sxs-lookup"><span data-stu-id="9fd84-115">excel</span></span>|<span data-ttu-id="9fd84-116">Логический</span><span class="sxs-lookup"><span data-stu-id="9fd84-116">Boolean</span></span>|<span data-ttu-id="9fd84-117">Значение, заданное в поле IF MS Office Excel, не должно быть исключено.</span><span class="sxs-lookup"><span data-stu-id="9fd84-117">The value for if MS Office Excel should be excluded or not.</span></span>|
|<span data-ttu-id="9fd84-118">тень</span><span class="sxs-lookup"><span data-stu-id="9fd84-118">groove</span></span>|<span data-ttu-id="9fd84-119">Логический</span><span class="sxs-lookup"><span data-stu-id="9fd84-119">Boolean</span></span>|<span data-ttu-id="9fd84-120">Значение, которое должно быть исключено, если MS Office OneDrive для бизнеса — Groove.</span><span class="sxs-lookup"><span data-stu-id="9fd84-120">The value for if MS Office OneDrive for Business - Groove should be excluded or not.</span></span>|
|<span data-ttu-id="9fd84-121">infoPath</span><span class="sxs-lookup"><span data-stu-id="9fd84-121">infoPath</span></span>|<span data-ttu-id="9fd84-122">Логический</span><span class="sxs-lookup"><span data-stu-id="9fd84-122">Boolean</span></span>|<span data-ttu-id="9fd84-123">Значение, если MS Office InfoPath следует исключить.</span><span class="sxs-lookup"><span data-stu-id="9fd84-123">The value for if MS Office InfoPath should be excluded or not.</span></span>|
|<span data-ttu-id="9fd84-124">Lync</span><span class="sxs-lookup"><span data-stu-id="9fd84-124">lync</span></span>|<span data-ttu-id="9fd84-125">Логический</span><span class="sxs-lookup"><span data-stu-id="9fd84-125">Boolean</span></span>|<span data-ttu-id="9fd84-126">Значение, если MS Office Skype для бизнеса — не следует исключать.</span><span class="sxs-lookup"><span data-stu-id="9fd84-126">The value for if MS Office Skype for Business - Lync should be excluded or not.</span></span>|
|<span data-ttu-id="9fd84-127">oneDrive</span><span class="sxs-lookup"><span data-stu-id="9fd84-127">oneDrive</span></span>|<span data-ttu-id="9fd84-128">Логический</span><span class="sxs-lookup"><span data-stu-id="9fd84-128">Boolean</span></span>|<span data-ttu-id="9fd84-129">Значение, которое должно быть исключено, если MS Office OneDrive должен быть исключен.</span><span class="sxs-lookup"><span data-stu-id="9fd84-129">The value for if MS Office OneDrive should be excluded or not.</span></span>|
|<span data-ttu-id="9fd84-130">Microsoft</span><span class="sxs-lookup"><span data-stu-id="9fd84-130">oneNote</span></span>|<span data-ttu-id="9fd84-131">Логический</span><span class="sxs-lookup"><span data-stu-id="9fd84-131">Boolean</span></span>|<span data-ttu-id="9fd84-132">Значение, если MS Office OneNote должен быть исключен или нет.</span><span class="sxs-lookup"><span data-stu-id="9fd84-132">The value for if MS Office OneNote should be excluded or not.</span></span>|
|<span data-ttu-id="9fd84-133">outlook</span><span class="sxs-lookup"><span data-stu-id="9fd84-133">outlook</span></span>|<span data-ttu-id="9fd84-134">Логический</span><span class="sxs-lookup"><span data-stu-id="9fd84-134">Boolean</span></span>|<span data-ttu-id="9fd84-135">Значение, если MS Office Outlook следует исключить из проверки.</span><span class="sxs-lookup"><span data-stu-id="9fd84-135">The value for if MS Office Outlook should be excluded or not.</span></span>|
|<span data-ttu-id="9fd84-136">powerPoint</span><span class="sxs-lookup"><span data-stu-id="9fd84-136">powerPoint</span></span>|<span data-ttu-id="9fd84-137">Логический</span><span class="sxs-lookup"><span data-stu-id="9fd84-137">Boolean</span></span>|<span data-ttu-id="9fd84-138">Значение, если MS Office PowerPoint следует исключить из проверки.</span><span class="sxs-lookup"><span data-stu-id="9fd84-138">The value for if MS Office PowerPoint should be excluded or not.</span></span>|
|<span data-ttu-id="9fd84-139">publisher</span><span class="sxs-lookup"><span data-stu-id="9fd84-139">publisher</span></span>|<span data-ttu-id="9fd84-140">Логический</span><span class="sxs-lookup"><span data-stu-id="9fd84-140">Boolean</span></span>|<span data-ttu-id="9fd84-141">Значение, если MS Office Publisher должен быть исключен или нет.</span><span class="sxs-lookup"><span data-stu-id="9fd84-141">The value for if MS Office Publisher should be excluded or not.</span></span>|
|<span data-ttu-id="9fd84-142">шарепоинтдесигнер</span><span class="sxs-lookup"><span data-stu-id="9fd84-142">sharePointDesigner</span></span>|<span data-ttu-id="9fd84-143">Логический</span><span class="sxs-lookup"><span data-stu-id="9fd84-143">Boolean</span></span>|<span data-ttu-id="9fd84-144">Значение для параметра if MS Office Шарепоинтдесигнер должно быть исключено или нет.</span><span class="sxs-lookup"><span data-stu-id="9fd84-144">The value for if MS Office SharePointDesigner should be excluded or not.</span></span>|
|<span data-ttu-id="9fd84-145">Teams</span><span class="sxs-lookup"><span data-stu-id="9fd84-145">teams</span></span>|<span data-ttu-id="9fd84-146">Логический</span><span class="sxs-lookup"><span data-stu-id="9fd84-146">Boolean</span></span>|<span data-ttu-id="9fd84-147">Значение, которое должно быть исключено, если MS Office Teams должен быть исключен.</span><span class="sxs-lookup"><span data-stu-id="9fd84-147">The value for if MS Office Teams should be excluded or not.</span></span>|
|<span data-ttu-id="9fd84-148">Visio</span><span class="sxs-lookup"><span data-stu-id="9fd84-148">visio</span></span>|<span data-ttu-id="9fd84-149">Логический</span><span class="sxs-lookup"><span data-stu-id="9fd84-149">Boolean</span></span>|<span data-ttu-id="9fd84-150">Значение, заданное для if MS Office Visio, должно быть исключено.</span><span class="sxs-lookup"><span data-stu-id="9fd84-150">The value for if MS Office Visio should be excluded or not.</span></span>|
|<span data-ttu-id="9fd84-151">текстовых</span><span class="sxs-lookup"><span data-stu-id="9fd84-151">word</span></span>|<span data-ttu-id="9fd84-152">Логический</span><span class="sxs-lookup"><span data-stu-id="9fd84-152">Boolean</span></span>|<span data-ttu-id="9fd84-153">Значение, заданное для if MS Office Word, должно быть исключено.</span><span class="sxs-lookup"><span data-stu-id="9fd84-153">The value for if MS Office Word should be excluded or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9fd84-154">Связи</span><span class="sxs-lookup"><span data-stu-id="9fd84-154">Relationships</span></span>
<span data-ttu-id="9fd84-155">Нет</span><span class="sxs-lookup"><span data-stu-id="9fd84-155">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9fd84-156">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9fd84-156">JSON Representation</span></span>
<span data-ttu-id="9fd84-157">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9fd84-157">Here is a JSON representation of the resource.</span></span>
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



