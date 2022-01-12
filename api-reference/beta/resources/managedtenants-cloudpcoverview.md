---
title: тип ресурса cloudPcOverview
description: Представляет обзор облачных компьютеров для данного управляемого клиента.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 1eb4349c16a529c1ae3a8a9f57c221dd129ba5cc
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61795559"
---
# <a name="cloudpcoverview-resource-type"></a>тип ресурса cloudPcOverview

Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет обзор облачных компьютеров для данного управляемого клиента.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список cloudPcOverviews](../api/managedtenants-managedtenant-list-cloudpcsoverview.md)|[коллекция microsoft.graph.managedTenants.cloudPcOverview](../resources/managedtenants-cloudpcoverview.md)|Получите список объектов [cloudPcOverview](../resources/managedtenants-cloudpcoverview.md) и их свойств.|
|[Get cloudPcOverview](../api/managedtenants-cloudpcoverview-get.md)|[microsoft.graph.managedTenants.cloudPcOverview](../resources/managedtenants-cloudpcoverview.md)|Ознакомьтесь с свойствами и отношениями объекта [cloudPcOverview.](../resources/managedtenants-cloudpcoverview.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для облачного обзора ПК. Обязательный. Только для чтения.|
|lastRefreshedDateTime|DateTimeOffset|Дата и время последнего обновления объекта на платформе управления с несколькими клиентами. Необязательно. Только для чтения.|
|numberOfCloudPcConnectionStatusFailed|Int32|Количество подключений облачных ПК, которые имеют статус `failed` . Необязательно. Только для чтения.|
|numberOfCloudPcConnectionStatusPassed|Int32|Количество подключений облачных ПК, которые имеют статус `passed` . Необязательно. Только для чтения.|
|numberOfCloudPcConnectionStatusPending|Int32|Количество подключений облачных ПК, которые имеют статус `pending` . Необязательно. Только для чтения.|
|numberOfCloudPcConnectionStatusRunning|Int32|Количество подключений облачных ПК, которые имеют статус `running` . Необязательно. Только для чтения.|
|numberOfCloudPcConnectionStatusUnkownFutureValue|Int32|Количество подключений облачных ПК, которые имеют статус `unknownFutureValue` . Необязательно. Только для чтения.|
|numberOfCloudPcStatusDeprovisioning|Int32|Количество облачных компьютеров, которые имеют статус `deprovisioning` . Необязательно. Только для чтения.|
|numberOfCloudPcStatusFailed|Int32|Количество облачных компьютеров, которые имеют статус `failed` . Необязательно. Только для чтения.|
|numberOfCloudPcStatusInGracePeriod|Int32|Количество облачных компьютеров, которые имеют статус `inGracePeriod` . Необязательно. Только для чтения.|
|numberOfCloudPcStatusNotProvisioned|Int32|Количество облачных компьютеров, которые имеют статус `notProvisioned` . Необязательно. Только для чтения.|
|numberOfCloudPcStatusProvisioned|Int32|Количество облачных компьютеров, которые имеют статус `provisioned` . Необязательно. Только для чтения.|
|numberOfCloudPcStatusProvisioning|Int32|Количество облачных компьютеров, которые имеют статус `provisioning` . Необязательно. Только для чтения.|
|numberOfCloudPcStatusUnknown|Int32|Количество облачных компьютеров, которые имеют статус `unknown` . Необязательно. Только для чтения.|
|numberOfCloudPcStatusUpgrading|Int32|Количество облачных компьютеров, которые имеют статус `upgrading` . Необязательно. Только для чтения.|
|tenantDisplayName|String|Имя отображения управляемого клиента. Необязательно. Только для чтения.|
|totalCloudPcConnectionStatus|Int32|Общее число статусов подключения к облачному компьютеру для данного управляемого клиента. Необязательно. Только для чтения.|
|totalCloudPcStatus|Int32|Общее количество облачных статуй пк для данного управляемого клиента. Необязательно. Только для чтения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.cloudPcOverview",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.cloudPcOverview",
  "id": "String (identifier)",
  "tenantDisplayName": "String",
  "totalCloudPcStatus": "Integer",
  "numberOfCloudPcStatusNotProvisioned": "Integer",
  "numberOfCloudPcStatusProvisioning": "Integer",
  "numberOfCloudPcStatusProvisioned": "Integer",
  "numberOfCloudPcStatusUpgrading": "Integer",
  "numberOfCloudPcStatusInGracePeriod": "Integer",
  "numberOfCloudPcStatusDeprovisioning": "Integer",
  "numberOfCloudPcStatusFailed": "Integer",
  "numberOfCloudPcStatusUnknown": "Integer",
  "totalCloudPcConnectionStatus": "Integer",
  "numberOfCloudPcConnectionStatusPending": "Integer",
  "numberOfCloudPcConnectionStatusRunning": "Integer",
  "numberOfCloudPcConnectionStatusPassed": "Integer",
  "numberOfCloudPcConnectionStatusFailed": "Integer",
  "numberOfCloudPcConnectionStatusUnkownFutureValue": "Integer",
  "lastRefreshedDateTime": "String (timestamp)"
}
```
