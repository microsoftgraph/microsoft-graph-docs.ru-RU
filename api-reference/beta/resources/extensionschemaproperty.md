---
title: Тип ресурса extensionSchemaProperty
description: Ресурс **extensionSchemaProperty** используется для задания имени и типа свойства в качестве части определения schemaExtension.
localization_priority: Normal
ms.openlocfilehash: 05fb5eb94f760bce26ba09bf3e8e862ff5fd2fb8
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340275"
---
# <a name="extensionschemaproperty-resource-type"></a>Тип ресурса extensionSchemaProperty

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **extensionSchemaProperty** используется для задания имени и типа свойства в качестве части определения [schemaExtension](schemaextension.md).


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|name|Строка| Имя строго типизированного свойства, определенного как часть расширения схемы.|
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
