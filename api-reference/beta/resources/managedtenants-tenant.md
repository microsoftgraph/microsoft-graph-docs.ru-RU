---
title: тип ресурса клиента
description: Представляет клиента, связанного с управляющей сущностью.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 7094915b850161a14b8c5ba93bcebbfd15eedafb
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61842455"
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
|displayName|String|Отображаемое имя для клиента. Обязательное. Только для чтения.|
|id|String|Идентификатор Azure Active Directory клиента для клиента. Обязательное. Только для чтения.|
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
