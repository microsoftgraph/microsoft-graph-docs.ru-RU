---
title: Тип ресурса tenantGroup
description: Представляет логическую группу управляемых клиентов.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 2ab0d97afff68dca7d76b1ad6c4e461ad6af6233
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402693"
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
|allTenantsIncluded|Boolean|Флаг, указывающий, включены ли все управляемые клиенты в группу клиента. Обязательный. Только для чтения.|
|displayName|String|Имя отображения для группы клиента. Необязательно. Только для чтения.|
|id|String|Уникальный идентификатор для группы клиентов. Обязательный. Только для чтения.|
|managementActions|[коллекция microsoft.graph.managedTenants.managementActionInfo](../resources/managedtenants-managementactioninfo.md)|Коллекция действий управления, связанных с группой клиентов. Необязательно. Только для чтения.|
|managementIntents|[коллекция microsoft.graph.managedTenants.managementIntentInfo](../resources/managedtenants-managementintentinfo.md)|Коллекция намерений управления, связанных с группой клиента. Необязательно. Только для чтения.|
|tenantIds|Коллекция объектов string|Коллекция управляемых идентификаторов клиента включается в группу клиентов. Необязательно. Только для чтения.|

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
