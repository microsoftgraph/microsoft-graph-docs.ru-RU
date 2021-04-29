---
title: Тип ресурса siteSource
description: Контейнер для сайта, связанного с хранителями.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: c178565b628728fcf6124ea3058e979f8423ce90
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080479"
---
# <a name="sitesource-resource-type"></a><span data-ttu-id="99ca3-103">Тип ресурса siteSource</span><span class="sxs-lookup"><span data-stu-id="99ca3-103">siteSource resource type</span></span>

<span data-ttu-id="99ca3-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="99ca3-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99ca3-105">Контейнер для сайта, связанного с [хранителями.](ediscovery-custodian.md)</span><span class="sxs-lookup"><span data-stu-id="99ca3-105">The container for a site associated with a [custodian](ediscovery-custodian.md).</span></span>

## <a name="methods"></a><span data-ttu-id="99ca3-106">Методы</span><span class="sxs-lookup"><span data-stu-id="99ca3-106">Methods</span></span>

|<span data-ttu-id="99ca3-107">Метод</span><span class="sxs-lookup"><span data-stu-id="99ca3-107">Method</span></span>|<span data-ttu-id="99ca3-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="99ca3-108">Return type</span></span>|<span data-ttu-id="99ca3-109">Описание</span><span class="sxs-lookup"><span data-stu-id="99ca3-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="99ca3-110">List siteSources</span><span class="sxs-lookup"><span data-stu-id="99ca3-110">List siteSources</span></span>](../api/ediscovery-custodian-list-sitesources.md)|<span data-ttu-id="99ca3-111">[коллекция microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md)</span><span class="sxs-lookup"><span data-stu-id="99ca3-111">[microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) collection</span></span>|<span data-ttu-id="99ca3-112">Получите список **объектов siteSource** и их свойств.</span><span class="sxs-lookup"><span data-stu-id="99ca3-112">Get a list of **siteSource** objects and their properties.</span></span>|
|[<span data-ttu-id="99ca3-113">Создание siteSource</span><span class="sxs-lookup"><span data-stu-id="99ca3-113">Create siteSource</span></span>](../api/ediscovery-custodian-post-sitesources.md)|[<span data-ttu-id="99ca3-114">microsoft.graph.ediscovery.siteSource</span><span class="sxs-lookup"><span data-stu-id="99ca3-114">microsoft.graph.ediscovery.siteSource</span></span>](../resources/ediscovery-sitesource.md)|<span data-ttu-id="99ca3-115">Создание нового **объекта siteSource.**</span><span class="sxs-lookup"><span data-stu-id="99ca3-115">Create a new **siteSource** object.</span></span>|
|[<span data-ttu-id="99ca3-116">Get siteSource</span><span class="sxs-lookup"><span data-stu-id="99ca3-116">Get siteSource</span></span>](../api/ediscovery-sitesource-get.md)|[<span data-ttu-id="99ca3-117">microsoft.graph.ediscovery.siteSource</span><span class="sxs-lookup"><span data-stu-id="99ca3-117">microsoft.graph.ediscovery.siteSource</span></span>](../resources/ediscovery-sitesource.md)|<span data-ttu-id="99ca3-118">Ознакомьтесь с свойствами и отношениями **объекта siteSource.**</span><span class="sxs-lookup"><span data-stu-id="99ca3-118">Read the properties and relationships of a **siteSource** object.</span></span>|
|[<span data-ttu-id="99ca3-119">Удаление siteSource</span><span class="sxs-lookup"><span data-stu-id="99ca3-119">Delete siteSource</span></span>](../api/ediscovery-sitesource-delete.md)|<span data-ttu-id="99ca3-120">Нет</span><span class="sxs-lookup"><span data-stu-id="99ca3-120">None</span></span>|<span data-ttu-id="99ca3-121">Удаление **объекта siteSource.**</span><span class="sxs-lookup"><span data-stu-id="99ca3-121">Delete a **siteSource** object.</span></span>|

## <a name="properties"></a><span data-ttu-id="99ca3-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="99ca3-122">Properties</span></span>

