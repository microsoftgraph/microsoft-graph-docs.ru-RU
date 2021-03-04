---
title: Тип ресурса siteSource
description: Контейнер для сайта, связанного с хранителями.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 4fa4b8d0ccbe80ef0f65d27fa8ef648d1ea07b63
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447359"
---
# <a name="sitesource-resource-type"></a><span data-ttu-id="3f7f2-103">Тип ресурса siteSource</span><span class="sxs-lookup"><span data-stu-id="3f7f2-103">siteSource resource type</span></span>

<span data-ttu-id="3f7f2-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="3f7f2-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f7f2-105">Контейнер для сайта, связанного с [хранителями.](ediscovery-custodian.md)</span><span class="sxs-lookup"><span data-stu-id="3f7f2-105">The container for a site associated with a [custodian](ediscovery-custodian.md).</span></span>

## <a name="methods"></a><span data-ttu-id="3f7f2-106">Методы</span><span class="sxs-lookup"><span data-stu-id="3f7f2-106">Methods</span></span>

|<span data-ttu-id="3f7f2-107">Метод</span><span class="sxs-lookup"><span data-stu-id="3f7f2-107">Method</span></span>|<span data-ttu-id="3f7f2-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="3f7f2-108">Return type</span></span>|<span data-ttu-id="3f7f2-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3f7f2-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3f7f2-110">List siteSources</span><span class="sxs-lookup"><span data-stu-id="3f7f2-110">List siteSources</span></span>](../api/ediscovery-custodian-list-sitesources.md)|<span data-ttu-id="3f7f2-111">[коллекция microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md)</span><span class="sxs-lookup"><span data-stu-id="3f7f2-111">[microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) collection</span></span>|<span data-ttu-id="3f7f2-112">Получите список **объектов siteSource** и их свойств.</span><span class="sxs-lookup"><span data-stu-id="3f7f2-112">Get a list of **siteSource** objects and their properties.</span></span>|
|[<span data-ttu-id="3f7f2-113">Создание siteSource</span><span class="sxs-lookup"><span data-stu-id="3f7f2-113">Create siteSource</span></span>](../api/ediscovery-custodian-post-sitesources.md)|[<span data-ttu-id="3f7f2-114">microsoft.graph.ediscovery.siteSource</span><span class="sxs-lookup"><span data-stu-id="3f7f2-114">microsoft.graph.ediscovery.siteSource</span></span>](../resources/ediscovery-sitesource.md)|<span data-ttu-id="3f7f2-115">Создание нового **объекта siteSource.**</span><span class="sxs-lookup"><span data-stu-id="3f7f2-115">Create a new **siteSource** object.</span></span>|
|[<span data-ttu-id="3f7f2-116">Get siteSource</span><span class="sxs-lookup"><span data-stu-id="3f7f2-116">Get siteSource</span></span>](../api/ediscovery-sitesource-get.md)|[<span data-ttu-id="3f7f2-117">microsoft.graph.ediscovery.siteSource</span><span class="sxs-lookup"><span data-stu-id="3f7f2-117">microsoft.graph.ediscovery.siteSource</span></span>](../resources/ediscovery-sitesource.md)|<span data-ttu-id="3f7f2-118">Ознакомьтесь с свойствами и отношениями **объекта siteSource.**</span><span class="sxs-lookup"><span data-stu-id="3f7f2-118">Read the properties and relationships of a **siteSource** object.</span></span>|
|[<span data-ttu-id="3f7f2-119">Удаление siteSource</span><span class="sxs-lookup"><span data-stu-id="3f7f2-119">Delete siteSource</span></span>](../api/ediscovery-sitesource-delete.md)|<span data-ttu-id="3f7f2-120">Нет</span><span class="sxs-lookup"><span data-stu-id="3f7f2-120">None</span></span>|<span data-ttu-id="3f7f2-121">Удаление **объекта siteSource.**</span><span class="sxs-lookup"><span data-stu-id="3f7f2-121">Delete a **siteSource** object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3f7f2-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="3f7f2-122">Properties</span></span>

