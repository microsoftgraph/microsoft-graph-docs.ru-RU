---
author: JeremyKelley
title: тип ресурса пакета
description: Facet, описывающий driveItem, который является логической группировкой других driveItems
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 9edf98faebc01fe23de16201fe5810eaa6db34fb
ms.sourcegitcommit: f5382652b6880fab42040df40a08de7cb2d74d35
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/17/2022
ms.locfileid: "63561642"
---
# <a name="bundle-resource-type"></a>тип ресурса пакета

Пространство имен: microsoft.graph

Пакет — это логическая группировка файлов, используемых для одновременного обмена несколькими файлами. Она представлена [объектом driveItem][]`bundle`, содержащим аспект, и может быть разделена таким же образом, как и любой другой driveItem.

Грань `bundle` на [driveItem][] определяет элемент как пакет и группу сведений, связанных с пакетом, в одну структуру. Он включен только в [ресурсы driveItem][] , возвращаемые из **конечной** точки пакетов.

Обратите внимание `bundle` , что сам тип ресурса не является самостоятельной сущностью и является только аспектом [на driveItem][]. Коллекция `bundles` на [диске имеет][] тип [driveItem][], а не `bundle`.

## <a name="methods"></a>Методы

|                        Метод             |         Тип возвращаемых данных      | Описание        |
| :---------------------------------------- | :----------------------- | :------------------|
| [Пакеты списков][bundle-list]               | Коллекция [driveItem][] | Список всех пакетов в диске |
| [Получить пакет][bundle-get]                  | [driveItem][]            | Получить метаданные пакета |
| [Создание пакета][bundle-create]            | [driveItem][]            | Создание нового пакета |
| [Добавление элемента][bundle-add-item]               | Нет                     | Добавление [driveItem в][] существующий пакет |
| [Удаление элемента][bundle-remove-item]         | Нет                     | Удаление [driveItem из][] существующего пакета |
| [Пакет обновления][bundle-update]            | [driveItem][]            | Обновление метаданных пакета |
| [Удаление пакета][bundle-delete]            | Нет                     | Удаление пакета |


## <a name="properties"></a>Свойства

| Имя свойства | Тип      | Описание
|:--------------|:----------|:------------------------------------------------
| childCount    | Int32     | Количество дочерних объектов в корне данного контейнера.
| album         | [album][] | Если пакет — [это альбом][], то `album` свойство включено

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


