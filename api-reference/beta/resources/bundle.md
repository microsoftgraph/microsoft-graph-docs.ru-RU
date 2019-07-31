---
author: JeremyKelley
ms.author: jeremyke
title: Тип ресурса пакета
description: Аспект, описывающий driveItem, который является логической группировкой других элементов driveitem
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: f843afa112f95e391761d0c8804600018a67534c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974105"
---
# <a name="bundle-resource-type"></a><span data-ttu-id="2606d-103">Тип ресурса пакета</span><span class="sxs-lookup"><span data-stu-id="2606d-103">bundle resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2606d-104">Пакет — это логическая группа файлов, используемых для совместного использования нескольких файлов.</span><span class="sxs-lookup"><span data-stu-id="2606d-104">A bundle is a logical grouping of files used to share multiple files at once.</span></span> <span data-ttu-id="2606d-105">Он представлен объектом [driveItem][] , содержащим `bundle` аспект, и к нему можно предоставить доступ таким же образом, как и любой другой driveItem.</span><span class="sxs-lookup"><span data-stu-id="2606d-105">It is represented by a [driveItem][] entity containing a `bundle` facet and can be shared in the same way as any other driveItem.</span></span>

<span data-ttu-id="2606d-106">`bundle` Аспект в [driveItem][] определяет элемент как пакет и содержит сведения, относящиеся к пакету, в единую структуру.</span><span class="sxs-lookup"><span data-stu-id="2606d-106">The `bundle` facet on a [driveItem][] identifies an item as a bundle and groups bundle-specific information into a single structure.</span></span> <span data-ttu-id="2606d-107">Он включается только в ресурсы [driveItem][] , возвращенные из конечной точки " **пакеты** ".</span><span class="sxs-lookup"><span data-stu-id="2606d-107">It is only included on [driveItem][] resources returned from the **bundles** endpoint.</span></span>

<span data-ttu-id="2606d-108">Обратите внимание `bundle` , что сам тип ресурса сам по себе не является сущностью и является единственным аспектом [driveItem][].</span><span class="sxs-lookup"><span data-stu-id="2606d-108">Note that the `bundle` resource type itself is not an entity of its own, and is only a facet on a [driveItem][].</span></span> <span data-ttu-id="2606d-109">Коллекция на [диске][] имеет тип [driveItem][], а не `bundle` `bundles`</span><span class="sxs-lookup"><span data-stu-id="2606d-109">The `bundles` collection on a [drive][] is of type [driveItem][], not `bundle`.</span></span>

## <a name="methods"></a><span data-ttu-id="2606d-110">Методы</span><span class="sxs-lookup"><span data-stu-id="2606d-110">Methods</span></span>

