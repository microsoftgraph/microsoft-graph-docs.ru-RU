---
title: Тип ресурса userSource
description: Контейнер для почтового ящика пользователя и сайта OneDrive для бизнеса.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 45bd3444baa6b3e0aa7c13f6678fd9c2312915b5
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/08/2022
ms.locfileid: "65946052"
---
# <a name="usersource-resource-type"></a>Тип ресурса userSource

Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Контейнер для почтового ящика пользователя и сайта OneDrive для бизнеса.

Наследуется [от dataSource](../resources/security-datasource.md).

## <a name="methods"></a>Методы
Нет. 
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|Пользователь, создавший **userSource**.|
|createdDateTime|DateTimeOffset|Дата и время создания **userSource**|
|displayName|Строка|Отображаемое имя, связанное с почтовым ящиком и сайтом.|
|email|String|Адрес электронной почты почтового ящика пользователя.|
|id|String|Идентификатор **объекта userSource**. Это не идентификатор фактической группы.|
|includedSources|Строка|Указывает источники, включенные в эту группу. Возможные значения: `mailbox`, `site`.|
|siteWebUrl|Строка|URL-адрес сайта OneDrive для бизнеса пользователя. Только для чтения.|
|holdStatus|Строка|Состояние удержания **объекта userSource**. Возможные значения: `notApplied`, , `applied`, `applying`, `removing``partial`|
### <a name="sourcetype-values"></a>Значения sourceType

Типы источников, связанных с пользователем. Включает почтовый ящик и сайт по умолчанию.

|Member|Описание|
|:----|-----------|
|mailbox|Представляет почтовый ящик.|
|site|Представляет сайт OneDrive для бизнеса.|

### <a name="usersourceholdstatus-values"></a>Значения userSourceHoldStatus

|Имя|Описание|
|:----|-----------|
|notApplied|UserSource не находится на удержании (все источники в нем не находятся на удержании).|
|Применяется|UserSource находится на удержании (все источники находятся на удержании).|
|Применение|UserSource находится в состоянии применения удержания (активируется операция applyHold).|
|Удаление|UserSource удаляет состояние удержания (активируется операция removeHold).|
|Частичное|UserSource находится в смешанном состоянии, где некоторые источники находятся на удержании, а некоторые не находятся в состоянии удержания или ошибки.|

## <a name="relationships"></a>Отношения
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
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