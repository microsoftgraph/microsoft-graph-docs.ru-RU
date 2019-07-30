---
author: JeremyKelley
ms.author: jeremyke
title: Тип ресурса пакета
description: Аспект, описывающий driveItem, который является логической группировкой других элементов driveitem
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 596dc8a77ce5b1e580b14e3e5c56c9e985b0dfbf
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932937"
---
# <a name="bundle-resource-type"></a><span data-ttu-id="59a27-103">Тип ресурса пакета</span><span class="sxs-lookup"><span data-stu-id="59a27-103">bundle resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59a27-104">Пакет — это логическая группа файлов, используемых для совместного использования нескольких файлов.</span><span class="sxs-lookup"><span data-stu-id="59a27-104">A bundle is a logical grouping of files used to share multiple files at once.</span></span> <span data-ttu-id="59a27-105">Он представлен объектом [driveItem][] , содержащим `bundle` аспект, и к нему можно предоставить доступ таким же образом, как и любой другой driveItem.</span><span class="sxs-lookup"><span data-stu-id="59a27-105">It is represented by a [driveItem][] entity containing a `bundle` facet and can be shared in the same way as any other driveItem.</span></span>

<span data-ttu-id="59a27-106">`bundle` Аспект в [driveItem][] определяет элемент как пакет и содержит сведения, относящиеся к пакету, в единую структуру.</span><span class="sxs-lookup"><span data-stu-id="59a27-106">The `bundle` facet on a [driveItem][] identifies an item as a bundle and groups bundle-specific information into a single structure.</span></span> <span data-ttu-id="59a27-107">Он включается только в ресурсы [driveItem][] , возвращенные из конечной точки " **пакеты** ".</span><span class="sxs-lookup"><span data-stu-id="59a27-107">It is only included on [driveItem][] resources returned from the **bundles** endpoint.</span></span>

<span data-ttu-id="59a27-108">Обратите внимание `bundle` , что сам тип ресурса сам по себе не является сущностью и является единственным аспектом [driveItem][].</span><span class="sxs-lookup"><span data-stu-id="59a27-108">Note that the `bundle` resource type itself is not an entity of its own, and is only a facet on a [driveItem][].</span></span> <span data-ttu-id="59a27-109">Коллекция на [диске][] имеет тип [driveItem][], а не `bundle` `bundles`</span><span class="sxs-lookup"><span data-stu-id="59a27-109">The `bundles` collection on a [drive][] is of type [driveItem][], not `bundle`.</span></span>

## <a name="methods"></a><span data-ttu-id="59a27-110">Методы</span><span class="sxs-lookup"><span data-stu-id="59a27-110">Methods</span></span>

