---
title: тип ресурса windowsProtectionState
description: Представляем состояние Windows для управляемых устройств, работающих Windows.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: dc89db998f8fa75e46b3346f2517e5ee950e0ab5
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402627"
---
# <a name="windowsprotectionstate-resource-type"></a>тип ресурса windowsProtectionState

Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляем состояние Windows для управляемых устройств, работающих Windows.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список windowsProtectionStates](../api/managedtenants-managedtenant-list-windowsprotectionstates.md)|[коллекция microsoft.graph.managedTenants.windowsProtectionState](../resources/managedtenants-windowsprotectionstate.md)|Получите список объектов [WindowsProtectionState](../resources/managedtenants-windowsprotectionstate.md) и их свойств.|
|[Get windowsProtectionState](../api/managedtenants-windowsprotectionstate-get.md)|[microsoft.graph.managedTenants.windowsProtectionState](../resources/managedtenants-windowsprotectionstate.md)|Ознакомьтесь с свойствами и отношениями [объекта windowsProtectionState.](../resources/managedtenants-windowsprotectionstate.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|antiMalwareVersion|String|Антивирусная версия для управляемого устройства. Необязательно. Только для чтения.|
|attentionRequired|Boolean|Флаг, указывающий, требуется ли внимание для управляемого устройства. Необязательно. Только для чтения.|
|deviceDeleted|Boolean|Флаг, указывающий, удалено ли управляемое устройство. Необязательно. Только для чтения.|
|devicePropertyRefreshDateTime|DateTimeOffset|Дата и время обновления свойства устройства. Необязательно. Только для чтения.|
|engineVersion|String|Версия антивирусного двигателя для управляемого устройства. Необязательно. Только для чтения.|
|fullScanOverdue|Boolean|Флаг, указывающий, просрочена ли быстрая проверка управляемого устройства. Необязательно. Только для чтения.|
|fullScanRequired|Boolean|Флаг, указывающий, просрочена ли полная проверка управляемого устройства. Необязательно. Только для чтения.|
|id|String|Уникальный идентификатор состояния Windows защиты. Обязательный. Только для чтения.|
|lastFullScanDateTime|DateTimeOffset|Дата и время завершения полного сканирования. Необязательно. Только для чтения.|
|lastFullScanSignatureVersion|String|Версия антивирусной версии, используемая для последнего полного сканирования. Необязательно. Только для чтения.|
|lastQuickScanDateTime|DateTimeOffset|Дата и время быстрого сканирования завершены. Необязательно. Только для чтения.|
|lastQuickScanSignatureVersion|String|Версия антивирусной версии, используемая для последнего полного сканирования. Необязательно. Только для чтения.|
|lastRefreshedDateTime|DateTimeOffset|Дата и время последнего обновления объекта на платформе управления с несколькими клиентами. Необязательно. Только для чтения.|
|lastReportedDateTime|DateTimeOffset|Дата и время последнего сообщений о состоянии защиты для управляемого устройства. Необязательно. Только для чтения.|
|malwareProtectionEnabled|Boolean|Флаг, указывающий, включена ли защита от вредоносных программ для управляемого устройства. Необязательно. Только для чтения.|
|managedDeviceHealthState|String|Состояние здоровья управляемого устройства. Необязательно. Только для чтения.|
|managedDeviceId|String|Уникальный идентификатор управляемого устройства. Необязательно. Только для чтения.|
|managedDeviceName|String|Имя отображения управляемого устройства. Необязательно. Только для чтения.|
|networkInspectionSystemEnabled|Boolean|Флаг, указывающий, включена ли система проверки сети. Необязательно. Только для чтения.|
|quickScanOverdue|Boolean|Флаг, указывающий на погоду, просрочен. Необязательно. Только для чтения.|
|realTimeProtectionEnabled|Boolean|Флаг, указывающий, включена ли защита в режиме реального времени. Необязательно. Только для чтения.|
|rebootRequired|Boolean|Флаг, указывающий, требуется ли перезагрузка. Необязательно. Только для чтения.|
|signatureUpdateOverdue|Boolean|Флаг, указывающий, просрочено ли обновление подписи. Необязательно. Только для чтения.|
|signatureVersion|String|Версия подписи для управляемого устройства. Необязательно. Только для чтения.|
|tenantDisplayName|String|Имя отображения управляемого клиента. Необязательно. Только для чтения.|
|tenantId|String|Идентификатор Azure Active Directory клиента для [управляемого клиента.](../resources/managedtenants-tenant.md) Необязательно. Только для чтения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.windowsProtectionState",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.windowsProtectionState",
  "id": "String (identifier)",
  "tenantId": "String",
  "tenantDisplayName": "String",
  "managedDeviceId": "String",
  "managedDeviceName": "String",
  "malwareProtectionEnabled": "Boolean",
  "managedDeviceHealthState": "String",
  "realTimeProtectionEnabled": "Boolean",
  "networkInspectionSystemEnabled": "Boolean",
  "quickScanOverdue": "Boolean",
  "fullScanOverdue": "Boolean",
  "signatureUpdateOverdue": "Boolean",
  "rebootRequired": "Boolean",
  "attentionRequired": "Boolean",
  "fullScanRequired": "Boolean",
  "engineVersion": "String",
  "signatureVersion": "String",
  "antiMalwareVersion": "String",
  "lastQuickScanDateTime": "String (timestamp)",
  "lastFullScanDateTime": "String (timestamp)",
  "lastQuickScanSignatureVersion": "String",
  "lastFullScanSignatureVersion": "String",
  "lastReportedDateTime": "String (timestamp)",
  "devicePropertyRefreshDateTime": "String (timestamp)",
  "deviceDeleted": "Boolean",
  "lastRefreshedDateTime": "String (timestamp)"
}
```
