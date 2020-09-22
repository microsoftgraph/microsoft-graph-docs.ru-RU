---
title: Тип ресурса extensionSchemaProperty
description: Ресурс **extensionSchemaProperty** используется для задания имени и типа свойства в качестве части определения schemaExtension.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: keylimesoda
ms.openlocfilehash: c0bb3a423983b70066e2451a5029f4eaf2acaebd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026945"
---
# <a name="extensionschemaproperty-resource-type"></a>Тип ресурса extensionSchemaProperty

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **extensionSchemaProperty** используется для задания имени и типа свойства в качестве части определения [schemaExtension](schemaextension.md).


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|name|String| Имя строго типизированного свойства, определенного как часть расширения схемы.|
|type|String| Тип свойства, определенного в качестве части расширения схемы.  Разрешенные значения: *Binary, Boolean, DateTime, Integer* или *String*.  Дополнительные сведения см. в приведенной ниже таблице.|

#### <a name="supported-property-data-types"></a>Поддерживаемые типы данных свойств 
При определении свойства в расширении схемы поддерживаются следующие типы данных:

| Тип свойства | Примечания |
|-------------|------------|
| Binary | Не более 256 байт. |
| Boolean | Не поддерживается для ресурсов message, event и post. |
| DateTime | Должен быть указан в формате ISO 8601. Данные времени будут храниться в формате UTC. |
| Целое число | 32-разрядное значение. Не поддерживается для ресурсов message, event и post. |
| String | Не более 256 символов |

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.extensionSchemaProperty"
}-->

```json
{
  "name": "String",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "extensionSchemaProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


