---
title: "siteSource resource type" description: ""The container for a site associated with a custodian".
author: "SeunginLyu" ms.localizationpriority: medium ms.prod: "ediscovery" doc_type: resourcePageType
---

# <a name="sitesource-resource-type"></a>Тип ресурса siteSource

Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
Контейнер для сайта, связанного с хранителями.

IInherits из [dataSource](../resources/security-datasource.md).


## <a name="methods"></a>Методы
Нет.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|Пользователь, создавший **siteSource**.|
|createdDateTime|DateTimeOffset|Дата и время создания **siteSource** .|
|displayName|Строка|Отображаемое имя **siteSource**. Это будет имя сайта SharePoint.|
|id|String| Идентификатор **siteSource**. Источник сайта можно получить в любое время с помощью [get site](../api/site-get.md) - https://graph.microsoft.com/v1.0/sites/{siteId}|
|holdStatus|Строка|Состояние удержания **ресурса siteSource**. Возможные значения: `notApplied`, , `applied`, `applying`, `removing``partial`|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|site|[site](../resources/site.md)|Сайт SharePoint, связанный с **siteSource**.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.siteSource",
  "baseType": "microsoft.graph.ediscovery.dataSource",
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

