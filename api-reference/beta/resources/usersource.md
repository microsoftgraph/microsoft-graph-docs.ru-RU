---
title: Тип ресурса userSource
description: Контейнер для почтового ящика хранителя и сайта OneDrive для бизнеса.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 10184e053a0c62aaba6599f7d6f9bb6a33de8828
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706042"
---
# <a name="usersource-resource-type"></a>Тип ресурса userSource

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Контейнер для почтового [ящика хранителя](custodian.md) и сайта OneDrive для бизнеса.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список userSources](../api/custodian-list-usersources.md)|[Коллекция userSource](../resources/usersource.md)|Получите список объектов **userSource** и их свойств.|
|[Создание userSource](../api/custodian-post-usersources.md)|[userSource](../resources/usersource.md)|Создание объекта **userSource.**|
|[Get userSource](../api/usersource-get.md)|[userSource](../resources/usersource.md)|Чтение свойств и связей объекта **userSource.**|
|[Удаление userSource](../api/usersource-delete.md)|Нет|Удаление объекта **userSource.**|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|Пользователь, создавший **userSource.**|
|createdDateTime|DateTimeOffset|Дата и время создания **userSource**|
|displayName|String|Отображаемая фамилия, связанная с почтовым ящиком и сайтом.|
|email|String|Адрес электронной почты почтового ящика пользователя.|
|id|String|ИД **userSource.** Это не ИД фактической группы|
|includedSources|sourceType|Указывает источники, включенные в эту группу. Возможные значения: `mailbox`, `site`.|

### <a name="sourcetype-values"></a>значения sourceType

Типы источников, связанных с пользователем. Включает почтовый ящик и сайт по умолчанию.

|Member|Описание|
|:----|-----------|
|mailbox|Представляет почтовый ящик.|
|site|Представляет сайт OneDrive для бизнеса.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userSource",
  "baseType": "microsoft.graph.dataSource",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.userSource",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "id": "String (identifier)",
  "email": "String",
  "includedSources": "String"
}
```
