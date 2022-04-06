---
author: swapnil1993
title: Тип ресурса documentSet
description: Содержит метаданные о параметрах набора документов.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: d6a997dd721200eb732f83fb53bbb3155921f111
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2022
ms.locfileid: "63758300"
---
# <a name="documentset-resource-type"></a>Тип ресурса documentSet

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
Содержит метаданные о параметрах набора документов.

## <a name="properties"></a>Свойства

| Свойство                    | Тип                                           | Описание                                                                                                                       |
| :-------------------------- | :--------------------------------------------- | :-------------------------------------------------------------------------------------------------------------------------------- |
| allowedContentTypes         | Collection (microsoft.graph.contentTypeInfo)    | Типы контента разрешены в наборе документов.                                                                                            |
| defaultContents             | Collection(microsoft.graph.documentSetContent) | Содержимое набора документов по умолчанию.                                                                                                 |
| propagateWelcomePageChanges | Boolean                                        | Указывает, следует ли добавлять имя установленного документа в каждое имя файла.                                                          |
| shouldPrefixNameToFile      | Логическое                                        | Добавьте имя набора документов в каждое имя файла.                                                                               |
| welcomePageUrl              | String                                         | Url-адрес страницы welcome.                                                                                                        |

## <a name="relationships"></a>Связи

| Связь   | Тип                      | Описание
|:----------------|:--------------------------|:-------------------------------
| sharedColumns       | Коллекция (microsoft.graph.columnDefinition) | Столбцы, отредактированы в наборе документов, которые синхронизируются со всеми документами в наборе. Эти данные можно прочитать только в самих документах. 
| welcomePageColumns  | Коллекция (microsoft.graph.columnDefinition)  | Указывает столбцы, которые будут показываться на странице приветствия для набора документов.

## <a name="json-representation"></a>Представление JSON

Ниже приводится представление JSON ресурса **documentSet** .

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.documentSet" } -->

```json
{
  "shouldPrefixNameToFile": true,
  "allowedContentTypes": [{ "@type": "microsoft.graph.contentTypeInfo" }],
  "defaultContents": [{ "@type": "microsoft.graph.documentSetContent" }],
  "propagateWelcomePageChanges": false,
  "welcomePageUrl": "string"
}
```

[contentTypeInfo]: contentTypeInfo.md
[documentSetContent]: documentsetcontent.md
