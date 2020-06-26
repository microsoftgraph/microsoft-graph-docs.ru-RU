---
title: Тип ресурса addIn
description: Ниже представлено описание ресурса в формате JSON.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 1700f3c6bec06c9f2e7ec6093fccffab443d2b08
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895974"
---
# <a name="addin-resource-type"></a>Тип ресурса addIn

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определяет пользовательское поведение, которое служба может использовать для вызова приложения в определенных контекстах. Например, приложения, которые могут визуализировать файловые потоки, [могут настраивать](https://docs.microsoft.com/onedrive/developer/file-handlers/?view=odsp-graph-online) надстройки для работы с обработчиками файлов. Это позволит таким службам, как Microsoft 365, вызывать приложение в контексте документа, над которым работает пользователь.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|кодом||
|properties|Коллекция [keyValue](keyvalue.md)||
|type|string||

## <a name="json-representation"></a>Представление в формате JSON

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
