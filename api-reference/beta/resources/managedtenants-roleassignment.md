---
title: Тип ресурса roleAssignment
description: Представляет назначение роли вошедаму пользователю для управляемого клиента.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 8455036941676bd304f12d957220dd982530b6db
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/15/2022
ms.locfileid: "66096411"
---
# <a name="roleassignment-resource-type"></a>Тип ресурса roleAssignment

Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет назначение роли вошедаму пользователю для [управляемого клиента](../resources/managedtenants-tenant.md).

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|assignmentType|delegatedPrivilegeStatus|Тип отношений администратора, связанных с назначением роли. Возможные значения: `none`, `delegatedAdminPrivileges`, `unknownFutureValue`, `granularDelegatedAdminPrivileges`, `delegatedAndGranularDelegetedAdminPrivileges`. Обратите внимание, что необходимо использовать заголовок `Prefer: include-unknown-enum-members` запроса для получения следующих значений из этого развиваемого [перечисления](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations): `granularDelegatedAdminPrivileges` , `delegatedAndGranularDelegetedAdminPrivileges`.|
|roles|[Коллекция microsoft.graph.managedTenants.roleDefinition](../resources/managedtenants-roledefinition.md)|Коллекция назначенных ролей.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.roleAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.roleAssignment",
  "assignmentType": "String",
  "roles": [
    {
      "@odata.type": "microsoft.graph.managedTenants.roleDefinition"
    }
  ]
}
```
