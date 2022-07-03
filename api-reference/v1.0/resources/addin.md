---
title: Тип ресурса addIn
description: Ниже показано представление ресурса в формате JSON.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 3547cdf43bc359e62bb4f1f60a2ffc142f727c9b
ms.sourcegitcommit: 6a4e81d2b8e7447771c9060998c7e1cc18a57902
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/03/2022
ms.locfileid: "66609747"
---
# <a name="addin-resource-type"></a>Тип ресурса addIn

Пространство имен: microsoft.graph

Определяет пользовательское поведение, которое служба может использовать для вызова приложения в определенных контекстах. Например, приложения, которые могут отображать потоки файлов, могут настроить [addIns](/onedrive/developer/file-handlers/) для функции FileHandler. Это позволит таким службам, как Microsoft 365, вызывать приложение в контексте документов, над которыми работает пользователь.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|guid||
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
  "id": "Guid",
  "properties": [{"@odata.type": "microsoft.graph.keyValue"}],
  "type": "String"
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

