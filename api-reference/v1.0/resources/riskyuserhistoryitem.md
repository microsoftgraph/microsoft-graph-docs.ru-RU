---
title: Тип ресурса Рискюсерхисторитем
description: элемент истории опасного пользователя
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4bcf9e1834e8fff48a148095ffe7ddbd459ee23e
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896002"
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
|id|Строка|Наследуется от [объекта](../resources/entity.md)|
|initiatedBy|String|Идентификатор субъекта, который выполняет операцию.|
|isDeleted|Boolean| Наследуется от [рискюсер](../resources/riskyuser.md)|
|Процесс обработки|Boolean| Наследуется от [рискюсер](../resources/riskyuser.md)|
|riskDetail|riskDetail|Наследуется от [рискюсер](../resources/riskyuser.md). Возможные значения: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|рискластупдатеддатетиме|DateTimeOffset|Наследуется от [рискюсер](../resources/riskyuser.md)|
|riskLevel|riskLevel|Наследуется от [рискюсер](../resources/riskyuser.md). Возможные значения: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|riskState|Наследуется от [рискюсер](../resources/riskyuser.md). Возможные значения: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|userDisplayName|String|Наследуется от [рискюсер](../resources/riskyuser.md)|
|userId|String|Идентификатор пользователя.|
|userPrincipalName|Строка|Опасное имя участника пользователя. Наследуется от [рискюсер](../resources/riskyuser.md)|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|лист|Коллекция [рискюсерхисторитем](../resources/riskyuserhistoryitem.md)| Наследуется от [рискюсер](../resources/riskyuser.md)|

## <a name="json-representation"></a>Представление в формате JSON
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

