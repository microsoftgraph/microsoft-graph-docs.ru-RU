---
title: тип ресурса qualityUpdateCatalogEntry
description: Метаданные для обновления Windows 10 качества, которое можно утвердить для развертывания.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: f455919bfc3d5f0e6c4e2aa5ef6a6b630b66bc52
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52068082"
---
# <a name="qualityupdatecatalogentry-resource-type"></a><span data-ttu-id="aae9c-103">тип ресурса qualityUpdateCatalogEntry</span><span class="sxs-lookup"><span data-stu-id="aae9c-103">qualityUpdateCatalogEntry resource type</span></span>

<span data-ttu-id="aae9c-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="aae9c-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aae9c-105">Метаданные для обновления Windows 10 качества, которое можно утвердить для развертывания.</span><span class="sxs-lookup"><span data-stu-id="aae9c-105">Metadata for a Windows 10 quality update that you can be approve for deployment.</span></span>

<span data-ttu-id="aae9c-106">Windows 10 обновления качества выпускаются один или несколько раз в месяц.</span><span class="sxs-lookup"><span data-stu-id="aae9c-106">Windows 10 quality updates are released one or more times per month.</span></span> <span data-ttu-id="aae9c-107">Эти обновления содержат исправления безопасности и качества и обычно выпускаются во второй вторник каждого месяца, хотя они могут быть выпущены в любое время.</span><span class="sxs-lookup"><span data-stu-id="aae9c-107">These updates contain both security and quality fixes and are typically released on the second Tuesday of every month, though they may be released at any time.</span></span> <span data-ttu-id="aae9c-108">Эти обновления являются накопительными, поэтому более поздние версии всегда содержат все предыдущие исправления.</span><span class="sxs-lookup"><span data-stu-id="aae9c-108">These updates are cumulative, so later versions always contain all previous fixes.</span></span> <span data-ttu-id="aae9c-109">Корпорация Майкрософт настоятельно рекомендует сохранять устройства текущими, устанавливая последние обновления качества, как только они будут доступны.</span><span class="sxs-lookup"><span data-stu-id="aae9c-109">Microsoft strongly recommends keeping devices current by installing the most recent quality updates as soon as they are available.</span></span> 

