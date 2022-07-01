---
title: Тип ресурса retentionEventType
description: Представляет одну группу для одного типа событий хранения. Тип события — это универсальный декрипции для аналогичных событий, которые можно использовать с любой меткой с хранением на основе событий.
author: sseth
ms.localizationpriority: medium
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 38b9ee622663d249c5f6c117b376767eb29ae232
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447809"
---
# <a name="retentioneventtype-resource-type"></a>Тип ресурса retentionEventType

Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет одну группу для одного типа событий хранения.

При создании [события хранения](../resources/security-retentionevent.md) оно связано с определенным типом события, который, в свою очередь, связан с [меткой хранения](../resources/security-retentionlabel.md). В течение указанного периода хранения будет храниться только содержимое с примененной меткой хранения.
Дополнительные сведения см. [в разделе "Начало хранения при возникновении события"](/microsoft-365/compliance/event-driven-retention).


## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление retentionEventTypes](../api/security-retentioneventtype-list.md)|[Коллекция microsoft.graph.security.retentionEventType](../resources/security-retentioneventtype.md)|Получение списка объектов [retentionEventType](../resources/security-retentioneventtype.md) и их свойств.|
|[Создание retentionEventType](../api/security-retentioneventtype-post.md)|[microsoft.graph.security.retentionEventType](../resources/security-retentioneventtype.md)|Создайте объект [retentionEventType](../resources/security-retentioneventtype.md) .|
|[Получение retentionEventType](../api/security-retentioneventtype-get.md)|[microsoft.graph.security.retentionEventType](../resources/security-retentioneventtype.md)|Чтение свойств и связей объекта [retentionEventType](../resources/security-retentioneventtype.md) .|
|[Обновление retentionEventType](../api/security-retentioneventtype-update.md)|[microsoft.graph.security.retentionEventType](../resources/security-retentioneventtype.md)|Обновление свойств объекта [retentionEventType](../resources/security-retentioneventtype.md) .|
|[Удаление retentionEventType](../api/security-retentioneventtype-delete.md)|Нет|Удаление объекта [retentionEventType](../resources/security-retentioneventtype.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|createdBy|[Microsoft.graph.identitySet](/graph/api/resources/identityset)|Пользователь, создавший retentionEventType.|
|createdDateTime|DateTimeOffset|Дата создания retentionEventType.|
|description|String|Необязательные сведения о типе события.|
|displayName|String|Имя типа события.|
|id|String|Представляет уникальный идентификатор пользователя, создавшего retentionEventType. [entity](/graph/api/resources/entity).|
|lastModifiedBy|[Microsoft.graph.identitySet](/graph/api/resources/identityset)|Пользователь, который последним изменил retentionEventType.|
|lastModifiedDateTime|DateTimeOffset|Дата последнего изменения параметра retentionEventType.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.retentionEventType",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.retentionEventType",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)"
}
```

