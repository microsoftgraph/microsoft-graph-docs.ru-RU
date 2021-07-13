---
title: тип ресурса riskyUser
description: Представляет учетную запись, помеченную для риска для каждого управляемого клиента.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 3f66998080abcf9580cdd36e0f3e4b24edab2d2d
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53403165"
---
# <a name="riskyuser-resource-type"></a>тип ресурса riskyUser

Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет учетную запись, помеченную для риска для каждого управляемого клиента.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список riskyUsers](../api/managedtenants-managedtenant-list-riskyusers.md)|[коллекция microsoft.graph.managedTenants.riskyUser](../resources/managedtenants-riskyuser.md)|Получите список объектов [riskyUser](../resources/managedtenants-riskyuser.md) и их свойств.|
|[Get riskyUser](../api/managedtenants-riskyuser-get.md)|[microsoft.graph.managedTenants.riskyUser](../resources/managedtenants-riskyuser.md)|Ознакомьтесь с свойствами и отношениями объекта [riskyUser.](../resources/managedtenants-riskyuser.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для этого объекта. Обязательный. Только для чтения.|
|isDeleted|Boolean|Флаг, указывающий, удалена ли учетная запись. Необязательно. Только для чтения.|
|lastRefreshedDateTime|DateTimeOffset|Дата и время последнего обновления объекта на платформе управления с несколькими клиентами. Необязательно. Только для чтения.|
|riskDetail|String|Сведения о рисках для учетной записи, помеченной для риска. Необязательно. Только для чтения.|
|riskLastUpdatedDateTime|DateTimeOffset|Дата и время последнего обновления сведений о рисках. Необязательно. Только для чтения.|
|riskLevel|String|Уровень риска, который был обнаружен. Возможные значения: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`. Необязательно. Только для чтения.|
|riskState|String|Обнаружено состояние риска. Возможные значения: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`. Необязательно. Только для чтения.|
|tenantDisplayName|String|Имя отображения управляемого клиента. Необязательно. Только для чтения.|
|tenantId|String|Идентификатор Azure Active Directory клиента для [управляемого клиента.](../resources/managedtenants-tenant.md) Обязательный. Только для чтения.|
|userDisplayName|String|Имя отображения учетной записи, в которой был обнаружен риск. Необязательно. Только для чтения.|
|userId|String|Идентификатор учетной записи пользователя, в которой был обнаружен риск. Обязательный. Только для чтения.|
|userPrincipalName|String|Основное имя пользователя (UPN) для учетной записи, где был обнаружен риск. Необязательно. Только для чтения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.riskyUser",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.riskyUser",
  "id": "String (identifier)",
  "userId": "String",
  "tenantId": "String",
  "tenantDisplayName": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "riskState": "String",
  "riskLevel": "String",
  "riskDetail": "String",
  "isDeleted": "Boolean",
  "riskLastUpdatedDateTime": "String (timestamp)",
  "lastRefreshedDateTime": "String (timestamp)"
}
```
