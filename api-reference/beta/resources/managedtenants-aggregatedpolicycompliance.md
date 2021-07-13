---
title: тип ресурса aggregatedPolicyCompliance
description: Представляет сводное представление соответствия требованиям устройств для управляемого клиента.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 8b2c6ce85c0ec6df361ddfeb13a851740efb2acb
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402555"
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
|id|String|Уникальный идентификатор для общей политики соответствия требованиям к устройствам. Обязательный. Только для чтения|
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
