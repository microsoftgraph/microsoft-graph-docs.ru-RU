---
title: тип ресурсов managedTenant
description: Представляем доступные операции, взаимодействующие с платформой управления с несколькими клиентами.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: c0929949896eb153a61bf3193d9dab5d57d92496
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53403129"
---
# <a name="managedtenant-resource-type"></a>тип ресурсов managedTenant

Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В качестве корневого ресурса Microsoft 365 Lighthouse API **managedTenant** представляет возможности, доступные поставщику управляемых служб (MSP) для масштабирования удаленного управления клиентами клиентов, чтобы помочь им в здоровом и безопасном состоянии.

API Microsoft 365 Lighthouse определяется в поднаемной области OData. `microsoft.graph.managedTenants`

## <a name="properties"></a>Свойства
Нет

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|aggregatedPolicyCompliances|[коллекция microsoft.graph.managedTenants.aggregatedPolicyCompliance](../resources/managedtenants-aggregatedpolicycompliance.md)|Сводное представление политик соответствия требованиям устройств для управляемых клиентов.|
|cloudPcConnections|[коллекция microsoft.graph.managedTenants.cloudPcConnection](../resources/managedtenants-cloudpcconnection.md)|Коллекция подключений к облачным ПК для управляемых клиентов.|
|cloudPcDevices|[коллекция microsoft.graph.managedTenants.cloudPcDevice](../resources/managedtenants-cloudpcdevice.md)|Коллекция облачных компьютеров для управляемых клиентов.|
|cloudPcsOverview|[коллекция microsoft.graph.managedTenants.cloudPcOverview](../resources/managedtenants-cloudpcoverview.md)|Обзор сведений о облачном компьютере для управляемых клиентов.|
|conditionalAccessPolicyCoverages|[коллекция microsoft.graph.managedTenants.conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md)|Сводное представление покрытия политики условного доступа для управляемых клиентов.|
|credentialUserRegistrationsSummaries|[microsoft.graph.managedTenants.credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md) collection|Сводная информация для регистрации пользователей для многофакторной проверки подлинности и сброса пароля самообслуживления для управляемых клиентов.|
|deviceCompliancePolicySettingStateSummaries|[коллекция microsoft.graph.managedTenants.deviceCompliancePolicySettingStateSummary](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md)|Сводная информация для состояния политик соответствия требованиям к устройствам для управляемых клиентов.|
|managedDeviceCompliances|[коллекция microsoft.graph.managedTenants.managedDeviceCompliance](../resources/managedtenants-manageddevicecompliance.md)|Коллекция соответствия требованиям для управляемых устройств для управляемых клиентов.|
|managedDeviceComplianceTrends|[коллекция microsoft.graph.managedTenants.managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md)|Сведения о тенденциях для соответствия требованиям устройств для управляемых клиентов.|
|managementActions|[коллекция microsoft.graph.managedTenants.managementAction](../resources/managedtenants-managementaction.md)|Коллекция базовых действий управления для управляемых клиентов.|
|managementActionTenantDeploymentStatuses|[коллекция microsoft.graph.managedTenants.managementActionTenantDeploymentStatus](../resources/managedtenants-managementactiontenantdeploymentstatus.md)|Состояние уровня клиента действий управления для управляемых клиентов.|
|managementIntents|[коллекция microsoft.graph.managedTenants.managementIntent](../resources/managedtenants-managementintent.md)|Набор базовых намерений управления для управляемых клиентов.|
|managementTemplates|[коллекция microsoft.graph.managedTenants.managementTemplate](../resources/managedtenants-managementtemplate.md)|Коллекция шаблонов базового управления для управляемых клиентов.|
|riskyUsers|[коллекция microsoft.graph.managedTenants.riskyUser](../resources/managedtenants-riskyuser.md)|Коллекция пользователей, помеченных для риска для управляемых клиентов.|
|tenantGroups|[коллекция microsoft.graph.managedTenants.tenantGroup](../resources/managedtenants-tenantgroup.md)|Коллекция логической группировки управляемых клиентов, используемых платформой управления с несколькими арендаторами.|
|клиенты|[коллекция microsoft.graph.managedTenants.tenant](../resources/managedtenants-tenant.md)|Коллекция клиентов, связанных с управляющей сущностью.|
|tenantsCustomizedInformation|[microsoft.graph.managedTenants.tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) collection|Коллекция настраиваемых сведений уровня клиента для управляемых клиентов.|
|tenantsDetailedInformation|[коллекция microsoft.graph.managedTenants.tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md)|Уровень клиента коллекции подробные сведения об управляемых клиентах.|
|tenantTags|[коллекция microsoft.graph.managedTenants.tenantTag](../resources/managedtenants-tenanttag.md)|Коллекция тегов клиента для управляемых клиентов.|
|WindowsDeviceMalwareStates|[коллекция microsoft.graph.managedTenants.windowsDeviceMalwareState](../resources/managedtenants-windowsdevicemalwarestate.md)|Состояние вредоносных программ для Windows устройств, зарегистрированных в Microsoft Endpoint Manager, в управляемых клиентах.|
|windowsProtectionStates|[коллекция microsoft.graph.managedTenants.windowsProtectionState](../resources/managedtenants-windowsprotectionstate.md)|Состояние защиты для Windows устройств, зарегистрированных Microsoft Endpoint Manager, для управляемых клиентов.|

## <a name="json-representation"></a>Представление JSON
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
