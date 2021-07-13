---
title: тип ресурса managedDeviceCompliance
description: Представляет состояние соответствия требованиям устройства для каждого управляемого устройства, принадлежащего заданным управляемым клиентом.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 237bea472df044f36fb7fbfb740fdef43260e3b2
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402532"
---
# <a name="manageddevicecompliance-resource-type"></a>тип ресурса managedDeviceCompliance

Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет состояние соответствия требованиям устройства для каждого управляемого устройства, принадлежащего заданным управляемым клиентом.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список управляемыхDeviceCompliances](../api/managedtenants-managedtenant-list-manageddevicecompliances.md)|[коллекция microsoft.graph.managedTenants.managedDeviceCompliance](../resources/managedtenants-manageddevicecompliance.md)|Получите список объектов [managedDeviceCompliance](../resources/managedtenants-manageddevicecompliance.md) и их свойств.|
|[УправлениеDeviceCompliance](../api/managedtenants-manageddevicecompliance-get.md)|[microsoft.graph.managedTenants.managedDeviceCompliance](../resources/managedtenants-manageddevicecompliance.md)|Ознакомьтесь с свойствами и отношениями объекта [managedDeviceCompliance.](../resources/managedtenants-manageddevicecompliance.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|complianceStatus|String|Состояние соответствия устройства требованиям. Это свойство доступно только для чтения. Возможные значения: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`. Необязательно. Только для чтения.|
|deviceType|String|Платформа устройства. Это свойство доступно только для чтения. Возможные значения: `desktop` `windowsRT` , `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `chromeOS` `linux` `blackberry` `palm` , `unknown` `cloudPC` , .  Необязательно. Только для чтения.|
|id|String|Уникальный идентификатор для этого объекта. Обязательный. Только для чтения.|
|inGracePeriodUntilDateTime|DateTimeOffset|Дата и время истечения срока действия льготного периода. Необязательно. Только для чтения.|
|lastRefreshedDateTime|DateTimeOffset|Дата и время последнего обновления объекта на платформе управления с несколькими клиентами. Необязательно. Только для чтения.|
|lastSyncDateTime|DateTimeOffset|Дата и время успешной синхронизации устройства с Microsoft Endpoint Manager. Необязательно. Только для чтения.|
|managedDeviceId|String|Идентификатор управляемого устройства в Microsoft Endpoint Manager. Необязательно. Только для чтения.|
|managedDeviceName|String|Имя отображения управляемого устройства. Необязательно. Только для чтения.|
|manufacturer|String|Изготовление для устройства. Необязательно. Только для чтения.|
|model|String|Модель для устройства. Необязательно. Только для чтения.|
|osDescription|String|Описание операционной системы управляемого устройства. Необязательно. Только для чтения.|
|osVersion|String|Версия операционной системы для управляемого устройства. Необязательно. Только для чтения.|
|ownerType|String|Тип владельца управляемого устройства. Необязательно. Только для чтения.|
|tenantDisplayName|String|Имя отображения управляемого клиента. Необязательно. Только для чтения.|
|tenantId|String|Идентификатор Azure Active Directory клиента для [управляемого клиента.](../resources/managedtenants-tenant.md) Необязательно. Только для чтения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.managedDeviceCompliance",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managedDeviceCompliance",
  "id": "String (identifier)",
  "tenantId": "String",
  "tenantDisplayName": "String",
  "managedDeviceId": "String",
  "managedDeviceName": "String",
  "complianceStatus": "String",
  "osDescription": "String",
  "osVersion": "String",
  "lastSyncDateTime": "String (timestamp)",
  "ownerType": "String",
  "model": "String",
  "manufacturer": "String",
  "inGracePeriodUntilDateTime": "String (timestamp)",
  "lastRefreshedDateTime": "String (timestamp)",
  "deviceType": "String"
}
```
