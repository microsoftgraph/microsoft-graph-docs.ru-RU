---
author: swapnil1993
title: Тип ресурса documentSet
description: Содержит метаданные о параметрах набора документов.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: c39eeb8689f882939d506eb8e68e2d6c9409e350
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/22/2022
ms.locfileid: "63721664"
---
# <a name="documentset-resource-type"></a>Тип ресурса documentSet

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
Содержит метаданные о параметрах набора документов.

## <a name="properties"></a>Свойства

| Свойство                    | Тип                                           | Описание                                                                                                                       |
| :-------------------------- | :--------------------------------------------- | :-------------------------------------------------------------------------------------------------------------------------------- |
| shouldPrefixNameToFile      | Boolean                                        | Добавьте имя набора документов в каждое имя файла.                                                                               |
| allowedContentTypes         | Collection (microsoft.graph.contentTypeInfo)    | Типы контента разрешены в наборе документов.                                                                                            |
| defaultContents             | Collection(microsoft.graph.documentSetContent) | Содержимое набора документов по умолчанию.                                                                                                 |
| propagateWelcomePageChanges | Boolean                                        | Указывает, следует ли нажимать изменения приветствия страниц на унаследованные типы контента.                                                        |
| sharedColumns               | Коллекция (microsoft.graph.columnDefinition)   | Столбцы, отредактированы в наборе документов, которые синхронизируются со всеми документами в наборе. Эти данные можно прочитать только в самих документах. |
| welcomePageColumns          | Коллекция (microsoft.graph.columnDefinition)   | Указывает столбцы, которые будут показываться на странице приветствия для набора документов.                                                               |
| welcomePageUrl              | строка                                         | Url-адрес страницы welcome.                                                                                                        |

## <a name="json-representation"></a>Представление JSON

Ниже приводится представление JSON ресурса **documentSet** .

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.documentSet" } -->

```json
{
  "shouldPrefixNameToFile": true,
  "allowedContentTypes": [{ "@type": "microsoft.graph.contentTypeInfo" }],
  "defaultContents": [{ "@type": "microsoft.graph.documentSetContent" }],
  "propagateWelcomePageChanges": false,
  "sharedColumns": [{ "@type": "microsoft.graph.columnDefinition" }],
  "welcomePageColumns": [{ "@type": "microsoft.graph.columnDefinition" }],
  "welcomePageUrl": "string"
}
```

[contentTypeInfo]: contentTypeInfo.md
[documentSetContent]: documentsetcontent.md
