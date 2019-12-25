---
title: Тип ресурса addIn
description: Ниже представлено описание ресурса в формате JSON.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 3671ad561fde44aac90d20284c7acbfedba6b0c3
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40863937"
---
# <a name="addin-resource-type"></a>Тип ресурса addIn

Определяет пользовательское поведение, которое служба может использовать для вызова приложения в определенных контекстах. Например, приложения, которые могут визуализировать файловые потоки, [могут настраивать надстройки](/onedrive/developer/file-handlers/?view=odsp-graph-online) для своей функции "филехандлер". Это позволит таким службам, как Office 365, вызывать приложение в контексте документов, над которыми работает пользователь.

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
