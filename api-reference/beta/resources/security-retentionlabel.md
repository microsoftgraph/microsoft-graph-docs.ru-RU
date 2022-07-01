---
title: Тип ресурса retentionLabel
description: Представляет, как клиенты могут управлять своими данными, независимо от того, как долго они сохраняются или удаляются.
author: sseth
ms.localizationpriority: medium
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 8e74f494b56c2a622510648953f1a021a32140c7
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447779"
---
# <a name="retentionlabel-resource-type"></a>Тип ресурса retentionLabel

Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет, как клиенты могут управлять своими данными, в том числе о том, следует ли хранить или удалять их в течение длительного времени.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление меток retentionLabel](../api/security-retentionlabel-list.md)|[Коллекция microsoft.graph.security.retentionLabel](../resources/security-retentionlabel.md)|Получение списка объектов [retentionLabel](../resources/security-retentionlabel.md) и их свойств.|
|[Создание retentionLabel](../api/security-retentionlabel-post.md)|[microsoft.graph.security.retentionLabel](../resources/security-retentionlabel.md)|Создайте объект [retentionLabel](../resources/security-retentionlabel.md) .|
|[Получение retentionLabel](../api/security-retentionlabel-get.md)|[microsoft.graph.security.retentionLabel](../resources/security-retentionlabel.md)|Чтение свойств и связей объекта [retentionLabel](../resources/security-retentionlabel.md) .|
|[Обновление retentionLabel](../api/security-retentionlabel-update.md)|[microsoft.graph.security.retentionLabel](../resources/security-retentionlabel.md)|Обновление свойств объекта [retentionLabel](../resources/security-retentionlabel.md) .|
|[Удаление retentionLabel](../api/security-retentionlabel-delete.md)|Нет|Удаление объекта [retentionLabel](../resources/security-retentionlabel.md) .|
|[List retentionEventType](../api/security-retentioneventtype-list.md)|[Коллекция microsoft.graph.security.retentionEventType](../resources/security-retentioneventtype.md)|Получение ресурсов retentionEventType из свойства навигации exapnd eventType.|
|[Добавление retentionEventType](../api/security-retentioneventtype-post.md)|[microsoft.graph.security.retentionEventType](../resources/security-retentioneventtype.md)|Добавьте eventType, добавив соответствующее свойство odata при создании метки.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|actionAfterRetentionPeriod|microsoft.graph.security.actionAfterRetentionPeriod| Указывает действие, выполняемые с документом с этой меткой, примененной в течение периода хранения. Допустимые значения: `none`, `delete`, `startDispositionReview`, `unknownFutureValue`.|
|behaviorDuringRetentionPeriod|microsoft.graph.security.behaviorDuringRetentionPeriod|Указывает, как должен выглядеть документ с этой меткой в течение периода хранения. Допустимые значения: `doNotRetain`, `retain`, `retainAsRecord`, `retainAsRegulatoryRecord`, `unknownFutureValue`.|
|createdBy|[Microsoft.graph.identitySet](/graph/api/resources/identityset)|Представляет пользователя, создавшего метку retentionLabel.|
|createdDateTime|DateTimeOffset|Представляет дату и время создания метки хранения.|
|descriptionForAdmins|String|Предоставляет сведения о метках для администратора. Необязательно.|
|descriptionForUsers|String|Предоставляет сведения о метке для пользователя. Необязательное свойство.|
|displayName|String|Уникальная строка, определяющее имя метки.|
|dispositionReviewStages|[Коллекция microsoft.graph.security.dispositionReviewStage](../resources/security-dispositionreviewstage.md)|Просмотрите этапы, на которых рецензенты получают уведомления, чтобы определить, должен ли документ быть удален или сохранен.|
|id|String|Уникальный идентификатор метки хранения. [entity](/graph/api/resources/entity).|
|isInUse|Логическое|Указывает, используется ли метка в данный момент.|
|lastModifiedBy|[Microsoft.graph.identitySet](/graph/api/resources/identityset)|Пользователь, который последним изменил метку retentionLabel.|
|lastModifiedDateTime|DateTimeOffset|Дата последнего изменения метки хранения.|
|retentionDuration|[microsoft.graph.security.retentionDuration](../resources/security-retentionduration.md)|Указывает количество дней для сохранения содержимого.|
|retentionTrigger|microsoft.graph.security.retentionTrigger|Указывает, рассчитывается ли длительность хранения на основе даты создания содержимого, помеченной даты или даты последнего изменения. Допустимые значения: `dateLabeled`, `dateCreated`, `dateModified`, `dateOfEvent`, `unknownFutureValue`.|
|defaultRecordBehavior|microsoft.graph.security.defaultRecordBehavior|Указывает состояние блокировки или разблокировки метки записи при ее создании. Возможные значения: `startLocked`, , `startUnlocked``unknownFutureValue`.|
|labelToBeApplied|String|Указывает метку замены, которая будет применена автоматически по истечении срока хранения текущей метки. |


## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|dispositionReviewStages|[Коллекция microsoft.graph.security.dispositionReviewStage](../resources/security-dispositionreviewstage.md)|Если действие в конце срока хранения выбрано как dispositionReview, dispositionReviewStages задает последовательный набор этапов по крайней мере с одним рецензентом на каждом этапе.|
|eventType|[microsoft.graph.security.retentionEventType](../resources/security-retentioneventtype.md)|Представляет тип, связанный с событием хранения.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.retentionLabel",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.retentionLabel",
  "id": "String (identifier)",
  "displayName": "String",
  "behaviorDuringRetentionPeriod": "String",
  "actionAfterRetentionPeriod": "String",
  "retentionTrigger": "String",
  "retentionDuration": {
    "@odata.type": "microsoft.graph.security.retentionDuration"
  },
  "isInUse": "Boolean",
  "descriptionForAdmins": "String",
  "descriptionForUsers": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "labelToBeApplied": "String",
  "defaultRecordBehavior": "String"
}
```
