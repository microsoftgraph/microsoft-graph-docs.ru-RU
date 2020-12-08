---
title: Тип ресурса Усерсаурце
description: Контейнер для почтового ящика хранитель и сайта OneDrive для бизнеса.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 2ce5448947bded580cc4896ba549d7cc6fab95f9
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597742"
---
# <a name="usersource-resource-type"></a>Тип ресурса Усерсаурце

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Контейнер для почтового ящика [хранитель](custodian.md) и сайта OneDrive для бизнеса.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список Усерсаурцес](../api/custodian-list-usersources.md)|Коллекция [усерсаурце](../resources/usersource.md)|Получение списка объектов **усерсаурце** и их свойств.|
|[Создание Усерсаурце](../api/custodian-post-usersources.md)|[усерсаурце](../resources/usersource.md)|Создание нового объекта **усерсаурце** .|
|[Получение Усерсаурце](../api/usersource-get.md)|[усерсаурце](../resources/usersource.md)|Чтение свойств и связей объекта **усерсаурце** .|
|[Удаление Усерсаурце](../api/usersource-delete.md)|Нет|Удаление объекта **усерсаурце** .|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|Пользователь, создавший **усерсаурце**.|
|createdDateTime|DateTimeOffset|Дата и время создания ерсаурце **усерсаурце** для США|
|displayName|String|Отображаемое имя, связанное с почтовым ящиком и сайтом.|
|email|String|Адрес электронной почты почтового ящика пользователя.|
|id|String|Идентификатор **усерсаурце**. Это значение не является ИДЕНТИФИКАТОРом фактической группы|
|инклудедсаурцес|sourceType|Указывает, какие источники включены в эту группу. Возможные значения: `mailbox`, `site`.|

### <a name="sourcetype-values"></a>значения sourceType

Типы источника, связанные с пользователем. Включает почтовый ящик и сайт по умолчанию.

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
