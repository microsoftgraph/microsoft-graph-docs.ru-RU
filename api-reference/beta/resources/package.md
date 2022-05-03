---
author: JeremyKelley
description: " или коллекция элементов, которые должны рассматриваться как коллекция, а не отдельные элементы."
ms.date: 09/10/2017
title: Пакет
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: files
ms.openlocfilehash: 985b8bb918b0a54ef65253f2db13f0ca2345b64c
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176957"
---
# <a name="package-resource-type"></a>Тип ресурса Package

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **Package** указывает, что элемент DriveItem — это элемент верхнего уровня в "пакете" или коллекции элементов, с которыми следует обращаться как с коллекцией, а не как с отдельными элементами.

Пример пакета — записная книжка OneNote. Несмотря на то что записная книжка состоит из файлов и папок, представляющих ее содержимое, элемент верхнего уровня, который представляет записную книжку, имеет аспект **package**, с помощью которого можно информировать клиенты о том, что это коллекция данных, с которой необходимо обращаться особым образом.

Элементы DriveItem с аспектом **package** не включают аспект **folder** или **file**, но концептуально похожи на элемент с аспектом **folder**.

## <a name="json-representation"></a>Представление JSON

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.package" } -->
```json
{
  "type": "oneNote"
}
```

| Имя свойства | Тип   | Описание                                                                                                                                                                      |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **type**      | string | Строка, обозначающая тип пакета. Несмотря на то что `oneNote` — единственное значение, определенное на данный момент, следует ожидать, что могут быть возвращены пакеты других типов, и иметь возможность обработать их соответствующим образом. |

## <a name="remarks"></a>Заметки 

Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).


<!--
{
  "type": "#page.annotation",
  "description": "The Package facet indicates that an item is the root of a special collection of items that should be treated as a single unit.",
  "keywords": "package, facet, onenote",
  "section": "documentation",
  "suppressions": []
}
-->


