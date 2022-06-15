---
title: Тип ресурса myRole
description: Представляет назначения ролей для пользователя, выполнившего вход, для управляемого клиента.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 3607702c037155efef1e0353b3551ba79f3eda9c
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/15/2022
ms.locfileid: "66096414"
---
# <a name="myrole-resource-type"></a>Тип ресурса myRole

Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет назначения ролей для пользователя, выполнившего вход, для [управляемого клиента](../resources/managedtenants-tenant.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление myRoles](../api/managedtenants-managedtenant-list-myroles.md)|[Коллекция microsoft.graph.managedTenants.myRole](../resources/managedtenants-myrole.md)|Получение ролей, которые пользователь выполнил вход, через делегированное отношение между [управляемыми клиентами](../resources/managedtenants-tenant.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|assignments|[Коллекция microsoft.graph.managedTenants.roleAssignment](../resources/managedtenants-roleassignment.md)|Коллекция назначений ролей для [управляемого клиента](../resources/managedtenants-tenant.md).|
|tenantId|String|Идентификатор Azure Active Directory клиента для [управляемого клиента](../resources/managedtenants-tenant.md). Необязательно. Только для чтения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.myRole",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.myRole",
  "assignments": [
    {
      "@odata.type": "microsoft.graph.managedTenants.roleAssignment"
    }
  ],
  "tenantId": "String"
}
```
