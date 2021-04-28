---
title: тип ресурса softwareUpdateCatalogEntry
description: Метаданные для обновления программного обеспечения, которое можно утвердить для развертывания.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 3e6d0017860acbfc1371c1555279566e808da1eb
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52068149"
---
# <a name="softwareupdatecatalogentry-resource-type"></a><span data-ttu-id="d851f-103">тип ресурса softwareUpdateCatalogEntry</span><span class="sxs-lookup"><span data-stu-id="d851f-103">softwareUpdateCatalogEntry resource type</span></span>

<span data-ttu-id="d851f-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="d851f-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d851f-105">Метаданные для обновления программного обеспечения, которое можно утвердить для развертывания.</span><span class="sxs-lookup"><span data-stu-id="d851f-105">Metadata for a software update that you can approve for deployment.</span></span>

<span data-ttu-id="d851f-106">Наследует [из catalogEntry](../resources/windowsupdates-catalogentry.md).</span><span class="sxs-lookup"><span data-stu-id="d851f-106">Inherits from [catalogEntry](../resources/windowsupdates-catalogentry.md).</span></span> <span data-ttu-id="d851f-107">Базовый тип [для featureUpdateCatalogEntry](../resources/windowsupdates-featureupdatecatalogentry.md) и [qualityUpdateCatalogEntry.](../resources/windowsupdates-qualityupdatecatalogentry.md)</span><span class="sxs-lookup"><span data-stu-id="d851f-107">Base type for [featureUpdateCatalogEntry](../resources/windowsupdates-featureupdatecatalogentry.md) and [qualityUpdateCatalogEntry](../resources/windowsupdates-qualityupdatecatalogentry.md).</span></span>

<span data-ttu-id="d851f-108">Это абстрактный тип.</span><span class="sxs-lookup"><span data-stu-id="d851f-108">This is an abstract type.</span></span>

## <a name="properties"></a><span data-ttu-id="d851f-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="d851f-109">Properties</span></span>
|<span data-ttu-id="d851f-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="d851f-110">Property</span></span>|<span data-ttu-id="d851f-111">Тип</span><span class="sxs-lookup"><span data-stu-id="d851f-111">Type</span></span>|<span data-ttu-id="d851f-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d851f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d851f-113">deployableUntilDateTime</span><span class="sxs-lookup"><span data-stu-id="d851f-113">deployableUntilDateTime</span></span>|<span data-ttu-id="d851f-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d851f-114">DateTimeOffset</span></span>|<span data-ttu-id="d851f-115">Дата, в которую контент больше не доступен для развертывания с помощью службы.</span><span class="sxs-lookup"><span data-stu-id="d851f-115">The date on which the content is no longer available for deployment using the service.</span></span> <span data-ttu-id="d851f-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d851f-116">Read-only.</span></span> <span data-ttu-id="d851f-117">Унаследованный от [catalogEntry](../resources/windowsupdates-catalogentry.md).</span><span class="sxs-lookup"><span data-stu-id="d851f-117">Inherited from [catalogEntry](../resources/windowsupdates-catalogentry.md).</span></span>|
|<span data-ttu-id="d851f-118">displayName</span><span class="sxs-lookup"><span data-stu-id="d851f-118">displayName</span></span>|<span data-ttu-id="d851f-119">String</span><span class="sxs-lookup"><span data-stu-id="d851f-119">String</span></span>|<span data-ttu-id="d851f-120">Отображение имени контента.</span><span class="sxs-lookup"><span data-stu-id="d851f-120">The display name of the content.</span></span> <span data-ttu-id="d851f-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d851f-121">Read-only.</span></span> <span data-ttu-id="d851f-122">Унаследованный от [catalogEntry](../resources/windowsupdates-catalogentry.md).</span><span class="sxs-lookup"><span data-stu-id="d851f-122">Inherited from [catalogEntry](../resources/windowsupdates-catalogentry.md).</span></span>|
|<span data-ttu-id="d851f-123">id</span><span class="sxs-lookup"><span data-stu-id="d851f-123">id</span></span>|<span data-ttu-id="d851f-124">String</span><span class="sxs-lookup"><span data-stu-id="d851f-124">String</span></span>|<span data-ttu-id="d851f-125">Уникальный идентификатор для записи каталога.</span><span class="sxs-lookup"><span data-stu-id="d851f-125">The unique identifier for the catalog entry.</span></span> <span data-ttu-id="d851f-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d851f-126">Read-only.</span></span> <span data-ttu-id="d851f-127">Унаследованный от [catalogEntry](../resources/windowsupdates-catalogentry.md).</span><span class="sxs-lookup"><span data-stu-id="d851f-127">Inherited from [catalogEntry](../resources/windowsupdates-catalogentry.md).</span></span>|
|<span data-ttu-id="d851f-128">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="d851f-128">releaseDateTime</span></span>|<span data-ttu-id="d851f-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d851f-129">DateTimeOffset</span></span>|<span data-ttu-id="d851f-130">Дата выпуска контента.</span><span class="sxs-lookup"><span data-stu-id="d851f-130">The release date for the content.</span></span> <span data-ttu-id="d851f-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d851f-131">Read-only.</span></span> <span data-ttu-id="d851f-132">Унаследованный от [catalogEntry](../resources/windowsupdates-catalogentry.md).</span><span class="sxs-lookup"><span data-stu-id="d851f-132">Inherited from [catalogEntry](../resources/windowsupdates-catalogentry.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="d851f-133">Связи</span><span class="sxs-lookup"><span data-stu-id="d851f-133">Relationships</span></span>
<span data-ttu-id="d851f-134">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d851f-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d851f-135">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d851f-135">JSON representation</span></span>
<span data-ttu-id="d851f-136">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d851f-136">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.softwareUpdateCatalogEntry",
  "baseType": "microsoft.graph.windowsUpdates.catalogEntry",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.softwareUpdateCatalogEntry",
  "id": "String (identifier)",
  "displayName": "String",
  "releaseDateTime": "String (timestamp)",
  "deployableUntilDateTime": "String (timestamp)"
}
```

