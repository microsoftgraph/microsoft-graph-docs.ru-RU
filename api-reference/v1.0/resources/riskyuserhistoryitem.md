---
title: тип ресурса riskyUserHistoryItem
description: рискованный элемент истории пользователей
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: c83f35d9d8d187fd3a3bb64d727261431e3b13700735c4ad618f0a01b80fc1ce
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54189389"
---
# <a name="riskyuserhistoryitem-resource-type"></a>тип ресурса riskyUserHistoryItem

Пространство имен: microsoft.graph

Представляет историю рисков пользователя Azure AD, определяемую службой Azure AD Identity Protection.


Наследует от [riskyUser](../resources/riskyuser.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[История списка](../api/riskyuser-list-history.md)|[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection|Получите свойство riskyUserHistoryItems из свойства навигации по истории.|
|[Получить историю](../api/riskyuser-get-riskyuserhistoryitem.md)|[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)|Ознакомьтесь с свойствами и отношениями объекта [riskyUserHistoryItem.](../resources/riskyuserhistoryitem.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|действие|[riskUserActivity](../resources/riskuseractivity.md)|Действие, связанное с изменением уровня риска пользователя.|
|id|String|Унаследованный от [сущности](../resources/entity.md)|
|initiatedBy|String|ID субъекта, который делает операцию.|
|isDeleted|Логический| Унаследованный от [riskyUser](../resources/riskyuser.md)|
|isProcessing|Логический| Унаследованный от [riskyUser](../resources/riskyuser.md)|
|riskDetail|riskDetail|Унаследованный от [riskyUser](../resources/riskyuser.md). Возможные значения: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|riskLastUpdatedDateTime|DateTimeOffset|Унаследованный от [riskyUser](../resources/riskyuser.md)|
|riskLevel|riskLevel|Унаследованный от [riskyUser](../resources/riskyuser.md). Возможные значения: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|riskState|Унаследованный от [riskyUser](../resources/riskyuser.md). Возможные значения: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|userDisplayName|String|Унаследованный от [riskyUser](../resources/riskyuser.md)|
|userId|String|ID пользователя.|
|userPrincipalName|String|Рискованное основное имя пользователя. Унаследованный от [riskyUser](../resources/riskyuser.md)|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|история|[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection| Унаследованный от [riskyUser](../resources/riskyuser.md)|

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


