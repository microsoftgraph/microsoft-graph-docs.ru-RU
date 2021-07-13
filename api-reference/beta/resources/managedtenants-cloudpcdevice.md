---
title: тип ресурса cloudPcDevice
description: Представляет облачное компьютерное устройство, принадлежающее заданным управляемым клиентом.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 57eabb6720987a8a9bfca4c18e283057848b65cf
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402549"
---
# <a name="cloudpcdevice-resource-type"></a>тип ресурса cloudPcDevice

Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет облачное компьютерное устройство, принадлежающее заданным управляемым клиентом.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список cloudPcDevices](../api/managedtenants-managedtenant-list-cloudpcdevices.md)|[коллекция microsoft.graph.managedTenants.cloudPcDevice](../resources/managedtenants-cloudpcdevice.md)|Получите список объектов [cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) и их свойств.|
|[Get cloudPcDevice](../api/managedtenants-cloudpcdevice-get.md)|[microsoft.graph.managedTenants.cloudPcDevice](../resources/managedtenants-cloudpcdevice.md)|Ознакомьтесь с свойствами и отношениями объекта [cloudPcDevice.](../resources/managedtenants-cloudpcdevice.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|cloudPcStatus|String|Состояние облачного КОМПЬЮТЕРА. Возможные значения: `notProvisioned`, `provisioning`, `provisioned`, `upgrading`, `inGracePeriod`, `deprovisioning`, `failed`. Обязательный. Только для чтения.|
|displayName|String|Имя отображения облачного компьютера. Обязательный. Только для чтения.|
|id|String|Уникальный идентификатор облачного компьютера. Обязательный. Только для чтения.|
|lastRefreshedDateTime|DateTimeOffset|Дата и время последнего обновления объекта на платформе управления с несколькими клиентами. Обязательный. Только для чтения.|
|managedDeviceId|String|Идентификатор управляемого устройства для облачного КОМПЬЮТЕРА. Необязательно. Только для чтения.|
|managedDeviceName|String|Имя отображения управляемого устройства для облачного компьютера. Необязательно. Только для чтения.|
|provisioningPolicyId|String|Идентификатор политики обеспечения для облачного компьютера. Обязательный. Только для чтения.|
|servicePlanName|String|Имя плана службы для облачного компьютера. Обязательный. Только для чтения.|
|tenantDisplayName|String|Имя отображения управляемого клиента. Обязательный. Только для чтения.|
|tenantId|String|Идентификатор Azure Active Directory клиента для [управляемого клиента.](../resources/managedtenants-tenant.md) Обязательный. Только для чтения.|
|userPrincipalName|String|Основное имя пользователя (UPN) пользователя, назначенного на облачный КОМПЬЮТЕР. Обязательный. Только для чтения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.cloudPcDevice",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.cloudPcDevice",
  "id": "String (identifier)",
  "displayName": "String",
  "tenantId": "String",
  "tenantDisplayName": "String",
  "managedDeviceId": "String",
  "managedDeviceName": "String",
  "userPrincipalName": "String",
  "servicePlanName": "String",
  "cloudPcStatus": "String",
  "provisioningPolicyId": "String",
  "lastRefreshedDateTime": "String (timestamp)"
}
```
