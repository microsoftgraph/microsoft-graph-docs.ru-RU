---
title: Тип ресурса Рискюсер
description: элемент рискованных пользователей
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2810ffc35b1550ae75a21b5f8baebb91c444799f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47984189"
---
# <a name="riskyuser-resource-type"></a>Тип ресурса Рискюсер

Пространство имен: microsoft.graph

Представляет пользователей Azure AD, которые находятся под угрозой. Azure AD постоянно оценивает риск пользователя на основе различных сигналов и машинного обучения. Этот API предоставляет программный доступ ко всем пользователям с рисками в Azure AD.

Для получения дополнительных сведений о событиях риска обратитесь к разделу [Защита удостоверений Azure Active Directory](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/).

>**Примечание:** Для использования API riskyUsers требуется лицензия Azure AD Premium P2.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список riskyUsers](../api/riskyuser-list.md)|Коллекция [рискюсер](../resources/riskyuser.md)|Получение списка объектов **рискюсер** и их свойств.|
|[Получение Рискюсер](../api/riskyuser-get.md)|[рискюсер](../resources/riskyuser.md)|Чтение свойств и связей объекта **рискюсер** .|
|[Отклонение Рискюсер](../api/riskyuser-dismiss.md)|Нет|Отклонить риск одного или нескольких объектов **рискюсер** . |
|[Подтверждение Рискюсер в качестве скомпрометированного](../api/riskyuser-confirmcompromised.md)|Нет|Подтвердите, что один или несколько объектов **рискюсер** считаются скомпрометированными.|
|[Журнал списка](../api/riskyuser-list-history.md)|Коллекция [рискюсерхисторитем](../resources/riskyuserhistoryitem.md)|Получение **рискюсерхисторитемс** из свойства навигации по журналу.|
|[Получение журнала](../api/riskyuser-get-riskyuserhistoryitem.md)|[рискюсерхисторитем](../resources/riskyuserhistoryitem.md)|Чтение свойств и связей объекта [рискюсерхисторитем](../resources/riskyuserhistoryitem.md) .|


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор пользователя под угрозой.|
|isDeleted|Boolean|Указывает, удален ли пользователь. Возможные значения: `true` , `false`|
|Процесс обработки|Boolean|Указывает, вехсер ли опасное состояние пользователя при обработке внутренней|
|riskDetail|riskDetail|Сведения об обнаруженном риске. Возможные значения: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|рискластупдатеддатетиме|DateTimeOffset|Дата и время последнего обновления рискованного пользователя.|
|riskLevel|riskLevel|Уровень обнаруженного опасного пользователя. Возможные значения: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|riskState|Состояние риска пользователя. Возможные значения: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|userDisplayName|String|Опасное отображаемое имя пользователя.|
|userPrincipalName|String|Опасное имя участника пользователя.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|лист|Коллекция [рискюсерхисторитем](../resources/riskyuserhistoryitem.md)|   Действие, связанное с изменением уровня риска пользователя|

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


