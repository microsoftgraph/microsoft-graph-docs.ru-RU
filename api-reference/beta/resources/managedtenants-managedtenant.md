---
title: Тип ресурса managedTenant
description: Представляют доступные операции, взаимодействующие с мультитенантной платформой управления.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: a84cfd1bf2cdc0cae6a977ea7b31ed3b7b2c9929
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2022
ms.locfileid: "65397553"
---
# <a name="managedtenant-resource-type"></a>Тип ресурса managedTenant

Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В качестве корневого ресурса API Microsoft 365 Lighthouse **managedTenant** представляет возможности, доступные поставщику управляемых служб (MSP) для масштабирования удаленного управления клиентами клиентов, чтобы обеспечить их работоспособное и безопасное состояние.

API Microsoft 365 Lighthouse определяется в подименю OData. `microsoft.graph.managedTenants`

## <a name="properties"></a>Свойства
Нет

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|aggregatedPolicyCompliances|[Коллекция microsoft.graph.managedTenants.aggregatedPolicyCompliance](../resources/managedtenants-aggregatedpolicycompliance.md)|Агрегированное представление политик соответствия устройств в управляемых клиентах.|
|auditEvents|[Коллекция microsoft.graph.managedTenants.auditEvent](../resources/managedtenants-auditevent.md)|Коллекция событий аудита в управляемых клиентах.|
|cloudPcConnections|[Коллекция microsoft.graph.managedTenants.cloudPcConnection](../resources/managedtenants-cloudpcconnection.md)|Коллекция подключений облачных компьютеров между управляемыми клиентами.|
|cloudPcDevices|[Коллекция microsoft.graph.managedTenants.cloudPcDevice](../resources/managedtenants-cloudpcdevice.md)|Коллекция облачных компьютеров в управляемых клиентах.|
|cloudPcsOverview|[Коллекция microsoft.graph.managedTenants.cloudPcOverview](../resources/managedtenants-cloudpcoverview.md)|Общие сведения о облачных компьютерах в управляемых клиентах.|
|ConditionalAccessPolicyCoverages|[Коллекция microsoft.graph.managedTenants.conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md)|Агрегированное представление покрытия политики условного доступа для управляемых клиентов.|
|credentialUserRegistrationsSummaries|[Коллекция microsoft.graph.managedTenants.credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md)|Сводка по регистрации пользователей для многофакторной проверки подлинности и самостоятельного сброса пароля в управляемых клиентах.|
|deviceCompliancePolicySettingStateSummaries|[Коллекция microsoft.graph.managedTenants.deviceCompliancePolicySettingStateSummary](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md)|Сводка по состояниям параметров политики соответствия устройств в управляемых клиентах.|
|managedDeviceCompliances|[Коллекция microsoft.graph.managedTenants.managedDeviceCompliance](../resources/managedtenants-manageddevicecompliance.md)|Коллекция соответствия для управляемых устройств в управляемых клиентах.|
|managedDeviceComplianceTrends|[Коллекция microsoft.graph.managedTenants.managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md)|Аналитика тенденций для соответствия устройств в управляемых клиентах.|
|managementActions|[Коллекция microsoft.graph.managedTenants.managementAction](../resources/managedtenants-managementaction.md)|Коллекция базовых действий по управлению в управляемых клиентах.|
|managementActionTenantDeploymentStatuses|[Коллекция microsoft.graph.managedTenants.managementActionTenantDeploymentStatus](../resources/managedtenants-managementactiontenantdeploymentstatus.md)|Состояние действий управления на уровне клиента в управляемых клиентах.|
|managementIntents|[Коллекция microsoft.graph.managedTenants.managementIntent](../resources/managedtenants-managementintent.md)|Коллекция базовых намерений управления для управляемых клиентов.|
|managementTemplates|[Коллекция microsoft.graph.managedTenants.managementTemplate](../resources/managedtenants-managementtemplate.md)|Коллекция шаблонов базового управления для управляемых клиентов.|
|tenantGroups|[Коллекция microsoft.graph.managedTenants.tenantGroup](../resources/managedtenants-tenantgroup.md)|Коллекция логических групп управляемых клиентов, используемых платформой управления с несколькими клиентами.|
|Арендаторов|[Коллекция microsoft.graph.managedTenants.tenant](../resources/managedtenants-tenant.md)|Коллекция клиентов, связанных с управляющей сущностью.|
|tenantsCustomizedInformation|[Коллекция microsoft.graph.managedTenants.tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md)|Коллекция настраиваемых сведений на уровне клиента в управляемых клиентах.|
|tenantsDetailedInformation|[Коллекция microsoft.graph.managedTenants.tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md)|Подробные сведения об уровне клиента коллекции для управляемых клиентов.|
|tenantTags|[Коллекция microsoft.graph.managedTenants.tenantTag](../resources/managedtenants-tenanttag.md)|Коллекция тегов клиента в управляемых клиентах.|
|tenantUsage|[Коллекция microsoft.graph.managedTenants.tenantUsage](../resources/managedtenants-tenantusage.md)|Коллекция сведений об использовании клиентов в управляемых клиентах.|
|windowsDeviceMalwareStates|[Коллекция microsoft.graph.managedTenants.windowsDeviceMalwareState](../resources/managedtenants-windowsdevicemalwarestate.md)|Состояние вредоносных программ для Windows устройств, зарегистрированных в Microsoft Endpoint Manager, в управляемых клиентах.|
|windowsProtectionStates|[Коллекция microsoft.graph.managedTenants.windowsProtectionState](../resources/managedtenants-windowsprotectionstate.md)|Состояние защиты для Windows устройств, зарегистрированных в Microsoft Endpoint Manager, в управляемых клиентах.|

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.managedTenant",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managedTenant",
  "id": "String (identifier)"
}
```
