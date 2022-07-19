---
title: Тип ресурса siteSource
description: Контейнер для сайта, связанного с хранителями.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 00951a56f9ab3f98271b9ecde38b8a844e21919e
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2022
ms.locfileid: "66839878"
---
# <a name="sitesource-resource-type"></a>Тип ресурса siteSource

Пространство имен: microsoft.graph.security


Контейнер для сайта, связанного с хранителями.

Наследуется [от dataSource](../resources/security-datasource.md).


## <a name="methods"></a>Методы
Нет.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|Пользователь, создавший **siteSource**.|
|createdDateTime|DateTimeOffset|Дата и время создания **siteSource** .|
|displayName|Строка|Отображаемое имя **siteSource**. Это будет имя сайта SharePoint.|
|id|Строка| Идентификатор **siteSource**. |
|holdStatus|microsoft.graph.security.dataSourceHoldStatus|Состояние удержания **ресурса siteSource**. Допустимые значения: `notApplied`, `applied`, `applying`, `removing`, `partial`.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|site|[site](../resources/site.md)|Сайт SharePoint, связанный с **siteSource**.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.siteSource",
  "baseType": "microsoft.graph.security.dataSource",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.siteSource",
  "id": "String (identifier)",
  "displayName": "String",
  "holdStatus": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```

