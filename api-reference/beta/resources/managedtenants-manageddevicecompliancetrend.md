---
title: тип ресурса managedDeviceComplianceTrend
description: Представляет тенденцию совместимых и не совместимых устройств для данного управляемого клиента.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 671f54fb20f8ef3ecc94525061009a26e2f583f9
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61793932"
---
# <a name="manageddevicecompliancetrend-resource-type"></a>тип ресурса managedDeviceComplianceTrend

Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет тенденцию совместимых и не совместимых устройств для данного управляемого клиента.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список управляемыхDeviceComplianceTrends](../api/managedtenants-managedtenant-list-manageddevicecompliancetrends.md)|[коллекция microsoft.graph.managedTenants.managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md)|Получите список объектов [managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md) и их свойств.|
|[Get managedDeviceComplianceTrend](../api/managedtenants-manageddevicecompliancetrend-get.md)|[microsoft.graph.managedTenants.managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md)|Ознакомьтесь с свойствами и отношениями объекта [managedDeviceComplianceTrend.](../resources/managedtenants-manageddevicecompliancetrend.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|compliantDeviceCount|Int32|Количество устройств с соответствующим состоянием. Обязательный. Только для чтения.|
|configManagerDeviceCount|Int32|Количество устройств, вмеяное диспетчером конфигурации. Обязательное. Только для чтения.|
|countDateTime|String|Был выполнен снимок соответствия требованиям даты и времени. Обязательное. Только для чтения.|
|errorDeviceCount|Int32|Количество устройств с состоянием ошибки. Обязательный. Только для чтения.|
|id|String|Уникальный идентификатор для этого объекта. Обязательное. Только для чтения.|
|inGracePeriodDeviceCount|Int32|Количество устройств, которые находятся в состоянии льготного периода. Обязательный. Только для чтения.|
|noncompliantDeviceCount|Int32|Количество устройств, которые находятся в состоянии, не удовлетворяемом требованиям. Обязательное. Только для чтения.|
|tenantDisplayName|String|Имя отображения управляемого клиента. Необязательно. Только для чтения.|
|tenantId|String|Идентификатор Azure Active Directory клиента для [управляемого клиента.](../resources/managedtenants-tenant.md) Необязательно. Только для чтения.|
|unknownDeviceCount|Int32|Количество устройств в неизвестном состоянии. Обязательное. Только для чтения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.managedDeviceComplianceTrend",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managedDeviceComplianceTrend",
  "id": "String (identifier)",
  "tenantId": "String",
  "tenantDisplayName": "String",
  "unknownDeviceCount": "Integer",
  "compliantDeviceCount": "Integer",
  "noncompliantDeviceCount": "Integer",
  "errorDeviceCount": "Integer",
  "inGracePeriodDeviceCount": "Integer",
  "configManagerDeviceCount": "Integer",
  "countDateTime": "String"
}
```
