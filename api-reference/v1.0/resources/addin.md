---
title: Тип ресурса addIn
description: Ниже представлено описание ресурса в формате JSON.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: ad65d0a9a3bed59bcb630082807004a7ca89ba5f
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938999"
---
# <a name="addin-resource-type"></a>Тип ресурса addIn

Определяет пользовательское поведение, которое может использоваться службой использования для вызова приложения в определенных контекстах. Например, приложения, которые могут визуализировать файловые потоки, [могут настраивать надстройки](https://docs.microsoft.com/en-us/onedrive/developer/file-handlers/?view=odsp-graph-online) для своей функции "филехандлер". Это позволит таким службам, как Office 365, вызвать приложение в контексте документа, над которым работает пользователь.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|кодом||
|properties|Коллекция [keyValue](keyvalue.md)||
|type|string||

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.addIn"
}-->

```json
{
  "id": "guid",
  "properties": [{"@odata.type": "microsoft.graph.keyValue"}],
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "addIn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
