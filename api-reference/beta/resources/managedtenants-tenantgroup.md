---
title: Тип ресурса tenantGroup
description: Представляет логическую группу управляемых клиентов.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: fa731082fbfc32f323b15460780e2ff355a965f8
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61791873"
---
# <a name="tenantgroup-resource-type"></a>Тип ресурса tenantGroup

Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет логическую группу управляемых клиентов.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список tenantGroups](../api/managedtenants-managedtenant-list-tenantgroups.md)|[коллекция microsoft.graph.managedTenants.tenantGroup](../resources/managedtenants-tenantgroup.md)|Получите список объектов [tenantGroup](../resources/managedtenants-tenantgroup.md) и их свойств.|
|[Get tenantGroup](../api/managedtenants-tenantgroup-get.md)|[microsoft.graph.managedTenants.tenantGroup](../resources/managedtenants-tenantgroup.md)|Ознакомьтесь с свойствами и отношениями объекта [tenantGroup.](../resources/managedtenants-tenantgroup.md)|
|[tenantSearch](../api/managedtenants-tenantgroup-tenantsearch.md)|[коллекция microsoft.graph.managedTenants.tenantGroup](../resources/managedtenants-tenantgroup.md)|Поиск определенного управляемого клиента в группах клиентов.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|allTenantsIncluded|Логический|Флаг, указывающий, включены ли все управляемые клиенты в группу клиента. Обязательное. Только для чтения.|
|displayName|String|Имя отображения для группы клиента. Необязательно. Только для чтения.|
|id|String|Уникальный идентификатор для группы клиентов. Обязательное. Только для чтения.|
|managementActions|[коллекция microsoft.graph.managedTenants.managementActionInfo](../resources/managedtenants-managementactioninfo.md)|Коллекция действий управления, связанных с группой клиентов. Необязательно. Только для чтения.|
|managementIntents|[коллекция microsoft.graph.managedTenants.managementIntentInfo](../resources/managedtenants-managementintentinfo.md)|Коллекция намерений управления, связанных с группой клиента. Необязательно. Только для чтения.|
|tenantIds|Коллекция строк|Коллекция управляемых идентификаторов клиента включается в группу клиентов. Необязательно. Только для чтения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.tenantGroup",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.tenantGroup",
  "id": "String (identifier)",
  "displayName": "String",
  "allTenantsIncluded": "Boolean",
  "tenantIds": [
    "String"
  ],
  "managementIntents": [
    {
      "@odata.type": "microsoft.graph.managedTenants.managementIntentInfo"
    }
  ],
  "managementActions": [
    {
      "@odata.type": "microsoft.graph.managedTenants.managementActionInfo"
    }
  ]
}
```