|<span data-ttu-id="99ca3-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="99ca3-123">Property</span></span>|<span data-ttu-id="99ca3-124">Тип</span><span class="sxs-lookup"><span data-stu-id="99ca3-124">Type</span></span>|<span data-ttu-id="99ca3-125">Описание</span><span class="sxs-lookup"><span data-stu-id="99ca3-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99ca3-126">createdBy</span><span class="sxs-lookup"><span data-stu-id="99ca3-126">createdBy</span></span>|[<span data-ttu-id="99ca3-127">identitySet</span><span class="sxs-lookup"><span data-stu-id="99ca3-127">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="99ca3-128">Пользователь, создавший **сайтSource**.</span><span class="sxs-lookup"><span data-stu-id="99ca3-128">The user who created the **siteSource**.</span></span>|
|<span data-ttu-id="99ca3-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="99ca3-129">createdDateTime</span></span>|<span data-ttu-id="99ca3-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99ca3-130">DateTimeOffset</span></span>|<span data-ttu-id="99ca3-131">Дата и время **создания сайтаSource.**</span><span class="sxs-lookup"><span data-stu-id="99ca3-131">The date and time the **siteSource** was created.</span></span>|
|<span data-ttu-id="99ca3-132">displayName</span><span class="sxs-lookup"><span data-stu-id="99ca3-132">displayName</span></span>|<span data-ttu-id="99ca3-133">String</span><span class="sxs-lookup"><span data-stu-id="99ca3-133">String</span></span>|<span data-ttu-id="99ca3-134">Имя отображения **сайтаSource**.</span><span class="sxs-lookup"><span data-stu-id="99ca3-134">The display name of the **siteSource**.</span></span> <span data-ttu-id="99ca3-135">Это будет имя сайта SharePoint.</span><span class="sxs-lookup"><span data-stu-id="99ca3-135">This will be the name of the SharePoint site.</span></span>|
|<span data-ttu-id="99ca3-136">id</span><span class="sxs-lookup"><span data-stu-id="99ca3-136">id</span></span>|<span data-ttu-id="99ca3-137">String</span><span class="sxs-lookup"><span data-stu-id="99ca3-137">String</span></span>| <span data-ttu-id="99ca3-138">ID **сайтаSource**.</span><span class="sxs-lookup"><span data-stu-id="99ca3-138">The ID of the **siteSource**.</span></span> <span data-ttu-id="99ca3-139">Источник сайта можно получить в любое время с помощью [сайта Get](../api/site-get.md) - https://graph.microsoft.com/v1.0/sites/{siteId}</span><span class="sxs-lookup"><span data-stu-id="99ca3-139">The site source can be retrieved at any time with [Get site](../api/site-get.md) - https://graph.microsoft.com/v1.0/sites/{siteId}</span></span>|

## <a name="relationships"></a><span data-ttu-id="99ca3-140">Связи</span><span class="sxs-lookup"><span data-stu-id="99ca3-140">Relationships</span></span>

|<span data-ttu-id="99ca3-141">Связь</span><span class="sxs-lookup"><span data-stu-id="99ca3-141">Relationship</span></span>|<span data-ttu-id="99ca3-142">Тип</span><span class="sxs-lookup"><span data-stu-id="99ca3-142">Type</span></span>|<span data-ttu-id="99ca3-143">Описание</span><span class="sxs-lookup"><span data-stu-id="99ca3-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99ca3-144">site</span><span class="sxs-lookup"><span data-stu-id="99ca3-144">site</span></span>|[<span data-ttu-id="99ca3-145">site</span><span class="sxs-lookup"><span data-stu-id="99ca3-145">site</span></span>](../resources/site.md)|<span data-ttu-id="99ca3-146">Сайт SharePoint, связанный **с siteSource**.</span><span class="sxs-lookup"><span data-stu-id="99ca3-146">The SharePoint site associated with the **siteSource**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="99ca3-147">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="99ca3-147">JSON representation</span></span>

<span data-ttu-id="99ca3-148">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="99ca3-148">The following is a JSON representation of the resource.</span></span>
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
