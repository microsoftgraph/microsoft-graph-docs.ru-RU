---
author: JeremyKelley
ms.author: jeremyke
title: Тип ресурса пакета
description: Аспект, описывающий driveItem, который является логической группировкой других элементов driveitem
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: ae03674970c8861c7d1c158e62662d9691e74789
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507868"
---
# <a name="bundle-resource-type"></a><span data-ttu-id="6168a-103">Тип ресурса пакета</span><span class="sxs-lookup"><span data-stu-id="6168a-103">bundle resource type</span></span>

<span data-ttu-id="6168a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6168a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6168a-105">Пакет — это логическая группа файлов, используемых для совместного использования нескольких файлов.</span><span class="sxs-lookup"><span data-stu-id="6168a-105">A bundle is a logical grouping of files used to share multiple files at once.</span></span> <span data-ttu-id="6168a-106">Он представлен объектом [driveItem][] , содержащим `bundle` аспект, и к нему можно предоставить доступ таким же образом, как и любой другой driveItem.</span><span class="sxs-lookup"><span data-stu-id="6168a-106">It is represented by a [driveItem][] entity containing a `bundle` facet and can be shared in the same way as any other driveItem.</span></span>

<span data-ttu-id="6168a-107">`bundle` Аспект в [driveItem][] определяет элемент как пакет и содержит сведения, относящиеся к пакету, в единую структуру.</span><span class="sxs-lookup"><span data-stu-id="6168a-107">The `bundle` facet on a [driveItem][] identifies an item as a bundle and groups bundle-specific information into a single structure.</span></span> <span data-ttu-id="6168a-108">Он включается только в ресурсы [driveItem][] , возвращенные из конечной точки " **пакеты** ".</span><span class="sxs-lookup"><span data-stu-id="6168a-108">It is only included on [driveItem][] resources returned from the **bundles** endpoint.</span></span>

<span data-ttu-id="6168a-109">Обратите внимание `bundle` , что сам тип ресурса сам по себе не является сущностью и является единственным аспектом [driveItem][].</span><span class="sxs-lookup"><span data-stu-id="6168a-109">Note that the `bundle` resource type itself is not an entity of its own, and is only a facet on a [driveItem][].</span></span> <span data-ttu-id="6168a-110">Коллекция на [диске][] имеет тип [driveItem][], а не `bundle` `bundles`</span><span class="sxs-lookup"><span data-stu-id="6168a-110">The `bundles` collection on a [drive][] is of type [driveItem][], not `bundle`.</span></span>

## <a name="methods"></a><span data-ttu-id="6168a-111">Методы</span><span class="sxs-lookup"><span data-stu-id="6168a-111">Methods</span></span>

