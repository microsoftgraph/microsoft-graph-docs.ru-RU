---
author: swapnil1993
title: Тип ресурса documentSet
description: Содержит метаданные о параметрах набора документов.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 25a2b5e71c76a8a097ff9c490313ae6d319abeb8
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447399"
---
# <a name="documentset-resource-type"></a>Тип ресурса documentSet

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
Содержит метаданные о параметрах набора документов.

## <a name="properties"></a>Свойства

| Имя свойства  | Тип    | Описание
|:---------------|:--------|:--------------------------------------------------
| shouldPrefixNameToFile | Boolean  | Добавьте имя набора документов в каждое имя файла.
| allowedContentTypes | Collection (microsoft.graph.contentTypeInfo) | Типы контента разрешены в наборе документов.
| defaultContents     | Collection (microsoft.graph.documentSetContent) | Содержимое набора документов по умолчанию.  
| propagateWelcomePageChanges | Boolean | Указывает, следует ли нажимать изменения приветствия страниц на унаследованные типы контента.  
| sharedColumns       | Коллекция (microsoft.graph.columnDefinition) | Столбцы, отредактированы в наборе документов, которые синхронизируются со всеми документами в наборе. Эти данные можно прочитать только в самих документах. 
| welcomePageColumns  | Коллекция (microsoft.graph.columnDefinition)  | Указывает столбцы, которые будут показываться на странице приветствия для набора документов.  
| welcomePageUrl      | string | Url-адрес страницы welcome.  

## <a name="json-representation"></a>Представление JSON

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
