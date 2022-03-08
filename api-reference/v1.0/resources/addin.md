---
title: тип ресурса addIn
description: Ниже представлено описание ресурса в формате JSON.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 138fdd62e448c3a525ed9eaa6afe7c734cdd5404
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337175"
---
# <a name="addin-resource-type"></a>тип ресурса addIn

Пространство имен: microsoft.graph

Определяет пользовательское поведение, которое служба может использовать для вызова приложения в определенных контекстах. Например, приложения, которые могут отрисовки файлового потока, могут настраивать [addIns](/onedrive/developer/file-handlers/?view=odsp-graph-online) для функции FileHandler. Это позволит таким службам, как Microsoft 365, вызывать приложение в контексте документов, над которыми работает пользователь.

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

