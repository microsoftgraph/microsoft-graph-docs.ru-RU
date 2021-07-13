---
title: тип ресурса cloudPcConnection
description: Представляет облачное подключение к ПК для данного управляемого клиента.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 75af7be7633e43bc594f7185f196f40abca39883
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402550"
---
# <a name="cloudpcconnection-resource-type"></a>тип ресурса cloudPcConnection

Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет облачное подключение к ПК для данного управляемого клиента.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список cloudPcConnections](../api/managedtenants-managedtenant-list-cloudpcconnections.md)|[коллекция microsoft.graph.managedTenants.cloudPcConnection](../resources/managedtenants-cloudpcconnection.md)|Получите список объектов [cloudPcConnection](../resources/managedtenants-cloudpcconnection.md) и их свойств.|
|[Get cloudPcConnection](../api/managedtenants-cloudpcconnection-get.md)|[microsoft.graph.managedTenants.cloudPcConnection](../resources/managedtenants-cloudpcconnection.md)|Ознакомьтесь с свойствами и отношениями объекта [cloudPcConnection.](../resources/managedtenants-cloudpcconnection.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Отображение имени облачного подключения к КОМПЬЮТЕРУ. Обязательный. Только для чтения.|
|healthCheckStatus|String|Состояние здоровья облачного подключения к ПК. Возможные значения: `pending`, `running`, `passed`, `failed`, `unknownFutureValue`.  Обязательный атрибут. Только для чтения.|
|id|String|Уникальный идентификатор для облачного подключения к ПК. Обязательный. Только для чтения.|
|lastRefreshedDateTime|DateTimeOffset|Дата и время последнего обновления объекта на платформе управления с несколькими клиентами. Обязательный. Только для чтения.|
|tenantDisplayName|String|Имя отображения управляемого клиента. Обязательный. Только для чтения.|
|tenantId|String|Идентификатор Azure Active Directory клиента для [управляемого клиента.](../resources/managedtenants-tenant.md) Обязательный. Только для чтения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.cloudPcConnection",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.cloudPcConnection",
  "id": "String (identifier)",
  "displayName": "String",
  "tenantId": "String",
  "tenantDisplayName": "String",
  "healthCheckStatus": "String",
  "lastRefreshedDateTime": "String (timestamp)"
}
```
