---
title: Тип ресурса Информатионпротектионконтентлабел
description: Описывает объект Информатионпротектионконтентлабел, определяющий метаданные МИП для объекта.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8422f83db0c94eed74d5690343c51b70e2d87d82
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016452"
---
# <a name="informationprotectioncontentlabel-resource-type"></a>Тип ресурса Информатионпротектионконтентлабел

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает объект Информатионпротектионконтентлабел, определяющий метаданные МИП для объекта. **информатионпротектионконтентлабел** возвращается с помощью API [екстрактлабел](../api/informationprotectionlabel-extractLabel.md) , который разрешается в метку, которая в данный момент применена к файлу. 

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|assignmentMethod|String| Возможные значения: `standard`, `privileged`, `auto`.|
|креатиондатетиме|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|label|[лабелдетаилс](labeldetails.md)| Сведения о метке, которая в настоящее время применяется к файлу. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.informationProtectionContentLabel",
  "baseType": null
}-->

```json
{
  "assignmentMethod": "String",
  "creationDateTime": "String (timestamp)",
  "label": {"@odata.type": "microsoft.graph.labelDetails"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "informationProtectionContentLabel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

