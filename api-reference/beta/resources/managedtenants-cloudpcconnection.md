---
title: тип ресурса cloudPcConnection
description: Представляет облачное подключение к ПК для данного управляемого клиента.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 4f7f306a54354d0c6d4860abd0866001f5e8626f
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61860434"
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
|lastRefreshedDateTime|DateTimeOffset|Дата и время последнего обновления объекта на платформе управления с несколькими клиентами. Обязательное. Только для чтения.|
|tenantDisplayName|String|Имя отображения управляемого клиента. Обязательное. Только для чтения.|
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
