---
author: JeremyKelley
ms.date: 09/10/2017
title: SpecialFolder
ms.localizationpriority: medium
description: Ресурс SpecialFolder группирует элементы данных, связанные со специальной папкой, в единую структуру.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f8bef54bc709cb457bf30e0ce01e8a774d785cbf
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59136349"
---
# <a name="specialfolder-resource-type"></a>Тип ресурса SpecialFolder

Пространство имен: microsoft.graph

Ресурс **SpecialFolder** группирует элементы данных, связанные со специальной папкой, в единую структуру.

Если у элемента **DriveItem** есть аспект **specialFolder**, значение которого не равно null, то элемент представляет специальную (именованную) папку.
Прямой доступ к специальным папкам можно получить с помощью [коллекции специальных папок](../api/drive-get-specialfolder.md).

Специальные папки предоставляют простые псевдонимы для доступа к известным папкам, чтобы не нужно было искать папку по пути (что требует локализации) или ссылаться на папку по идентификатору. При переименовании специальной папки или ее перемещении в другое расположение на диске команда с таким синтаксисом будет по-прежнему возвращать эту папку.

Когда приложение впервые пробует записать что-то в специальную папку, она создается автоматически, если не была создана ранее. Если пользователь удалил такую папку, она создается повторно при записи в нее.

**Примечание.** Если ваше приложение запросило только область **Files.Read** и запрашивает специальную папку, которая не существует, в качестве отклика будет возвращена ошибка `403 Forbidden`.

## <a name="json-representation"></a>Представление JSON

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

## <a name="properties"></a>Свойства

| Свойство  | Тип   | Описание                                                            |
|:----------|:-------|:-----------------------------------------------------------------------|
| name      | string | Уникальный идентификатор для этого элемента в коллекции `/drive/special`. |

## <a name="special-folders"></a>Специальные папки

Вот специальные папки, доступные в OneDrive персональный и OneDrive для бизнеса.

| Имя        | Идентификатор папки    | Описание                                                              |
|:------------|:-------------|:-------------------------------------------------------------------------|
| Корневая папка приложения    | `approot`    | Личная папка приложения. Обычно расположена в папке `/Apps/{Application Name}` |
| Альбом камеры | `cameraroll` | Папка для резервных копий "Альбом камеры". Недоступна в OneDrive для бизнеса.   |
| Документы   | `documents`  | Папка "Документы".                                                    |
| Музыка       | `music`      | Папка "Музыка". Недоступна в OneDrive для бизнеса.                |
| Фотографии      | `photos`     | Папка "Фотографии".                                                       |

## <a name="remarks"></a>Заметки 

Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).

<!-- {
  "type": "#page.annotation",
  "description": "The SpecialFolder facet provides information about folders accessible as special folders.",
  "keywords": "special folder,item,facet",
  "section": "documentation",
  "tocPath": "Facets/SpecialFolder"
} -->

