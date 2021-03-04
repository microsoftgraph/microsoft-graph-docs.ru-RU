---
title: Тип ресурса userSource
description: Контейнер для почтового ящика хранителя и сайта OneDrive для бизнеса.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: f0d98ac894d3d60bed2bb249ef9daec707f6f7ba
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447538"
---
# <a name="usersource-resource-type"></a>Тип ресурса userSource

Пространство имен: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Контейнер для [почтового ящика хранителя](ediscovery-custodian.md) и сайта OneDrive для бизнеса.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список userSources](../api/ediscovery-custodian-list-usersources.md)|[коллекция microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md)|Получите список объектов **userSource** и их свойств.|
|[Создание userSource](../api/ediscovery-custodian-post-usersources.md)|[microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md)|Создание нового **объекта userSource.**|
|[Get userSource](../api/ediscovery-usersource-get.md)|[microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md)|Ознакомьтесь с свойствами и отношениями **объекта userSource.**|
|[Удаление userSource](../api/ediscovery-usersource-delete.md)|Нет|Удаление **объекта userSource.**|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|Пользователь, создавший **userSource**.|
|createdDateTime|DateTimeOffset|Дата и время создания **userSource**|
|displayName|String|Имя отображения, связанное с почтовым ящиком и сайтом.|
|email|String|Адрес электронной почты почтового ящика пользователя.|
|id|String|ID **пользователяSource**. Это не ID фактической группы|
|includedSources|microsoft.graph.ediscovery.sourceType|Указывает, какие источники включены в эту группу. Возможные значения: `mailbox`, `site`.|

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
  "@odata.type": "microsoft.graph.ediscovery.userSource",
  "baseType": "microsoft.graph.ediscovery.dataSource",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.userSource",
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
