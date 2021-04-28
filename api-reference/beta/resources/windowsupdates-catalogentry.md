---
title: тип ресурса catalogEntry
description: Метаданные для части контента, которую можно утвердить для развертывания.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 5c9766fd93c0a550556cb7f47e3275f65c238de7
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067532"
---
# <a name="catalogentry-resource-type"></a><span data-ttu-id="98b21-103">тип ресурса catalogEntry</span><span class="sxs-lookup"><span data-stu-id="98b21-103">catalogEntry resource type</span></span>

<span data-ttu-id="98b21-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="98b21-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98b21-105">Метаданные для части контента, которую можно утвердить для развертывания.</span><span class="sxs-lookup"><span data-stu-id="98b21-105">Metadata for a piece of content that you can approve for deployment.</span></span>

<span data-ttu-id="98b21-106">Все записи каталога существуют как один из следующих производных типов: [featureUpdateCatalogEntry](../resources/windowsupdates-featureupdatecatalogentry.md) и [qualityUpdateCatalogEntry.](../resources/windowsupdates-qualityupdatecatalogentry.md)</span><span class="sxs-lookup"><span data-stu-id="98b21-106">All catalog entries exist as one of the following derived types: [featureUpdateCatalogEntry](../resources/windowsupdates-featureupdatecatalogentry.md) and [qualityUpdateCatalogEntry](../resources/windowsupdates-qualityupdatecatalogentry.md).</span></span>

<span data-ttu-id="98b21-107">Базовый тип [для softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span><span class="sxs-lookup"><span data-stu-id="98b21-107">Base type for [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span></span>

<span data-ttu-id="98b21-108">Это абстрактный тип.</span><span class="sxs-lookup"><span data-stu-id="98b21-108">This is an abstract type.</span></span>

## <a name="properties"></a><span data-ttu-id="98b21-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="98b21-109">Properties</span></span>
|<span data-ttu-id="98b21-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="98b21-110">Property</span></span>|<span data-ttu-id="98b21-111">Тип</span><span class="sxs-lookup"><span data-stu-id="98b21-111">Type</span></span>|<span data-ttu-id="98b21-112">Описание</span><span class="sxs-lookup"><span data-stu-id="98b21-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98b21-113">deployableUntilDateTime</span><span class="sxs-lookup"><span data-stu-id="98b21-113">deployableUntilDateTime</span></span>|<span data-ttu-id="98b21-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="98b21-114">DateTimeOffset</span></span>|<span data-ttu-id="98b21-115">Дата, в которую контент больше не доступен для развертывания с помощью службы.</span><span class="sxs-lookup"><span data-stu-id="98b21-115">The date on which the content is no longer available to deploy using the service.</span></span> <span data-ttu-id="98b21-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="98b21-116">Read-only.</span></span>|
|<span data-ttu-id="98b21-117">displayName</span><span class="sxs-lookup"><span data-stu-id="98b21-117">displayName</span></span>|<span data-ttu-id="98b21-118">String</span><span class="sxs-lookup"><span data-stu-id="98b21-118">String</span></span>|<span data-ttu-id="98b21-119">Отображение имени контента.</span><span class="sxs-lookup"><span data-stu-id="98b21-119">The display name of the content.</span></span> <span data-ttu-id="98b21-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="98b21-120">Read-only.</span></span>|
|<span data-ttu-id="98b21-121">id</span><span class="sxs-lookup"><span data-stu-id="98b21-121">id</span></span>|<span data-ttu-id="98b21-122">String</span><span class="sxs-lookup"><span data-stu-id="98b21-122">String</span></span>|<span data-ttu-id="98b21-123">Уникальный идентификатор для записи каталога.</span><span class="sxs-lookup"><span data-stu-id="98b21-123">The unique identifier for the catalog entry.</span></span> <span data-ttu-id="98b21-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="98b21-124">Read-only.</span></span>|
|<span data-ttu-id="98b21-125">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="98b21-125">releaseDateTime</span></span>|<span data-ttu-id="98b21-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="98b21-126">DateTimeOffset</span></span>|<span data-ttu-id="98b21-127">Дата выпуска контента.</span><span class="sxs-lookup"><span data-stu-id="98b21-127">The release date for the content.</span></span> <span data-ttu-id="98b21-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="98b21-128">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="98b21-129">Связи</span><span class="sxs-lookup"><span data-stu-id="98b21-129">Relationships</span></span>
<span data-ttu-id="98b21-130">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="98b21-130">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="98b21-131">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="98b21-131">JSON representation</span></span>
<span data-ttu-id="98b21-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="98b21-132">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.catalogEntry",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.catalogEntry",
  "id": "String (identifier)",
  "displayName": "String",
  "releaseDateTime": "String (timestamp)",
  "deployableUntilDateTime": "String (timestamp)"
}
```

