---
title: тип ресурса managedTenantGenericError
description: Представляет общую ошибку для управляемого клиента.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 167d8a581f2e8020ea4efabf951d07c409947ef3
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61789980"
---
# <a name="managedtenantgenericerror-resource-type"></a>тип ресурса managedTenantGenericError

Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет общую ошибку для управляемого клиента.

Наследует [от managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|error|String|Сообщение об ошибке для исключения. Наследуется [от managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md). Обязательный. Только для чтения.|
|tenantId|String|Идентификатор Azure Active Directory клиента для управляемого клиента. Наследуется [от managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md). Необязательно. Только для чтения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.managedTenantGenericError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managedTenantGenericError",
  "tenantId": "String",
  "error": "String"
}
```
