---
title: тип ресурса managedTenantOperationError
description: Абстрактный тип, который представляет ошибку для управляемой операции клиента.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: d8dc51747ac63f6f8a719b0256c398d14d1c4034
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53403045"
---
# <a name="managedtenantoperationerror-resource-type"></a>тип ресурса managedTenantOperationError

Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Абстрактный тип, который представляет ошибку для управляемой операции клиента.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|error|String|Сообщение об ошибке для исключения.|
|tenantId|String|Идентификатор Azure Active Directory клиента для [управляемого клиента.](../resources/managedtenants-tenant.md)|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.managedTenantOperationError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managedTenantOperationError",
  "tenantId": "String",
  "error": "String"
}
```
