---
author: swapnil1993
title: Тип ресурса documentSet
description: Содержит метаданные о параметрах набора документов.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: b64f5b0f12a41a0386818c68ba644d92bfa60603
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/30/2021
ms.locfileid: "58696708"
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
