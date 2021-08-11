---
title: тип ресурса riskyUser
description: элемент рискованных пользователей
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: d54cab6905142282890f60042802c9f8060330bbffb5923505b5bae1a6cd9b45
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54235305"
---
# <a name="riskyuser-resource-type"></a>тип ресурса riskyUser

Пространство имен: microsoft.graph

Представляет пользователей Azure AD, которые находятся в опасности. Azure AD непрерывно оценивает риски пользователей на основе различных сигналов и машинного обучения. Этот API предоставляет программный доступ ко всем пользователям в Azure AD.

Дополнительные сведения о событиях риска см. [в Azure Active Directory Identity Protection.](/azure/active-directory/identity-protection/overview-identity-protection)

>**Примечание:** Использование API riskyUsers требует Azure AD Premium P2 лицензии.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список riskyUsers](../api/riskyuser-list.md)|[коллекция riskyUser](../resources/riskyuser.md)|Получите список объектов **riskyUser** и их свойств.|
|[Get riskyUser](../api/riskyuser-get.md)|[riskyUser](../resources/riskyuser.md)|Ознакомьтесь с свойствами и отношениями объекта **riskyUser.**|
|[Отклонение riskyUser](../api/riskyuser-dismiss.md)|Нет|Отклонять риск одного или более **объектов riskyUser.** |
|[Подтверждение riskyUser как скомпрометированного](../api/riskyuser-confirmcompromised.md)|Нет|Подтвердим, что один или несколько **объектов riskyUser** могут быть скомпрометированы.|
|[История списка](../api/riskyuser-list-history.md)|[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection|Получите **свойство riskyUserHistoryItems из** свойства навигации по истории.|
|[Получить историю](../api/riskyuser-get-riskyuserhistoryitem.md)|[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)|Ознакомьтесь с свойствами и отношениями объекта [riskyUserHistoryItem.](../resources/riskyuserhistoryitem.md)|


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный ID пользователя в опасности.|
|isDeleted|Логическое|Указывает, удален ли пользователь. Возможные значения: `true`, `false`.|
|isProcessing|Логическое|Указывает, обрабатывается ли приложением рискованное состояние пользователя.|
|riskDetail|riskDetail|Сведения об обнаружении риска. Возможные значения: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|riskLastUpdatedDateTime|DateTimeOffset|Дата и время последнего обновления рискованного пользователя.  Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.|
|riskLevel|riskLevel|Уровень обнаруженного рискованного пользователя. Возможные значения: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|riskState|Состояние риска пользователя. Возможные значения: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|userDisplayName|String|Рискованное имя отображения пользователя.|
|userPrincipalName|String|Рискованное основное имя пользователя.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|история|[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection|   Действие, связанное с изменением уровня риска пользователя|

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
