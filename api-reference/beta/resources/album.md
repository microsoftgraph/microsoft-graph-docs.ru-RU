---
author: JeremyKelley
ms.author: jeremyke
title: Тип ресурса "альбом"
description: Аспект, описывающий пакет, который представляет собой фотоальбом.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 60d653db52f71de6fe4079df25223b393ea18da3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508361"
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
После настройки **коверимажеитемид** эскизы альбома всегда будут элементом, связанным с этим идентификатором. Вы можете переопределить обложку по умолчанию, заменив пакет [элементов пакета][и задав] `album` для свойства **коверимажеитемид** значение ID изображения, содержащегося в альбоме.
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
