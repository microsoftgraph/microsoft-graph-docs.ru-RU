---
title: тип ресурса managedTenantExecutionError
description: Представляет исключение для управляемой операции клиента.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 5a1fd2d1524cad663ee6acef93ab20cc8e40fd24
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402429"
---
# <a name="managedtenantexecutionerror-resource-type"></a>тип ресурса managedTenantExecutionError

Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет исключение для управляемой операции клиента.

Наследует [от managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|error|String|Сообщение об ошибке для исключения. Наследуется [от managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md). Обязательный. Только для чтения.|
|errorDetails|String|Дополнительные сведения об ошибках для исключения. Необязательно. Только для чтения.|
|nodeId|Int32|Идентификатор узла, в котором произошло исключение. Обязательный. Только для чтения.|
|rawToken|String|Маркер для исключения. Необязательно. Только для чтения.|
|statementIndex|Int32|Индекс заявления для исключения. Обязательный. Только для чтения.|
|tenantId|String|Идентификатор Azure Active Directory клиента для управляемого клиента. Наследуется [от managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md). Обязательный. Только для чтения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.managedTenantExecutionError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managedTenantExecutionError",
  "tenantId": "String",
  "error": "String",
  "rawToken": "String",
  "statementIndex": "Integer",
  "nodeId": "Integer",
  "errorDetails": "String"
}
```
