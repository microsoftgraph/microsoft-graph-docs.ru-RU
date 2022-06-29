---
title: Обновление retentionLabel
description: Обновление свойств объекта retentionLabel.
author: sseth
ms.localizationpriority: medium
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 717457b49b98074e72cffe4cec5b8fe5b36f54db
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447787"
---
# <a name="update-retentionlabel"></a>Обновление retentionLabel
Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [retentionLabel](../resources/security-retentionlabel.md) .

Чтобы обновить этап [проверки](../resources/security-dispositionreviewstage.md) перед ликвидацией, включите свойство **actionAfterRetentionPeriod** в текст запроса, указав одно из возможных значений.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|RecordsManagement.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|RecordsManagement.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /security/labels/retentionLabels/{retentionLabelId}

```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]


|Свойство|Тип|Описание|
|:---|:---|:---|
|actionAfterRetentionPeriod|microsoft.graph.security.actionAfterRetentionPeriod| Указывает действие, которое будет применено к документу с этой меткой по истечении срока хранения. Допустимые значения: `none`, `delete`, `startDispositionReview`, `unknownFutureValue`.|
|behaviorDuringRetentionPeriod|microsoft.graph.security.behaviorDuringRetentionPeriod|Указывает, как должен выглядеть документ с этой меткой в течение периода хранения. Допустимые значения: `doNotRetain`, `retain`, `retainAsRecord`, `retainAsRegulatoryRecord`, `unknownFutureValue`.|
|createdBy|[Microsoft.graph.identitySet](/graph/api/resources/identityset)|Представляет пользователя, создавшего метку retentionLabel.|
|createdDateTime|DateTimeOffset|Представляет дату и время создания метки хранения.|
|descriptionForAdmins|String|Это необязательное свойство, которое предоставляет сведения о метке для администратора.|
|descriptionForUsers|String|Это необязательное свойство, которое предоставляет сведения о метке для пользователя.|
|displayName|String|Уникальная строка, определяющее имя метки.|
|dispositionReviewStages|[Коллекция microsoft.graph.security.dispositionReviewStage](../resources/security-dispositionreviewstage.md)|Просмотрите этапы, на которых рецензенты получают уведомления, чтобы определить, должен ли документ быть удален или сохранен.|
|id|String|Уникальный идентификатор метки хранения. [entity](/graph/api/resources/entity).|
|isInUse|Логическое|Указывает, используется ли метка в данный момент.|
|lastModifiedBy|[Microsoft.graph.identitySet](/graph/api/resources/identityset)|Пользователь, который последним изменил метку retentionLabel.|
|lastModifiedDateTime|DateTimeOffset|Дата последнего изменения метки хранения.|
|retentionDuration|[microsoft.graph.security.retentionduration](../resources/security-retentionduration.md)|Указывает количество дней для сохранения содержимого.|
|retentionTrigger|microsoft.graph.security.retentionTrigger|Указывает, рассчитывается ли длительность хранения на основе даты создания содержимого, помеченной даты или даты последнего изменения. Допустимые значения: `dateLabeled`, `dateCreated`, `dateModified`, `dateOfEvent`, `unknownFutureValue`.|
|defaultRecordBehavior|microsoft.graph.security.defaultRecordBehavior|Указывает состояние блокировки или разблокировки метки записи при ее создании. Возможные значения: `startLocked`, , `startUnlocked``unknownFutureValue`.|
|labelToBeApplied|String|Указывает метку замены, которая будет применена автоматически по истечении срока хранения текущей метки. |



## <a name="response"></a>Отклик

В случае успешного выполнения `200 OK` этот метод возвращает код отклика и обновленный объект [microsoft.graph.security.retentionLabel](../resources/security-retentionlabel.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "update_retentionlabel"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/security/labels/retentionLabels/{retentionLabelId}
Content-Type: application/json
Content-length: 555

{
  "@odata.type": "#microsoft.graph.security.retentionLabel",
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
  "labelToBeApplied": "String",
  "defaultRecordBehavior": "String"
}
```


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security.retentionLabel"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.security.retentionLabel",
  "id": "64a99fb4-07be-0481-8746-44c15c0eef1f",
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

