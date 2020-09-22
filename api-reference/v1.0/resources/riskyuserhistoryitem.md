---
title: Тип ресурса Рискюсерхисторитем
description: элемент истории опасного пользователя
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 551f008696b3c9507f1cae414c34de5a8779ab24
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47984161"
---
# <a name="riskyuserhistoryitem-resource-type"></a>Тип ресурса Рискюсерхисторитем

Пространство имен: microsoft.graph

Представляет историю риска пользователя Azure AD, определенная службой защиты удостоверений Azure AD.


Наследуется от [рискюсер](../resources/riskyuser.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Журнал списка](../api/riskyuser-list-history.md)|Коллекция [рискюсерхисторитем](../resources/riskyuserhistoryitem.md)|Получение Рискюсерхисторитемс из свойства навигации по журналу.|
|[Получение журнала](../api/riskyuser-get-riskyuserhistoryitem.md)|[рискюсерхисторитем](../resources/riskyuserhistoryitem.md)|Чтение свойств и связей объекта [рискюсерхисторитем](../resources/riskyuserhistoryitem.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|activity|[рискусерактивити](../resources/riskuseractivity.md)|Действие, связанное с изменением уровня риска пользователя.|
|id|String|Наследуется от [объекта](../resources/entity.md)|
|initiatedBy|String|Идентификатор субъекта, который выполняет операцию.|
|isDeleted|Boolean| Наследуется от [рискюсер](../resources/riskyuser.md)|
|Процесс обработки|Boolean| Наследуется от [рискюсер](../resources/riskyuser.md)|
|riskDetail|riskDetail|Наследуется от [рискюсер](../resources/riskyuser.md). Возможные значения: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|рискластупдатеддатетиме|DateTimeOffset|Наследуется от [рискюсер](../resources/riskyuser.md)|
|riskLevel|riskLevel|Наследуется от [рискюсер](../resources/riskyuser.md). Возможные значения: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|riskState|Наследуется от [рискюсер](../resources/riskyuser.md). Возможные значения: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|userDisplayName|String|Наследуется от [рискюсер](../resources/riskyuser.md)|
|userId|String|Идентификатор пользователя.|
|userPrincipalName|String|Опасное имя участника пользователя. Наследуется от [рискюсер](../resources/riskyuser.md)|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|лист|Коллекция [рискюсерхисторитем](../resources/riskyuserhistoryitem.md)| Наследуется от [рискюсер](../resources/riskyuser.md)|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.riskyUserHistoryItem",
  "baseType": "microsoft.graph.riskyUser",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.riskyUserHistoryItem",
  "id": "String (identifier)",
  "isDeleted": "Boolean",
  "isProcessing": "Boolean",
  "riskLastUpdatedDateTime": "String (timestamp)",
  "riskLevel": "String",
  "riskState": "String",
  "riskDetail": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "userId": "String",
  "initiatedBy": "String",
  "activity": {
    "@odata.type": "microsoft.graph.riskUserActivity"
  }
}
```


