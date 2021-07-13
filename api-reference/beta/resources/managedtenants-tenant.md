---
title: тип ресурса клиента
description: Представляет клиента, связанного с управляющей сущностью.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: ee4bd57aa4e7fa2ea15c86376389d3b6e12198ea
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53403161"
---
# <a name="tenant-resource-type"></a>тип ресурса клиента

Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет клиента, связанного с управляющей сущностью.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список клиентов](../api/managedtenants-managedtenant-list-tenants.md)|[коллекция microsoft.graph.managedTenants.tenant](../resources/managedtenants-tenant.md)|Получите список объектов [клиента](../resources/managedtenants-tenant.md) и их свойств.|
|[Получить клиента](../api/managedtenants-tenant-get.md)|[microsoft.graph.managedTenants.tenant](../resources/managedtenants-tenant.md)|Ознакомьтесь с свойствами и отношениями [объекта-клиента.](../resources/managedtenants-tenant.md)|
|[offboardTenant](../api/managedtenants-tenant-offboardtenant.md)|[microsoft.graph.managedTenants.tenant](../resources/managedtenants-tenant.md)|Off boards a tenant from the multi-tenant management platform.|
|[resetTenantOnboardingStatus](../api/managedtenants-tenant-resettenantonboardingstatus.md)|[microsoft.graph.managedTenants.tenant](../resources/managedtenants-tenant.md)|Сбрасывает состояние onboarding клиента с помощью платформы управления с несколькими клиентами.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|contract|[microsoft.graph.managedTenants.tenantContract](../resources/managedtenants-tenantcontract.md)|Сведения об отношениях клиента с управляющей сущностью.|
|createdDateTime|DateTimeOffset|Дата и время создания клиента на платформе управления с несколькими арендаторами. Необязательно. Только для чтения.|
|displayName|String|Отображаемое имя для клиента. Обязательный. Только для чтения.|
|id|String|Идентификатор Azure Active Directory клиента для клиента. Обязательный. Только для чтения.|
|lastUpdatedDateTime|DateTimeOffset|Дата и время последнего обновления клиента в платформе управления с несколькими клиентами. Необязательно. Только для чтения.|
|tenantId|String|Идентификатор Azure Active Directory клиента для [управляемого клиента.](../resources/managedtenants-tenant.md) Необязательно. Только для чтения.|
|tenantStatusInformation|[microsoft.graph.managedTenants.tenantStatusInformation](../resources/managedtenants-tenantstatusinformation.md)|Сведения о состоянии на борту для клиента. Необязательно. Только для чтения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.tenant",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.tenant",
  "id": "String (identifier)",
  "tenantId": "String",
  "displayName": "String",
  "contract": {
    "@odata.type": "microsoft.graph.managedTenants.tenantContract"
  },
  "tenantStatusInformation": {
    "@odata.type": "microsoft.graph.managedTenants.tenantStatusInformation"
  },
  "lastUpdatedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)"
}
```
