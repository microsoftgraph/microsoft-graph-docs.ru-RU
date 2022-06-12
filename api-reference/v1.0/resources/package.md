---
author: Title: Package ms.localizationpriority: medium description: "Indicates that a driveItem is the top-level item in a "package" or a collection of items that should be treated as a collection instead of individual items".
ms.prod: files doc_type: resourcePageType
---

# <a name="package-resource-type"></a>Тип ресурса пакета

Пространство имен: microsoft.graph

Ресурс **пакета** указывает, что **driveItem** является элементом верхнего уровня в "пакете" или коллекции элементов, которые должны рассматриваться как коллекция, а не отдельные элементы.

Пример пакета — записная книжка OneNote. Несмотря на то что записная книжка состоит из файлов и папок, представляющих ее содержимое, элемент верхнего уровня, который представляет записную книжку, имеет аспект **package**, с помощью которого можно информировать клиенты о том, что это коллекция данных, с которой необходимо обращаться особым образом.

**Объекты driveItems** с аспектом пакета не включают аспект  папки или  файла, но концептуально похожи на элемент с **аспектом папки**.

## <a name="json-representation"></a>Представление JSON

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.package" } -->
```json
{
  "type": "oneNote"
}
```

## <a name="properties"></a>Свойства

| Имя свойства | Тип   | Описание                                                                                                                                                                      |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| type          | string | Строка, указывающая тип пакета. Несмотря на то что `oneNote`— единственное значение, определенное на данный момент, следует ожидать, что могут быть возвращены пакеты других типов, и иметь возможность обработать их соответствующим образом. |

## <a name="remarks"></a>Заметки 

Дополнительные сведения о аспектах в DriveItem см. [в разделе driveItem](driveitem.md).


<!-- {
  "type": "#page.annotation",
  "description": "The Package facet indicates that an item is the root of a special collection of items that should be treated as a single unit.",
  "keywords": "package, facet, onenote",
  "section": "documentation",
  "tocPath": "Facets/Package"
} -->

