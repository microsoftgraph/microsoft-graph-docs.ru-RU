---
author: swapnil1993
title: Тип ресурса documentSet
description: Содержит метаданные о параметрах набора документов.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: a3c0bc96cefaec37ff58f9f41f56c773f6c336cc
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59049524"
---
# <a name="documentset-resource-type"></a>Тип ресурса documentSet

Пространство имен: microsoft.graph

Представляет документ, установленный в SharePoint.

## <a name="properties"></a>Свойства

| Имя свойства  | Тип    | Описание|
|:---------------|:--------|:--------------------------------------------------|
| shouldPrefixNameToFile | Логический  | Добавьте имя установленного документа в каждое имя файла.|
| allowedContentTypes | Collection (microsoft.graph.contentTypeInfo) | Типы контента разрешены в наборе документов.|
| defaultContents     | Collection (microsoft.graph.documentSetContent) | Содержимое набора документов по умолчанию. | 
| propagateWelcomePageChanges | Логический | Указывает, следует ли нажимать изменения приветствия страниц на унаследованные типы контента.  |
| sharedColumns       | Коллекция (microsoft.graph.columnDefinition) | Столбцы, отредактированы в наборе документов, которые синхронизируются со всеми документами в наборе. Эти данные можно прочитать только в самих документах. |
| welcomePageColumns  | Коллекция (microsoft.graph.columnDefinition)  | Указывает столбцы, которые будут показываться на странице приветствия для набора документов.  |
| welcomePageUrl      | string | Url-адрес страницы welcome.  |

## <a name="json-representation"></a>Представление в формате JSON

Ниже приводится представление JSON ресурса **documentSet.**
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