|                        <span data-ttu-id="6168a-112">Метод</span><span class="sxs-lookup"><span data-stu-id="6168a-112">Method</span></span>             |         <span data-ttu-id="6168a-113">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="6168a-113">Return type</span></span>      | <span data-ttu-id="6168a-114">Описание</span><span class="sxs-lookup"><span data-stu-id="6168a-114">Description</span></span>        |
| :---------------------------------------- | :----------------------- | :------------------|
| <span data-ttu-id="6168a-115">[Пакеты списков][bundle-list]</span><span class="sxs-lookup"><span data-stu-id="6168a-115">[List bundles][bundle-list]</span></span>               | <span data-ttu-id="6168a-116">Коллекция [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="6168a-116">[driveItem][] collection</span></span> | <span data-ttu-id="6168a-117">Перечисление всех пакетов на диске</span><span class="sxs-lookup"><span data-stu-id="6168a-117">List all bundles in a drive</span></span> |
| <span data-ttu-id="6168a-118">[Получение пакета][bundle-get]</span><span class="sxs-lookup"><span data-stu-id="6168a-118">[Get bundle][bundle-get]</span></span>                  | <span data-ttu-id="6168a-119">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="6168a-119">[driveItem][]</span></span>            | <span data-ttu-id="6168a-120">Получение метаданных пакета</span><span class="sxs-lookup"><span data-stu-id="6168a-120">Get bundle metadata</span></span> |
| <span data-ttu-id="6168a-121">[Создание пакета][bundle-create]</span><span class="sxs-lookup"><span data-stu-id="6168a-121">[Create bundle][bundle-create]</span></span>            | <span data-ttu-id="6168a-122">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="6168a-122">[driveItem][]</span></span>            | <span data-ttu-id="6168a-123">Создание нового пакета</span><span class="sxs-lookup"><span data-stu-id="6168a-123">Create a new bundle</span></span> |
| <span data-ttu-id="6168a-124">[Добавление элемента][bundle-add-item]</span><span class="sxs-lookup"><span data-stu-id="6168a-124">[Add item][bundle-add-item]</span></span>               | <span data-ttu-id="6168a-125">Нет</span><span class="sxs-lookup"><span data-stu-id="6168a-125">None</span></span>                     | <span data-ttu-id="6168a-126">Добавление [driveItem][] в существующий пакет</span><span class="sxs-lookup"><span data-stu-id="6168a-126">Add a [driveItem][] to an existing bundle</span></span> |
| <span data-ttu-id="6168a-127">[Удаление элемента][bundle-remove-item]</span><span class="sxs-lookup"><span data-stu-id="6168a-127">[Remove item][bundle-remove-item]</span></span>         | <span data-ttu-id="6168a-128">Нет</span><span class="sxs-lookup"><span data-stu-id="6168a-128">None</span></span>                     | <span data-ttu-id="6168a-129">Удаление [driveItem][] из существующего пакета</span><span class="sxs-lookup"><span data-stu-id="6168a-129">Remove a [driveItem][] from an existing bundle</span></span> |
| <span data-ttu-id="6168a-130">[Пакет обновления][bundle-update]</span><span class="sxs-lookup"><span data-stu-id="6168a-130">[Update bundle][bundle-update]</span></span>            | <span data-ttu-id="6168a-131">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="6168a-131">[driveItem][]</span></span>            | <span data-ttu-id="6168a-132">Обновление метаданных пакета</span><span class="sxs-lookup"><span data-stu-id="6168a-132">Update bundle metadata</span></span> |
| <span data-ttu-id="6168a-133">[Удаление пакета][bundle-delete]</span><span class="sxs-lookup"><span data-stu-id="6168a-133">[Delete bundle][bundle-delete]</span></span>            | <span data-ttu-id="6168a-134">Нет</span><span class="sxs-lookup"><span data-stu-id="6168a-134">None</span></span>                     | <span data-ttu-id="6168a-135">Удаление пакета</span><span class="sxs-lookup"><span data-stu-id="6168a-135">Delete bundle</span></span> |


## <a name="properties"></a><span data-ttu-id="6168a-136">Свойства</span><span class="sxs-lookup"><span data-stu-id="6168a-136">Properties</span></span>

| <span data-ttu-id="6168a-137">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="6168a-137">Property name</span></span> | <span data-ttu-id="6168a-138">Тип</span><span class="sxs-lookup"><span data-stu-id="6168a-138">Type</span></span>      | <span data-ttu-id="6168a-139">Описание</span><span class="sxs-lookup"><span data-stu-id="6168a-139">Description</span></span>
|:--------------|:----------|:------------------------------------------------
| <span data-ttu-id="6168a-140">childCount</span><span class="sxs-lookup"><span data-stu-id="6168a-140">childCount</span></span>    | <span data-ttu-id="6168a-141">Int32</span><span class="sxs-lookup"><span data-stu-id="6168a-141">Int32</span></span>     | <span data-ttu-id="6168a-142">Количество дочерних объектов в корне данного контейнера.</span><span class="sxs-lookup"><span data-stu-id="6168a-142">Number of children contained immediately within this container.</span></span>
| <span data-ttu-id="6168a-143">album</span><span class="sxs-lookup"><span data-stu-id="6168a-143">album</span></span>         | <span data-ttu-id="6168a-144">[album][]</span><span class="sxs-lookup"><span data-stu-id="6168a-144">[album][]</span></span> | <span data-ttu-id="6168a-145">Если пакет является [альбомом][], то `album` свойство включается</span><span class="sxs-lookup"><span data-stu-id="6168a-145">If the bundle is an [album][], then the `album` property is included</span></span>

## <a name="json-representation"></a><span data-ttu-id="6168a-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6168a-146">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.bundle" } -->
```json
{
  "childCount": 3,
  "album": { "@odata.type": "microsoft.graph.album" },
}
```

[album]: album.md
[drive]: drive.md
[driveItem]: driveItem.md

[bundle-list]: ../api/bundle-list.md
[bundle-get]: ../api/bundle-get.md
[bundle-create]: ../api/drive-post-bundles.md
[bundle-add-item]: ../api/bundle-addItem.md
[bundle-remove-item]: ../api/bundle-removeItem.md
[bundle-update]: ../api/bundle-update.md
[bundle-delete]: ../api/bundle-delete.md
