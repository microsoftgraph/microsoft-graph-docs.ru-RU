---
title: Тип ресурса auditEvent
description: Представляет событие аудита для управляемых клиентов в Microsoft 365 Lighthouse.
author: vkumar2015
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: d0a6097178f160fd305060a4a7d6a289b184228c
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63339413"
---
# <a name="auditevent-resource-type"></a>Тип ресурса auditEvent

Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет событие аудита для управляемых клиентов в Microsoft 365 Lighthouse.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список объектов auditEvent](../api/managedtenants-managedtenant-list-auditevents.md)|[коллекция microsoft.graph.managedTenants.auditEvent](../resources/managedtenants-auditevent.md)|Получите список объектов [auditEvent](../resources/managedtenants-auditevent.md) и их свойств.|
|[Получение объекта auditEvent](../api/managedtenants-auditevent-get.md)|[microsoft.graph.managedTenants.auditEvent](../resources/managedtenants-auditevent.md)|Ознакомьтесь с свойствами и отношениями объекта [auditEvent](../resources/managedtenants-auditevent.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|activity|String|Строка, которая однозначно представляет операцию, которая произошла. Обязательный элемент. Только для чтения.|
|activityDateTime|DateTimeOffset|Время, когда действие не было. Обязательный элемент. Только для чтения.|
|activityId|Строка|Идентификатор запроса действий, который сделал событие аудита. Обязательный элемент. Только для чтения.|
|category|String|Категория, представляюная логическую группу действий. Обязательный элемент. Только для чтения.|
|httpVerb|Строка|Глагол HTTP, который использовался при создании запроса API. Обязательный элемент. Только для чтения.|
|id|String|Уникальный идентификатор события аудита. Обязательный элемент. Только для чтения.|
|initiatedByAppId|String|Идентификатор приложения, которое использовалось для запроса. Обязательный элемент. Только для чтения.|
|initiatedByUpn|String|UpN пользователя, который инициировал эту деятельность. Обязательный элемент. Только для чтения.|
|initiatedByUserId|Строка|Идентификатор пользователя, который инициировал действие. Обязательный элемент. Только для чтения.|
|ipAddress|String|IP-адрес, на котором было инициировано действие. Это может быть IPv4- или IPv6-адрес. Обязательный элемент. Только для чтения.|
|requestBody|Строка|Необработанные http-запросы. Некоторые конфиденциальные сведения могут быть удалены.|
|requestUrl|Строка|Необработанные URL-адрес запроса HTTP. Обязательный элемент. Только для чтения.|
|tenantIds|Строка|Коллекция идентификаторов Azure Active Directory для управляемых [клиентов, на](../resources/managedtenants-tenant.md) которые повлияло это изменение. Это форматированный список значений, разделенных запятой. Обязательный элемент. Только для чтения.|
|tenantNames|Строка|Коллекция имен клиентов, на которые повлияло это изменение. Это форматированный список значений, разделенных запятой. Обязательный элемент. Только для чтения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.auditEvent",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.auditEvent",
  "activity": "String",
  "activityDateTime": "String (timestamp)",
  "activityId": "String",
  "category": "String",
  "httpVerb": "String",
  "id": "String (identifier)",
  "initiatedByAppId": "String",
  "initiatedByUpn": "String",
  "initiatedByUserId": "String",
  "ipAddress": "String",
  "requestBody": "String",
  "requestUrl": "String",
  "tenantIds": "String",
  "tenantNames": "String"
}
```

