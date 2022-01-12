---
title: тип ресурса aggregatedPolicyCompliance
description: Представляет сводное представление соответствия требованиям устройств для управляемого клиента.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 9db12e1a86ee6953c81be839abee695d2ba3a55a
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61862341"
---
# <a name="aggregatedpolicycompliance-resource-type"></a>тип ресурса aggregatedPolicyCompliance

Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сводное представление соответствия требованиям устройств для управляемого клиента.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список агрегированныхPolicyCompliances](../api/managedtenants-managedtenant-list-aggregatedpolicycompliances.md)|[коллекция microsoft.graph.managedTenants.aggregatedPolicyCompliance](../resources/managedtenants-aggregatedpolicycompliance.md)|Получите список объектов [aggregatedPolicyCompliance](../resources/managedtenants-aggregatedpolicycompliance.md) и их свойств.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|compliancePolicyId|String|Идентификатор для политики соответствия требованиям к устройству. Необязательно. Только для чтения.|
|compliancePolicyName|String|Имя политики соответствия требованиям к устройству. Необязательно. Только для чтения.|
|compliancePolicyPlatform|String|Платформа для политики соответствия требованиям к устройствам. Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `androidAOSP`, `all`. Необязательно. Только для чтения.|
|compliancePolicyType|String|Тип политики соответствия требованиям. Необязательно. Только для чтения.|
|id|String|Уникальный идентификатор для общей политики соответствия требованиям к устройствам. Обязательное. Только для чтения|
|lastRefreshedDateTime|DateTimeOffset|Дата и время последнего обновления объекта на платформе управления с несколькими клиентами. Необязательно. Только для чтения.|
|numberOfCompliantDevices|Int64|Количество устройств, которые находятся в состоянии совместимых. Необязательно. Только для чтения.|
|numberOfErrorDevices|Int64|Количество устройств, которые находятся в состоянии ошибки. Необязательно. Только для чтения.|
|numberOfNonCompliantDevices|Int64|Количество устройств, которые находятся в состоянии, не удовлетворяемом требованиям. Необязательно. Только для чтения.|
|policyModifiedDateTime|DateTimeOffset|Дата и время последнего изменения политики устройства. Необязательно. Только для чтения.|
|tenantDisplayName|String|Имя отображения управляемого клиента. Необязательно. Только для чтения.|
|tenantId|String|Идентификатор Azure Active Directory клиента для [управляемого клиента.](../resources/managedtenants-tenant.md) Необязательно. Только для чтения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.aggregatedPolicyCompliance",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.aggregatedPolicyCompliance",
  "id": "String (identifier)",
  "tenantId": "String",
  "tenantDisplayName": "String",
  "compliancePolicyId": "String",
  "compliancePolicyName": "String",
  "compliancePolicyType": "String",
  "compliancePolicyPlatform": "String",
  "numberOfCompliantDevices": "Integer",
  "numberOfNonCompliantDevices": "Integer",
  "numberOfErrorDevices": "Integer",
  "policyModifiedDateTime": "String (timestamp)",
  "lastRefreshedDateTime": "String (timestamp)"
}
```
