---
title: тип ресурса managedTenantExecutionError
description: Представляет исключение для управляемой операции клиента.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 92917d60cc3bd22da02a8d447c305e275bab51a3
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61791898"
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
|nodeId|Int32|Идентификатор узла, в котором произошло исключение. Обязательное. Только для чтения.|
|rawToken|String|Маркер для исключения. Необязательно. Только для чтения.|
|statementIndex|Int32|Индекс заявления для исключения. Обязательное. Только для чтения.|
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