|                        <span data-ttu-id="59a27-111">Метод</span><span class="sxs-lookup"><span data-stu-id="59a27-111">Method</span></span>             |         <span data-ttu-id="59a27-112">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="59a27-112">Return type</span></span>      | <span data-ttu-id="59a27-113">Описание</span><span class="sxs-lookup"><span data-stu-id="59a27-113">Description</span></span>        |
| :---------------------------------------- | :----------------------- | :------------------|
| <span data-ttu-id="59a27-114">[Пакеты списков][bundle-list]</span><span class="sxs-lookup"><span data-stu-id="59a27-114">[List bundles][bundle-list]</span></span>               | <span data-ttu-id="59a27-115">Коллекция [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="59a27-115">[driveItem][] collection</span></span> | <span data-ttu-id="59a27-116">Перечисление всех пакетов на диске</span><span class="sxs-lookup"><span data-stu-id="59a27-116">List all bundles in a drive</span></span> |
| <span data-ttu-id="59a27-117">[Получение пакета][bundle-get]</span><span class="sxs-lookup"><span data-stu-id="59a27-117">[Get bundle][bundle-get]</span></span>                  | <span data-ttu-id="59a27-118">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="59a27-118">[driveItem][]</span></span>            | <span data-ttu-id="59a27-119">Получение метаданных пакета</span><span class="sxs-lookup"><span data-stu-id="59a27-119">Get bundle metadata</span></span> |
| <span data-ttu-id="59a27-120">[Создание пакета][bundle-create]</span><span class="sxs-lookup"><span data-stu-id="59a27-120">[Create bundle][bundle-create]</span></span>            | <span data-ttu-id="59a27-121">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="59a27-121">[driveItem][]</span></span>            | <span data-ttu-id="59a27-122">Создание нового пакета</span><span class="sxs-lookup"><span data-stu-id="59a27-122">Create a new bundle</span></span> |
| <span data-ttu-id="59a27-123">[Добавление элемента][bundle-add-item]</span><span class="sxs-lookup"><span data-stu-id="59a27-123">[Add item][bundle-add-item]</span></span>               | <span data-ttu-id="59a27-124">Нет</span><span class="sxs-lookup"><span data-stu-id="59a27-124">None</span></span>                     | <span data-ttu-id="59a27-125">Добавление [driveItem][] в существующий пакет</span><span class="sxs-lookup"><span data-stu-id="59a27-125">Add a [driveItem][] to an existing bundle</span></span> |
| <span data-ttu-id="59a27-126">[Удаление элемента][bundle-remove-item]</span><span class="sxs-lookup"><span data-stu-id="59a27-126">[Remove item][bundle-remove-item]</span></span>         | <span data-ttu-id="59a27-127">Нет</span><span class="sxs-lookup"><span data-stu-id="59a27-127">None</span></span>                     | <span data-ttu-id="59a27-128">Удаление [driveItem][] из существующего пакета</span><span class="sxs-lookup"><span data-stu-id="59a27-128">Remove a [driveItem][] from an existing bundle</span></span> |
| <span data-ttu-id="59a27-129">[Пакет обновления][bundle-update]</span><span class="sxs-lookup"><span data-stu-id="59a27-129">[Update bundle][bundle-update]</span></span>            | <span data-ttu-id="59a27-130">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="59a27-130">[driveItem][]</span></span>            | <span data-ttu-id="59a27-131">Обновление метаданных пакета</span><span class="sxs-lookup"><span data-stu-id="59a27-131">Update bundle metadata</span></span> |
| <span data-ttu-id="59a27-132">[Удаление пакета][bundle-delete]</span><span class="sxs-lookup"><span data-stu-id="59a27-132">[Delete bundle][bundle-delete]</span></span>            | <span data-ttu-id="59a27-133">Нет</span><span class="sxs-lookup"><span data-stu-id="59a27-133">None</span></span>                     | <span data-ttu-id="59a27-134">Удаление пакета</span><span class="sxs-lookup"><span data-stu-id="59a27-134">Delete bundle</span></span> |


## <a name="properties"></a><span data-ttu-id="59a27-135">Свойства</span><span class="sxs-lookup"><span data-stu-id="59a27-135">Properties</span></span>

| <span data-ttu-id="59a27-136">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="59a27-136">Property name</span></span> | <span data-ttu-id="59a27-137">Тип</span><span class="sxs-lookup"><span data-stu-id="59a27-137">Type</span></span>      | <span data-ttu-id="59a27-138">Описание</span><span class="sxs-lookup"><span data-stu-id="59a27-138">Description</span></span>
|:--------------|:----------|:------------------------------------------------
| <span data-ttu-id="59a27-139">childCount</span><span class="sxs-lookup"><span data-stu-id="59a27-139">childCount</span></span>    | <span data-ttu-id="59a27-140">Int32</span><span class="sxs-lookup"><span data-stu-id="59a27-140">Int32</span></span>     | <span data-ttu-id="59a27-141">Количество дочерних объектов в корне данного контейнера.</span><span class="sxs-lookup"><span data-stu-id="59a27-141">Number of children contained immediately within this container.</span></span>
| <span data-ttu-id="59a27-142">album</span><span class="sxs-lookup"><span data-stu-id="59a27-142">album</span></span>         | <span data-ttu-id="59a27-143">[album][]</span><span class="sxs-lookup"><span data-stu-id="59a27-143">[album][]</span></span> | <span data-ttu-id="59a27-144">Если пакет является альбомом [][], то `album` свойство включается</span><span class="sxs-lookup"><span data-stu-id="59a27-144">If the bundle is an [album][], then the `album` property is included</span></span>

## <a name="json-representation"></a><span data-ttu-id="59a27-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="59a27-145">JSON representation</span></span>

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
