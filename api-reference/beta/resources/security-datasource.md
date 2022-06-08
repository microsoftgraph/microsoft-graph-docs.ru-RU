---
title: Тип ресурса dataSource
description: Сущность dataSource — это абстрактный базовый класс, используемый для определения источников содержимого для обнаружения электронных данных.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: d95cdd3dd8f66c2c4de67c8c469281989e839f93
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/08/2022
ms.locfileid: "65946132"
---
# <a name="datasource-resource-type"></a>Тип ресурса dataSource

Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сущность dataSource — это абстрактный базовый класс, используемый для определения источников содержимого для обнаружения электронных данных.

## <a name="methods"></a>Методы

Нет.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|Пользователь, создавший **источник данных**.|
|createdDateTime|DateTimeOffset|Дата и время **создания источника** данных.|
|displayName|Строка|Отображаемое имя **источника данных**. Это будет имя сайта SharePoint.|
|id|Строка| Идентификатор источника **данных**. Это не идентификатор фактического сайта.|
|holdStatus|Строка|Состояние удержания **источника данных**. Возможные значения: `notApplied`, , `applied`, `applying`, `removing``partial`|
## <a name="relationships"></a>Отношения
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.dataSource",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.dataSource",
  "id": "String (identifier)",
  "displayName": "String",
  "holdStatus": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```