|                        <span data-ttu-id="2606d-111">Метод</span><span class="sxs-lookup"><span data-stu-id="2606d-111">Method</span></span>             |         <span data-ttu-id="2606d-112">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="2606d-112">Return type</span></span>      | <span data-ttu-id="2606d-113">Описание</span><span class="sxs-lookup"><span data-stu-id="2606d-113">Description</span></span>        |
| :---------------------------------------- | :----------------------- | :------------------|
| <span data-ttu-id="2606d-114">[Пакеты списков][bundle-list]</span><span class="sxs-lookup"><span data-stu-id="2606d-114">[List bundles][bundle-list]</span></span>               | <span data-ttu-id="2606d-115">Коллекция [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="2606d-115">[driveItem][] collection</span></span> | <span data-ttu-id="2606d-116">Перечисление всех пакетов на диске</span><span class="sxs-lookup"><span data-stu-id="2606d-116">List all bundles in a drive</span></span> |
| <span data-ttu-id="2606d-117">[Получение пакета][bundle-get]</span><span class="sxs-lookup"><span data-stu-id="2606d-117">[Get bundle][bundle-get]</span></span>                  | <span data-ttu-id="2606d-118">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="2606d-118">[driveItem][]</span></span>            | <span data-ttu-id="2606d-119">Получение метаданных пакета</span><span class="sxs-lookup"><span data-stu-id="2606d-119">Get bundle metadata</span></span> |
| <span data-ttu-id="2606d-120">[Создание пакета][bundle-create]</span><span class="sxs-lookup"><span data-stu-id="2606d-120">[Create bundle][bundle-create]</span></span>            | <span data-ttu-id="2606d-121">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="2606d-121">[driveItem][]</span></span>            | <span data-ttu-id="2606d-122">Создание нового пакета</span><span class="sxs-lookup"><span data-stu-id="2606d-122">Create a new bundle</span></span> |
| <span data-ttu-id="2606d-123">[Добавление элемента][bundle-add-item]</span><span class="sxs-lookup"><span data-stu-id="2606d-123">[Add item][bundle-add-item]</span></span>               | <span data-ttu-id="2606d-124">Нет</span><span class="sxs-lookup"><span data-stu-id="2606d-124">None</span></span>                     | <span data-ttu-id="2606d-125">Добавление [driveItem][] в существующий пакет</span><span class="sxs-lookup"><span data-stu-id="2606d-125">Add a [driveItem][] to an existing bundle</span></span> |
| <span data-ttu-id="2606d-126">[Удаление элемента][bundle-remove-item]</span><span class="sxs-lookup"><span data-stu-id="2606d-126">[Remove item][bundle-remove-item]</span></span>         | <span data-ttu-id="2606d-127">Нет</span><span class="sxs-lookup"><span data-stu-id="2606d-127">None</span></span>                     | <span data-ttu-id="2606d-128">Удаление [driveItem][] из существующего пакета</span><span class="sxs-lookup"><span data-stu-id="2606d-128">Remove a [driveItem][] from an existing bundle</span></span> |
| <span data-ttu-id="2606d-129">[Пакет обновления][bundle-update]</span><span class="sxs-lookup"><span data-stu-id="2606d-129">[Update bundle][bundle-update]</span></span>            | <span data-ttu-id="2606d-130">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="2606d-130">[driveItem][]</span></span>            | <span data-ttu-id="2606d-131">Обновление метаданных пакета</span><span class="sxs-lookup"><span data-stu-id="2606d-131">Update bundle metadata</span></span> |
| <span data-ttu-id="2606d-132">[Удаление пакета][bundle-delete]</span><span class="sxs-lookup"><span data-stu-id="2606d-132">[Delete bundle][bundle-delete]</span></span>            | <span data-ttu-id="2606d-133">Нет</span><span class="sxs-lookup"><span data-stu-id="2606d-133">None</span></span>                     | <span data-ttu-id="2606d-134">Удаление пакета</span><span class="sxs-lookup"><span data-stu-id="2606d-134">Delete bundle</span></span> |


## <a name="properties"></a><span data-ttu-id="2606d-135">Свойства</span><span class="sxs-lookup"><span data-stu-id="2606d-135">Properties</span></span>

| <span data-ttu-id="2606d-136">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="2606d-136">Property name</span></span> | <span data-ttu-id="2606d-137">Тип</span><span class="sxs-lookup"><span data-stu-id="2606d-137">Type</span></span>      | <span data-ttu-id="2606d-138">Описание</span><span class="sxs-lookup"><span data-stu-id="2606d-138">Description</span></span>
|:--------------|:----------|:------------------------------------------------
| <span data-ttu-id="2606d-139">childCount</span><span class="sxs-lookup"><span data-stu-id="2606d-139">childCount</span></span>    | <span data-ttu-id="2606d-140">Int32</span><span class="sxs-lookup"><span data-stu-id="2606d-140">Int32</span></span>     | <span data-ttu-id="2606d-141">Количество дочерних объектов в корне данного контейнера.</span><span class="sxs-lookup"><span data-stu-id="2606d-141">Number of children contained immediately within this container.</span></span>
| <span data-ttu-id="2606d-142">album</span><span class="sxs-lookup"><span data-stu-id="2606d-142">album</span></span>         | <span data-ttu-id="2606d-143">[album][]</span><span class="sxs-lookup"><span data-stu-id="2606d-143">[album][]</span></span> | <span data-ttu-id="2606d-144">Если пакет является альбомом [][], то `album` свойство включается</span><span class="sxs-lookup"><span data-stu-id="2606d-144">If the bundle is an [album][], then the `album` property is included</span></span>

## <a name="json-representation"></a><span data-ttu-id="2606d-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2606d-145">JSON representation</span></span>

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
