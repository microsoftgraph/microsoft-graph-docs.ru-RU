---
author: JeremyKelley
ms.author: jeremyke
title: Тип ресурса "альбом"
description: Аспект, описывающий пакет, который представляет собой фотоальбом.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: b17a910a488e1fb5f051b4acc02d788a21d530d9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48067414"
---
# <a name="album-resource-type"></a>Тип ресурса "альбом"

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Фотоальбом — это способ, позволяющий объединить [элементов driveitem][driveItem] с аспектами [фото][] в [пакете][]. Для пакетов этого типа будет задано свойство **альбома** для ресурса [пакета][] .

## <a name="properties"></a>Свойства

| Имя свойства     | Тип   | Описание
|:------------------|:-------|:------------------------------------------------
| коверимажеитемид | String | Уникальный идентификатор [driveItem][] , который является титульным изображением альбома.

**Примечание:** Если ранее не было задано значение параметра **коверимажеитемид** , эскизы для альбома выбираются автоматически.
После настройки **коверимажеитемид** эскизы альбома всегда будут элементом, связанным с этим идентификатором. Вы можете переопределить обложку по умолчанию, заменив пакет [элементов пакета][и задав] для свойства **коверимажеитемид** значение `album` ID изображения, содержащегося в альбоме.
Чтобы удалить обложку настраиваемого набора, можно установить для свойства **коверимажеитемид** значение null, а значение по умолчанию будет выбрано автоматически.

## <a name="json-representation"></a>Представление JSON

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.album" } -->

```json
{
  "coverImageItemId": "string"
}
```

[bundle]: bundle.md
[driveItem]: driveItem.md
[photo]: photo.md


