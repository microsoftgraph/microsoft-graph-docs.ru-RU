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
# <a name="bundle-resource-type"></a>Тип ресурса пакета

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Пакет — это логическая группа файлов, используемых для совместного использования нескольких файлов. Он представлен объектом [driveItem][] , содержащим `bundle` аспект, и к нему можно предоставить доступ таким же образом, как и любой другой driveItem.

`bundle` Аспект в [driveItem][] определяет элемент как пакет и содержит сведения, относящиеся к пакету, в единую структуру. Он включается только в ресурсы [driveItem][] , возвращенные из конечной точки " **пакеты** ".

Обратите внимание `bundle` , что сам тип ресурса сам по себе не является сущностью и является единственным аспектом [driveItem][]. Коллекция на [диске][] имеет тип [driveItem][], а не `bundle` `bundles`

## <a name="methods"></a>Методы

|                        Метод             |         Тип возвращаемых данных      | Описание        |
| :---------------------------------------- | :----------------------- | :------------------|
| [Пакеты списков][bundle-list]               | Коллекция [driveItem][] | Перечисление всех пакетов на диске |
| [Получение пакета][bundle-get]                  | [driveItem][]            | Получение метаданных пакета |
| [Создание пакета][bundle-create]            | [driveItem][]            | Создание нового пакета |
| [Добавление элемента][bundle-add-item]               | Нет                     | Добавление [driveItem][] в существующий пакет |
| [Удаление элемента][bundle-remove-item]         | Нет                     | Удаление [driveItem][] из существующего пакета |
| [Пакет обновления][bundle-update]            | [driveItem][]            | Обновление метаданных пакета |
| [Удаление пакета][bundle-delete]            | Нет                     | Удаление пакета |


## <a name="properties"></a>Свойства

| Имя свойства | Тип      | Описание
|:--------------|:----------|:------------------------------------------------
| childCount    | Int32     | Количество дочерних объектов в корне данного контейнера.
| album         | [album][] | Если пакет является альбомом [][], то `album` свойство включается

## <a name="json-representation"></a>Представление JSON

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
