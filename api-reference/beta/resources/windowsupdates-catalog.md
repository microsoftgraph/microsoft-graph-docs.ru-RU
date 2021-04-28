---
title: Тип ресурса каталога
description: Объект, представляющий каталог контента, который можно утвердить для развертывания.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 3fc0630a36d123e6c3e208838d81ee7c33c62853
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52068215"
---
# <a name="catalog-resource-type"></a><span data-ttu-id="d4507-103">Тип ресурса каталога</span><span class="sxs-lookup"><span data-stu-id="d4507-103">catalog resource type</span></span>

<span data-ttu-id="d4507-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="d4507-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4507-105">Объект, представляющий каталог контента, который можно утвердить для развертывания.</span><span class="sxs-lookup"><span data-stu-id="d4507-105">Entity representing the catalog of content that you can approve for deployment.</span></span>

## <a name="methods"></a><span data-ttu-id="d4507-106">Методы</span><span class="sxs-lookup"><span data-stu-id="d4507-106">Methods</span></span>
|<span data-ttu-id="d4507-107">Метод</span><span class="sxs-lookup"><span data-stu-id="d4507-107">Method</span></span>|<span data-ttu-id="d4507-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="d4507-108">Return type</span></span>|<span data-ttu-id="d4507-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d4507-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d4507-110">Записи списка</span><span class="sxs-lookup"><span data-stu-id="d4507-110">List entries</span></span>](../api/windowsupdates-catalog-list-entries.md)|<span data-ttu-id="d4507-111">[коллекция microsoft.graph.windowsUpdates.catalogEntry](../resources/windowsupdates-catalogentry.md)</span><span class="sxs-lookup"><span data-stu-id="d4507-111">[microsoft.graph.windowsUpdates.catalogEntry](../resources/windowsupdates-catalogentry.md) collection</span></span>|<span data-ttu-id="d4507-112">Получите ресурсы [catalogEntry](../resources/windowsupdates-catalogentry.md) из свойства навигации записей.</span><span class="sxs-lookup"><span data-stu-id="d4507-112">Get the [catalogEntry](../resources/windowsupdates-catalogentry.md) resources from the entries navigation property.</span></span> <span data-ttu-id="d4507-113">Возвращает **ресурсы catalogEntry** следующих производных типов: [featureUpdateCatalogEntry](../resources/windowsupdates-featureupdatecatalogentry.md), [qualityUpdateCatalogEntry](../resources/windowsupdates-qualityupdatecatalogentry.md).</span><span class="sxs-lookup"><span data-stu-id="d4507-113">Returns **catalogEntry** resources of the following derived types: [featureUpdateCatalogEntry](../resources/windowsupdates-featureupdatecatalogentry.md), [qualityUpdateCatalogEntry](../resources/windowsupdates-qualityupdatecatalogentry.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="d4507-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="d4507-114">Properties</span></span>
|<span data-ttu-id="d4507-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="d4507-115">Property</span></span>|<span data-ttu-id="d4507-116">Тип</span><span class="sxs-lookup"><span data-stu-id="d4507-116">Type</span></span>|<span data-ttu-id="d4507-117">Описание</span><span class="sxs-lookup"><span data-stu-id="d4507-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4507-118">id</span><span class="sxs-lookup"><span data-stu-id="d4507-118">id</span></span>|<span data-ttu-id="d4507-119">String</span><span class="sxs-lookup"><span data-stu-id="d4507-119">String</span></span>|<span data-ttu-id="d4507-120">Идентификатор каталога.</span><span class="sxs-lookup"><span data-stu-id="d4507-120">An identifier for the catalog.</span></span> <span data-ttu-id="d4507-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d4507-121">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d4507-122">Связи</span><span class="sxs-lookup"><span data-stu-id="d4507-122">Relationships</span></span>
|<span data-ttu-id="d4507-123">Связь</span><span class="sxs-lookup"><span data-stu-id="d4507-123">Relationship</span></span>|<span data-ttu-id="d4507-124">Тип</span><span class="sxs-lookup"><span data-stu-id="d4507-124">Type</span></span>|<span data-ttu-id="d4507-125">Описание</span><span class="sxs-lookup"><span data-stu-id="d4507-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4507-126">записи</span><span class="sxs-lookup"><span data-stu-id="d4507-126">entries</span></span>|<span data-ttu-id="d4507-127">[коллекция microsoft.graph.windowsUpdates.catalogEntry](../resources/windowsupdates-catalogentry.md)</span><span class="sxs-lookup"><span data-stu-id="d4507-127">[microsoft.graph.windowsUpdates.catalogEntry](../resources/windowsupdates-catalogentry.md) collection</span></span>|<span data-ttu-id="d4507-128">Списки содержимого, которое можно утвердить для развертывания.</span><span class="sxs-lookup"><span data-stu-id="d4507-128">Lists the content that you can approve for deployment.</span></span> <span data-ttu-id="d4507-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d4507-129">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d4507-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d4507-130">JSON representation</span></span>
<span data-ttu-id="d4507-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d4507-131">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.catalog",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.catalog",
  "id": "String (identifier)"
}
```