|<span data-ttu-id="3f7f2-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="3f7f2-123">Property</span></span>|<span data-ttu-id="3f7f2-124">Тип</span><span class="sxs-lookup"><span data-stu-id="3f7f2-124">Type</span></span>|<span data-ttu-id="3f7f2-125">Описание</span><span class="sxs-lookup"><span data-stu-id="3f7f2-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f7f2-126">createdBy</span><span class="sxs-lookup"><span data-stu-id="3f7f2-126">createdBy</span></span>|[<span data-ttu-id="3f7f2-127">identitySet</span><span class="sxs-lookup"><span data-stu-id="3f7f2-127">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="3f7f2-128">Пользователь, создавший **сайтSource**.</span><span class="sxs-lookup"><span data-stu-id="3f7f2-128">The user who created the **siteSource**.</span></span>|
|<span data-ttu-id="3f7f2-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3f7f2-129">createdDateTime</span></span>|<span data-ttu-id="3f7f2-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f7f2-130">DateTimeOffset</span></span>|<span data-ttu-id="3f7f2-131">Дата и время **создания сайтаSource.**</span><span class="sxs-lookup"><span data-stu-id="3f7f2-131">The date and time the **siteSource** was created.</span></span>|
|<span data-ttu-id="3f7f2-132">displayName</span><span class="sxs-lookup"><span data-stu-id="3f7f2-132">displayName</span></span>|<span data-ttu-id="3f7f2-133">String</span><span class="sxs-lookup"><span data-stu-id="3f7f2-133">String</span></span>|<span data-ttu-id="3f7f2-134">Имя отображения **сайтаSource**.</span><span class="sxs-lookup"><span data-stu-id="3f7f2-134">The display name of the **siteSource**.</span></span> <span data-ttu-id="3f7f2-135">Это будет имя сайта SharePoint.</span><span class="sxs-lookup"><span data-stu-id="3f7f2-135">This will be the name of the SharePoint site.</span></span>|
|<span data-ttu-id="3f7f2-136">id</span><span class="sxs-lookup"><span data-stu-id="3f7f2-136">id</span></span>|<span data-ttu-id="3f7f2-137">String</span><span class="sxs-lookup"><span data-stu-id="3f7f2-137">String</span></span>| <span data-ttu-id="3f7f2-138">ID **сайтаSource**.</span><span class="sxs-lookup"><span data-stu-id="3f7f2-138">The ID of the **siteSource**.</span></span> <span data-ttu-id="3f7f2-139">Это не ID фактического сайта.</span><span class="sxs-lookup"><span data-stu-id="3f7f2-139">This is not the ID of the actual site.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3f7f2-140">Связи</span><span class="sxs-lookup"><span data-stu-id="3f7f2-140">Relationships</span></span>

|<span data-ttu-id="3f7f2-141">Связь</span><span class="sxs-lookup"><span data-stu-id="3f7f2-141">Relationship</span></span>|<span data-ttu-id="3f7f2-142">Тип</span><span class="sxs-lookup"><span data-stu-id="3f7f2-142">Type</span></span>|<span data-ttu-id="3f7f2-143">Описание</span><span class="sxs-lookup"><span data-stu-id="3f7f2-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f7f2-144">site</span><span class="sxs-lookup"><span data-stu-id="3f7f2-144">site</span></span>|[<span data-ttu-id="3f7f2-145">site</span><span class="sxs-lookup"><span data-stu-id="3f7f2-145">site</span></span>](../resources/site.md)|<span data-ttu-id="3f7f2-146">Сайт SharePoint, связанный с **siteSource.**</span><span class="sxs-lookup"><span data-stu-id="3f7f2-146">The SharePoint site associated with the **siteSource**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3f7f2-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3f7f2-147">JSON representation</span></span>

<span data-ttu-id="3f7f2-148">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3f7f2-148">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.siteSource",
  "baseType": "microsoft.graph.ediscovery.dataSource",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.siteSource",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "id": "String (identifier)"
}
```
