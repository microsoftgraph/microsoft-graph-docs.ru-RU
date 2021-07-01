---
author: JeremyKelley
description: Группы специальных элементов данных, связанных с папками, в одну структуру.
title: тип ресурса specialFolder
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: d9552c79588f8533980879c2ed49ed32fdfe7927
ms.sourcegitcommit: 0adbbcbc65b6acab80e9195f13321055994f56be
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2021
ms.locfileid: "53236273"
---
# <a name="specialfolder-resource-type"></a>тип ресурса specialFolder

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Группы специальных элементов данных, связанных с папками, в одну структуру.

Если **у driveItem** есть ненулевая грань **specialFolder,** элемент представляет специальную (именовую) папку.
Доступ к специальным папкам можно получить через [коллекцию специальных папок](../api/drive-get-specialfolder.md).

Специальные папки предоставляют простые псевдонимы для доступа к известным папкам, чтобы не нужно было искать папку по пути (что требует локализации) или ссылаться на папку по идентификатору. При переименовании специальной папки или ее перемещении в другое расположение на диске команда с таким синтаксисом будет по-прежнему возвращать эту папку.

Когда приложение впервые пробует записать что-то в специальную папку, она создается автоматически, если не была создана ранее. Если пользователь удалил такую папку, она создается повторно при записи в нее.

[!INCLUDE [files-special-folder-list](../includes/files-special-folder-list.md)]

>**Примечание.** Если ваше приложение запросило только область **Files.Read** и запрашивает специальную папку, которая не существует, в качестве отклика будет возвращена ошибка `403 Forbidden`.

## <a name="properties"></a>Свойства

| Свойство  | Тип   | Описание                                                            |
|:----------|:-------|:-----------------------------------------------------------------------|
| name      | string | Уникальный идентификатор для этого элемента в коллекции `/drive/special`. |


## <a name="json-representation"></a>Представление в формате JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.specialFolder"
}-->
```json
{
  "name": "string"
}
```

## <a name="see-also"></a>См. также 

Дополнительные сведения о гранях на driveItem см. [в сайте driveItem.](driveitem.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The SpecialFolder facet provides information about folders accessible as special folders.",
  "keywords": "special folder,item,facet",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


