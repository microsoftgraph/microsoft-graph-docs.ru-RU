---
title: тип ресурса managedTenantGenericError
description: Представляет общую ошибку для управляемого клиента.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: d9cb6ac80bb48e7d8afc91db2cf386a21c7318e9
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402411"
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
