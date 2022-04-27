---
title: Тип ресурса riskyUserHistoryItem
description: Рискованный элемент журнала пользователей
author: cloudhandler
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: c5853ec669c4b8ed1e048dce701ac65b3fbc1dc4
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2022
ms.locfileid: "65060981"
---
# <a name="riskyuserhistoryitem-resource-type"></a>Тип ресурса riskyUserHistoryItem

Пространство имен: microsoft.graph

Представляет журнал рисков пользователя Azure AD, определенный защитой идентификации Azure AD.

Наследуется от [riskyUser](../resources/riskyuser.md).

>[!NOTE]
> 1. Для использования этого API требуется Azure AD Premium P2 лицензия.
> 2. Доступность данных журнала рисков регулируется политиками хранения [данных Azure AD](/azure/active-directory/reports-monitoring/reference-reports-data-retention#how-long-does-azure-ad-store-the-data).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Журнал списков](../api/riskyuser-list-history.md)|[Коллекция riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)|Получите riskyUserHistoryItems из свойства навигации журнала.|
|[Получение журнала](../api/riskyuser-get-riskyuserhistoryitem.md)|[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)|Чтение свойств и связей объекта [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|действие|[riskUserActivity](../resources/riskuseractivity.md)|Действие, связанное с изменением уровня риска пользователя.|
|id|String|Наследуется [от сущности](../resources/entity.md)|
|initiatedBy|String|Идентификатор субъекта, который выполняет операцию.|
|isDeleted|Логический| Наследуется от [riskyUser](../resources/riskyuser.md)|
|isProcessing|Boolean| Наследуется от [riskyUser](../resources/riskyuser.md)|
|riskDetail|riskDetail|Наследуется [от riskyUser](../resources/riskyuser.md). Возможные значения: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|riskLastUpdatedDateTime|DateTimeOffset|Наследуется от [riskyUser](../resources/riskyuser.md)|
|riskLevel|riskLevel|Наследуется [от riskyUser](../resources/riskyuser.md). Возможные значения: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|riskState|Наследуется [от riskyUser](../resources/riskyuser.md). Возможные значения: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|userDisplayName|String|Наследуется от [riskyUser](../resources/riskyuser.md)|
|userId|String|Идентификатор пользователя.|
|userPrincipalName|String|Имя участника-пользователя с риском. Наследуется от [riskyUser](../resources/riskyuser.md)|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|Истории|[Коллекция riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)| Наследуется от [riskyUser](../resources/riskyuser.md)|

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


