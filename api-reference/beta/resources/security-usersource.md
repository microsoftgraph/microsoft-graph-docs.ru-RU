---
title: Тип ресурса userSource
description: Контейнер для почтового ящика пользователя и OneDrive для бизнеса сайта.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: b36d9cc2947c263510c8b08d05f210a556985690
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2022
ms.locfileid: "66838180"
---
# <a name="usersource-resource-type"></a>Тип ресурса userSource

Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Контейнер для почтового ящика пользователя и OneDrive для бизнеса сайта.

Наследуется [от dataSource](../resources/security-datasource.md).

## <a name="methods"></a>Методы
Нет. 
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|Пользователь, создавший **userSource**.|
|createdDateTime|DateTimeOffset|Дата и время **создания объекта userSource** .|
|displayName|Строка|Отображаемое имя, связанное с почтовым ящиком и сайтом.|
|email|String|Email адрес почтового ящика пользователя.|
|id|String|Идентификатор **объекта userSource**. Это не идентификатор фактической группы.|
|includedSources|microsoft.graph.security.sourceType|Указывает источники, включенные в эту группу. Возможные значения: `mailbox`, `site`.|
|siteWebUrl|String|URL-адрес веб-сайта OneDrive для бизнеса пользователя. Только для чтения.|
|holdStatus|microsoft.graph.security.dataSourceHoldStatus|Состояние удержания **объекта userSource**. Допустимые значения: `notApplied`, `applied`, `applying`, `removing`, `partial`.|


### <a name="usersourceholdstatus-values"></a>Значения userSourceHoldStatus

|Имя|Описание|
|:----|-----------|
|notApplied|UserSource не находится на удержании (все источники в нем не находятся на удержании).|
|Применяется|UserSource находится на удержании (все источники находятся на удержании).|
|Применение|UserSource находится в состоянии применения удержания (активируется операция applyHold).|
|Удаление|UserSource удаляет состояние удержания (активируется операция removeHold).|
|Частичное|UserSource находится в смешанном состоянии, где некоторые источники находятся на удержании, а некоторые не находятся в состоянии удержания или ошибки.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.userSource",
  "baseType": "microsoft.graph.security.dataSource",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.userSource",
  "id": "String (identifier)",
  "displayName": "String",
  "holdStatus": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "email": "String",
  "includedSources": "String",
  "siteWebUrl": "String"
}
```