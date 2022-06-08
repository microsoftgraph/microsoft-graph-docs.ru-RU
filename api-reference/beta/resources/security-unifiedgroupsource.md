---
title: Тип ресурса unifiedGroupSource
description: Контейнер для группы хранителей.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 3e544a4b6d00bb59b5879fc13376fd94a5bba169
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/08/2022
ms.locfileid: "65946055"
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
|displayName|Строка|Отображаемое имя объединенной группы — это имя группы.|
|id|String|Идентификатор **unifiedGroupSource**. Это не идентификатор фактической группы.|
|includedSources|Строка|Указывает источники, включенные в эту группу. Возможные значения: `mailbox`, `site`.|
|holdStatus|Строка|Состояние удержания **объекта unifiedGroupSource**. Возможные значения: `notApplied`, , `applied`, `applying`, `removing``partial`|

## <a name="relationships"></a>Отношения
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

