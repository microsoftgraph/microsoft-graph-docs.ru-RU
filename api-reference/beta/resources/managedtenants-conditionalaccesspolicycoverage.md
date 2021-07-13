---
title: тип ресурса conditionalAccessPolicyCoverage
description: Представляет сведения о любой политике Azure Active Directory, определяемой правилами доступа к ресурсу для данного управляемого клиента.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: a4bc4f336692166ff032727a6fb13222edd9d7d9
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402543"
---
# <a name="conditionalaccesspolicycoverage-resource-type"></a>тип ресурса conditionalAccessPolicyCoverage

Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о любой политике Azure Active Directory, определяемой правилами доступа к ресурсу для данного управляемого клиента.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список conditionalAccessPolicyCoverages](../api/managedtenants-managedtenant-list-conditionalaccesspolicycoverages.md)|[коллекция microsoft.graph.managedTenants.conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md)|Получите список объектов [conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) и их свойств.|
|[Get conditionalAccessPolicyCoverage](../api/managedtenants-conditionalaccesspolicycoverage-get.md)|[microsoft.graph.managedTenants.conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md)|Ознакомьтесь с свойствами и отношениями объекта [conditionalAccessPolicyCoverage.](../resources/managedtenants-conditionalaccesspolicycoverage.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|conditionalAccessPolicyState|String|Состояние политики условного доступа. Возможные значения: `enabled`, `disabled`, `enabledForReportingButNotEnforced`. Обязательное. Только для чтения.|
|id|String|Уникальный идентификатор для этого объекта. Обязательный. Только для чтения.|
|latestPolicyModifiedDateTime|DateTimeOffset|Дата и время последнего изменения политики условного доступа. Обязательный. Только для чтения.|
|requiresDeviceCompliance|Boolean|Флаг, указывающий, требуется ли политике условного доступа соответствие требованиям устройства. Обязательный. Только для чтения.|
|tenantDisplayName|String|Имя отображения управляемого клиента. Обязательный. Только для чтения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.conditionalAccessPolicyCoverage",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.conditionalAccessPolicyCoverage",
  "id": "String (identifier)",
  "tenantDisplayName": "String",
  "conditionalAccessPolicyState": "String",
  "requiresDeviceCompliance": "Boolean",
  "latestPolicyModifiedDateTime": "String (timestamp)"
}
```
