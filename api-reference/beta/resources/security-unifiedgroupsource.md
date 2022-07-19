---
title: Тип ресурса unifiedGroupSource
description: Контейнер для группы хранителей.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: a6b8b05c3f57e4903b66aa7de95e8b4d94849d71
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2022
ms.locfileid: "66837809"
---
# <a name="unifiedgroupsource-resource-type"></a>Тип ресурса unifiedGroupSource

Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Контейнер для группы хранителей.

Наследуется [от dataSource](../resources/security-datasource.md).

## <a name="methods"></a>Методы
Нет.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|Пользователь, создавший **unifiedGroupSource**.|
|createdDateTime|DateTimeOffset|Дата и время создания **unifiedGroupSource** .|
|displayName|Строка|Отображаемое имя объединенной группы, которое является именем группы.|
|id|Строка|Идентификатор **unifiedGroupSource**. Это не идентификатор фактической группы.|
|includedSources|microsoft.graph.security.sourceType|Указывает источники, включенные в эту группу. Возможные значения: `mailbox`, `site`.|
|holdStatus|microsoft.graph.security.dataSourceHoldStatus|Состояние удержания **объекта unifiedGroupSource**. Допустимые значения: `notApplied`, `applied`, `applying`, `removing`, `partial`.|

### <a name="sourcetype-values"></a>Значения sourceType
|Member|Описание|
|:----|-----------|
| mailbox | Представляет почтовый ящик.|
| site | Представляет сайт SharePoint.|


## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|group|[group](../resources/group.md)|Представляет группу.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.unifiedGroupSource",
  "baseType": "microsoft.graph.security.dataSource",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.unifiedGroupSource",
  "id": "String (identifier)",
  "displayName": "String",
  "holdStatus": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "includedSources": "String"
}
```

