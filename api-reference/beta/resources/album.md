---
author: JeremyKelley
title: Тип ресурса альбома
description: Facet, описывающий пакет, который является фотоальбомом.
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 0f35eea761a467ce1a733f07fca5c33a218be030
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/22/2022
ms.locfileid: "63723224"
---
# <a name="album-resource-type"></a>Тип ресурса альбома

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Фотоальбом — это способ фактически группировать [driveItemsdriveItem][] с [][] фотоконкурсами вместе в [пакете][]. Пакеты этого типа будут иметь свойство **альбома** , заданной на [ресурсе пакета][] .

## <a name="properties"></a>Свойства

| Свойство         | Тип   | Описание                                                            |
| :--------------- | :----- | :--------------------------------------------------------------------- |
| coverImageItemId | String | Уникальный идентификатор [driveItem][] , который является обложкой альбома. |

**Примечание:** Если **coverImageItemId** еще не задан, эскизы для альбома выбираются автоматически.
После **набора coverImageItemId** эскизы для альбома всегда будут элементом, связанным с этим id. Вы можете переопредить крышку по умолчанию путем PATCHing [][itembundle] пакета и задав свойство **coverImageItemId** `album` в id изображения, содержатого в альбоме.
Чтобы удалить настраиваемую крышку, можно установить свойство **coverImageItemId** на нуль, и по умолчанию оно будет выбрано автоматически.

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
