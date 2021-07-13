---
title: Тип ресурса deviceCompliancePolicySettingStateSummary
description: Представляет сводку состояния политик соответствия требованиям к устройствам для данного управляемого клиента.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 02b69b5df1c6ae482c653960a0081bc078be815d
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402537"
---
# <a name="devicecompliancepolicysettingstatesummary-resource-type"></a>Тип ресурса deviceCompliancePolicySettingStateSummary

Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сводку состояния политик соответствия требованиям к устройствам для данного управляемого клиента.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список устройствCompliancePolicySettingStateSummary](../api/managedtenants-managedtenant-list-devicecompliancepolicysettingstatesummary.md)|[коллекция microsoft.graph.managedTenants.deviceCompliancePolicySettingStateSummary](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md)|Получите список объектов [deviceCompliancePolicySettingStateSummary](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md) и их свойств.|
|[Получение объекта deviceCompliancePolicySettingStateSummary](../api/managedtenants-devicecompliancepolicysettingstatesummary-get.md)|[microsoft.graph.managedTenants.deviceCompliancePolicySettingStateSummary](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md)|Ознакомьтесь с свойствами и отношениями [объекта deviceCompliancePolicySettingStateSummary.](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для этого объекта. Обязательный. Только для чтения.|
|conflictDeviceCount|Int32|Количество устройств в состоянии конфликта. Необязательно. Только для чтения.|
|errorDeviceCount|Int32|Количество устройств в состоянии ошибки. Необязательно. Только для чтения.|
|failedDeviceCount|Int32|Количество устройств в состоянии сбой. Необязательно. Только для чтения.|
|intuneAccountId|String|Identifer для Microsoft Intune учетной записи. Обязательный. Только для чтения.|
|intuneSettingId|String|Идентификатор для параметра Intune. Необязательно. Только для чтения.|
|lastRefreshedDateTime|DateTimeOffset|Дата и время последнего обновления объекта на платформе управления с несколькими клиентами. Необязательно. Только для чтения.|
|notApplicableDeviceCount|Int32|Количество устройств в не применимом состоянии. Необязательно. Только для чтения.|
|pendingDeviceCount|Int32|Количество устройств в ожидаемом состоянии. Необязательно. Только для чтения.|
|policyType|String|Тип для политики соответствия требованиям к устройству. Необязательно. Только для чтения.|
|settingName|String|Имя параметра в политике соответствия требованиям к устройству. Необязательно. Только для чтения.|
|succeededDeviceCount|Int32|Количество устройств в успешном состоянии. Необязательно. Только для чтения.|
|tenantDisplayName|String|Имя отображения управляемого клиента. Обязательный. Только для чтения.|
|tenantId|String|Идентификатор Azure Active Directory клиента для [управляемого клиента.](../resources/managedtenants-tenant.md) Обязательный. Только для чтения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.deviceCompliancePolicySettingStateSummary",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.deviceCompliancePolicySettingStateSummary",
  "id": "String (identifier)",
  "tenantId": "String",
  "tenantDisplayName": "String",
  "conflictDeviceCount": "Integer",
  "errorDeviceCount": "Integer",
  "failedDeviceCount": "Integer",
  "intuneAccountId": "String",
  "intuneSettingId": "String",
  "notApplicableDeviceCount": "Integer",
  "pendingDeviceCount": "Integer",
  "policyType": "String",
  "settingName": "String",
  "succeededDeviceCount": "Integer",
  "lastRefreshedDateTime": "String (timestamp)"
}
```
