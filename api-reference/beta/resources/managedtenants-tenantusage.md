---
title: Тип ресурса tenantUsage
description: Представляет количество ежемесячно активных пользователей на службу в управляемом клиенте за предыдущий месяц. Период времени для данных — это скользящее окно, которое создает моментальный снимок один раз в день.
author: kylewirpel
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: f1d568e2218c460aeef9bff54db636f30ac94d07
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2022
ms.locfileid: "65398654"
---
# <a name="tenantusage-resource-type"></a>Тип ресурса tenantUsage

Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет количество ежемесячно активных пользователей на службу в управляемом клиенте за предыдущий месяц. Период времени для данных — это скользящее окно, которое создает моментальный снимок один раз в день.


## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление tenantUsage](../api/managedtenants-managedtenant-list-tenantusage.md)|[Коллекция microsoft.graph.managedTenants.tenantUsage](../resources/managedtenants-tenantusage.md)|Возвращает [ежемесячные данные об использовании для каждой службы](../resources/managedtenants-tenantusage.md) в [управляемом клиенте](../resources/managedtenants-managedtenant.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор клиента. Обязательно. Только для чтения.|
|reportDateTime|DateTimeOffset|День создания отчета за предыдущий месяц. Обязательно. Только для чтения.|
|serviceUsages|[Коллекция microsoft.graph.managedTenants.serviceUsage](../resources/managedtenants-serviceusage.md)|Количество ежемесячных активных пользователей для каждой службы в клиенте. Примеры служб: , , , , `Outlook``Teams`. `Word``Intune``Exchange``Excel` Обязательно. Только для чтения.|
|tenantId|String|Идентификатор Azure Active Directory клиента для [управляемого клиента](../resources/managedtenants-tenant.md). Только для чтения.|
|totalActiveUsers|Int32|Общее количество уникальных активных пользователей. Обязательно. Только для чтения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.tenantUsage",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.tenantUsage",
  "id": "String (identifier)",
  "serviceUsages": [
    {
      "@odata.type": "microsoft.graph.managedTenants.serviceUsage"
    }
  ],
  "tenantId": "String",
  "reportDateTime": "String (timestamp)",
  "totalActiveUsers": "Integer"
}
```
