---
title: тип ресурса legalHold
description: тип ресурса legalHold
ms.localizationpriority: medium
author: mahage-msft
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 6de7272e31476a925f4e9e08f680e41b7b8fed14
ms.sourcegitcommit: 33e0bbada1b47310a18d8f794914b1319d88e6f4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2021
ms.locfileid: "61402876"
---
# <a name="legalhold-resource-type"></a>тип ресурса legalHold

Пространство имен: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет юридическое удержание. Юридические точки удерживают, привязанные к делу об обнаружении электронных обнаружений. Юридические удержания не следует путать с удержанием, которые используются для управления политиками хранения Microsoft 365 контента. Юридические точки электронного разыскного расследования являются для удержания контента на неопределенный срок для судебного разбирательства, внутренних расследований и других юридических действий, в которых контент должен быть защищен от удаления. Дополнительные сведения см. в [Advanced eDiscovery](/microsoft-365/compliance/managing-holds)

Наследует от [объекта](../resources/entity.md).

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список legalHolds](../api/ediscovery-case-list-legalholds.md)|[коллекция microsoft.graph.ediscovery.legalHold](../resources/ediscovery-legalhold.md)|Получите список объектов  **legalHold** и их свойств.|
|[Создание legalHold](../api/ediscovery-case-post-legalholds.md)|[microsoft.graph.ediscovery.legalHold](../resources/ediscovery-legalhold.md)|Создание нового **объекта legalHold.**|
|[Get legalHold](../api/ediscovery-legalhold-get.md)|[microsoft.graph.ediscovery.legalHold](../resources/ediscovery-legalhold.md)|Ознакомьтесь с свойствами и отношениями объекта **legalHold.**|
|[Обновление legalHold](../api/ediscovery-legalhold-update.md)|[microsoft.graph.ediscovery.legalHold](../resources/ediscovery-legalhold.md)|Обновление свойств объекта **legalHold.**|
|[Удаление legalHold](../api/ediscovery-legalhold-delete.md)|Нет|Удаление **объекта legalHold.**|
|[List siteSources](../api/ediscovery-legalhold-list-sitesources.md)|[коллекция microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md)|Получите список объектов [siteSource,](../resources/ediscovery-sitesource.md) связанных с юридическим удержанием.|
|[Создание siteSource](../api/ediscovery-legalhold-post-sitesources.md)|[microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md)|Создание нового объекта siteSource.|
|[Список userSources](../api/ediscovery-legalhold-list-usersources.md)|[коллекция microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md)|Получите список [объектов userSource,](../resources/ediscovery-usersource.md) связанных с юридическим удержанием.|
|[Создание userSource](../api/ediscovery-legalhold-post-usersources.md)|[microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md)|Создание нового **объекта userSource.**|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|contentQuery|String|Запрос KQL, который указывает содержимое, которое должно быть в указанных расположениях. Дополнительные материалы см. в статье [Ключевые запросы и условия поиска для поиска контента и поиска по электронной информации.](/microsoft-365/compliance/keyword-queries-and-search-conditions)  Чтобы удерживать все содержимое в указанных расположениях, оставьте **contentQuery пустым.** |
|createdBy|[identitySet](../resources/identityset.md)|Пользователь, создавший юридическое удержание. |
|createdDateTime|DateTimeOffset|Дата и время создания юридического удержания. |
|description|String| Описание юридического удержания. |
|displayName|String| Отображение имени юридического удержания. |
|ошибки|Коллекция строк|Перечислены все ошибки, которые произошли при размещении удержания. |
|id|String|ID для дела об обнаружении электронной почты. Только для чтения. Наследуется от [сущности](../resources/entity.md). |
|isEnabled|Boolean|Указывает, включено ли удержание и активно ли оно поддерживается. |
|lastModifiedBy|[identitySet](../resources/identityset.md)|пользователя, который в последний раз изменил юридическое удержание.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения юридического удержания. |
|status|microsoft.graph.ediscovery.legalHoldStatus|Состояние юридического удержания. Возможные значения: `Pending`, `Error`, `Success`, `UnknownFutureValue`.|

### <a name="legalholdstatus-values"></a>значения legalHoldStatus

|Member|Описание|
|:---|-----------|
|Pending| Продолжается процесс распределения удержания. |
|Ошибка| При применении удержания была допущена ошибка. Подробные сведения см. в свойстве ошибок объекта legalHold. |
|Успешно| Удержание было успешно применено и удерживает указанное содержимое. |

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|siteSources|[коллекция microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md)|Объект источника данных для SharePoint сайтов, связанных с юридическим удержанием. |
|userSources|[коллекция microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md)| Объект источника данных для юридического удержания. Это контейнер для почтового ящика и OneDrive для бизнеса сайта.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.legalHold",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.legalHold",
  "id": "String (identifier)",
  "description": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "isEnabled": "Boolean",
  "status": "String",
  "contentQuery": "String",
  "errors": [
    "String"
  ],
  "displayName": "String",
  "createdDateTime": "String (timestamp)"
}
```