<span data-ttu-id="aae9c-110">Наследует от [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span><span class="sxs-lookup"><span data-stu-id="aae9c-110">Inherits from [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span></span>

## <a name="properties"></a><span data-ttu-id="aae9c-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="aae9c-111">Properties</span></span>
|<span data-ttu-id="aae9c-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="aae9c-112">Property</span></span>|<span data-ttu-id="aae9c-113">Тип</span><span class="sxs-lookup"><span data-stu-id="aae9c-113">Type</span></span>|<span data-ttu-id="aae9c-114">Описание</span><span class="sxs-lookup"><span data-stu-id="aae9c-114">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aae9c-115">deployableUntilDateTime</span><span class="sxs-lookup"><span data-stu-id="aae9c-115">deployableUntilDateTime</span></span>|<span data-ttu-id="aae9c-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aae9c-116">DateTimeOffset</span></span>|<span data-ttu-id="aae9c-117">Дата, в которую контент больше не доступен для развертывания с помощью службы.</span><span class="sxs-lookup"><span data-stu-id="aae9c-117">The date on which the content is no longer available for deployment using the service.</span></span> <span data-ttu-id="aae9c-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="aae9c-118">Read-only.</span></span> <span data-ttu-id="aae9c-119">Унаследовано от [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span><span class="sxs-lookup"><span data-stu-id="aae9c-119">Inherited from [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span></span>|
|<span data-ttu-id="aae9c-120">displayName</span><span class="sxs-lookup"><span data-stu-id="aae9c-120">displayName</span></span>|<span data-ttu-id="aae9c-121">String</span><span class="sxs-lookup"><span data-stu-id="aae9c-121">String</span></span>|<span data-ttu-id="aae9c-122">Отображение имени контента.</span><span class="sxs-lookup"><span data-stu-id="aae9c-122">The display name of the content.</span></span> <span data-ttu-id="aae9c-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="aae9c-123">Read-only.</span></span> <span data-ttu-id="aae9c-124">Унаследовано от [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span><span class="sxs-lookup"><span data-stu-id="aae9c-124">Inherited from [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span></span>|
|<span data-ttu-id="aae9c-125">id</span><span class="sxs-lookup"><span data-stu-id="aae9c-125">id</span></span>|<span data-ttu-id="aae9c-126">String</span><span class="sxs-lookup"><span data-stu-id="aae9c-126">String</span></span>|<span data-ttu-id="aae9c-127">Уникальный идентификатор для записи каталога.</span><span class="sxs-lookup"><span data-stu-id="aae9c-127">The unique identifier for the catalog entry.</span></span> <span data-ttu-id="aae9c-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="aae9c-128">Read-only.</span></span> <span data-ttu-id="aae9c-129">Унаследовано от [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span><span class="sxs-lookup"><span data-stu-id="aae9c-129">Inherited from [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span></span>|
|<span data-ttu-id="aae9c-130">isExpeditable</span><span class="sxs-lookup"><span data-stu-id="aae9c-130">isExpeditable</span></span>|<span data-ttu-id="aae9c-131">Логический</span><span class="sxs-lookup"><span data-stu-id="aae9c-131">Boolean</span></span>|<span data-ttu-id="aae9c-132">Указывает, можно ли развертывать контент в качестве ускоренного обновления качества.</span><span class="sxs-lookup"><span data-stu-id="aae9c-132">Indicates whether the content can be deployed as an expedited quality update.</span></span> <span data-ttu-id="aae9c-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="aae9c-133">Read-only.</span></span>|
|<span data-ttu-id="aae9c-134">qualityUpdateClassification</span><span class="sxs-lookup"><span data-stu-id="aae9c-134">qualityUpdateClassification</span></span>|<span data-ttu-id="aae9c-135">microsoft.graph.windowsUpdates.qualityUpdateClassification</span><span class="sxs-lookup"><span data-stu-id="aae9c-135">microsoft.graph.windowsUpdates.qualityUpdateClassification</span></span>|<span data-ttu-id="aae9c-136">Классификация обновления качества.</span><span class="sxs-lookup"><span data-stu-id="aae9c-136">The classification on the quality update.</span></span> <span data-ttu-id="aae9c-137">Поддерживает подмножество значений **для qualityUpdateClassification.**</span><span class="sxs-lookup"><span data-stu-id="aae9c-137">Supports a subset of the values for **qualityUpdateClassification**.</span></span> <span data-ttu-id="aae9c-138">Возможные значения: `all`, `security`, `nonSecurity`.</span><span class="sxs-lookup"><span data-stu-id="aae9c-138">Possible values are: `all`, `security`, `nonSecurity`.</span></span> <span data-ttu-id="aae9c-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="aae9c-139">Read-only.</span></span>|
|<span data-ttu-id="aae9c-140">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="aae9c-140">releaseDateTime</span></span>|<span data-ttu-id="aae9c-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aae9c-141">DateTimeOffset</span></span>|<span data-ttu-id="aae9c-142">Дата выпуска контента.</span><span class="sxs-lookup"><span data-stu-id="aae9c-142">The release date of the content.</span></span> <span data-ttu-id="aae9c-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="aae9c-143">Read-only.</span></span> <span data-ttu-id="aae9c-144">Унаследовано от [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span><span class="sxs-lookup"><span data-stu-id="aae9c-144">Inherited from [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="aae9c-145">Связи</span><span class="sxs-lookup"><span data-stu-id="aae9c-145">Relationships</span></span>
<span data-ttu-id="aae9c-146">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="aae9c-146">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="aae9c-147">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="aae9c-147">JSON representation</span></span>
<span data-ttu-id="aae9c-148">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aae9c-148">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.qualityUpdateCatalogEntry",
  "baseType": "microsoft.graph.windowsUpdates.softwareUpdateCatalogEntry",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.qualityUpdateCatalogEntry",
  "id": "String (identifier)",
  "displayName": "String",
  "releaseDateTime": "String (timestamp)",
  "deployableUntilDateTime": "String (timestamp)",
  "isExpeditable": "Boolean",
  "qualityUpdateClassification": "String"
}
```

