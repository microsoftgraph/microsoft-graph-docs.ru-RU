---
title: Тип ресурса riskyUser
description: Элемент "Пользователи с риском"
author: cloudhandler
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 222ff5f10fdb7ddf9ebd80209551d5e3f44ce83b
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2022
ms.locfileid: "65060788"
---
# <a name="riskyuser-resource-type"></a>Тип ресурса riskyUser

Пространство имен: microsoft.graph

Представляет пользователей Azure AD, которые находятся под угрозой. Azure AD постоянно оценивает риск пользователей на основе различных сигналов и машинного обучения. Этот API обеспечивает программный доступ ко всем пользователям, которым в Azure AD предоставляется риск.

Дополнительные сведения о событиях риска см[. в Azure Active Directory identity Protection](/azure/active-directory/identity-protection/overview-identity-protection).

>[!NOTE]
> 1. Для использования API riskyUsers требуется Azure AD Premium P2 лицензии.
> 2. Доступность рискованных пользовательских данных регулируется политиками хранения [данных Azure AD](/azure/active-directory/reports-monitoring/reference-reports-data-retention#how-long-does-azure-ad-store-the-data).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление объектов riskyUsers](../api/riskyuser-list.md)|[Коллекция riskyUser](../resources/riskyuser.md)|Получение списка объектов **riskyUser** и их свойств.|
|[Получение riskyUser](../api/riskyuser-get.md)|[riskyUser](../resources/riskyuser.md)|Чтение свойств и связей объекта **riskyUser** .|
|[Закрытие riskyUser](../api/riskyuser-dismiss.md)|Нет|Закройте риск одного или нескольких **объектов riskyUser** . |
|[Подтверждение скомпрометированного пользователя riskyUser](../api/riskyuser-confirmcompromised.md)|Нет|Подтвердите **компрометацию одного или нескольких объектов riskyUser** .|
|[Журнал списков](../api/riskyuser-list-history.md)|[Коллекция riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)|Получите **riskyUserHistoryItems из** свойства навигации журнала.|
|[Получение журнала](../api/riskyuser-get-riskyuserhistoryitem.md)|[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)|Чтение свойств и связей объекта [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) .|


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор пользователя, на который есть риск.|
|isDeleted|Boolean|Указывает, удален ли пользователь. Возможные значения: `true`, `false`.|
|isProcessing|Логическое|Указывает, обрабатывается ли серверной частью состояние риска пользователя.|
|riskDetail|riskDetail|Сведения об обнаруженном риске. Возможные значения: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|riskLastUpdatedDateTime|DateTimeOffset|Дата и время последнего обновления пользователя с риском.  Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|riskLevel|riskLevel|Уровень обнаруженного пользователя, который является рискованным. Возможные значения: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|riskState|Состояние риска пользователя. Возможные значения: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|userDisplayName|String|Отображаемое имя пользователя, которое является рискованным.|
|userPrincipalName|String|Имя участника-пользователя с риском.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|Истории|[Коллекция riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)|   Действие, связанное с изменением уровня риска пользователя|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.riskyUser",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.riskyUser",
  "id": "String (identifier)",
  "isDeleted": "Boolean",
  "isProcessing": "Boolean",
  "riskLastUpdatedDateTime": "String (timestamp)",
  "riskLevel": "String",
  "riskState": "String",
  "riskDetail": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String"
}
```
