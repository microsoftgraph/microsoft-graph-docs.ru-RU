---
title: Тип ресурса unifiedRole
description: Роли каталога, которые можно назначить партнеру Майкрософт через делегированное отношение администратора.
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: resourcePageType
ms.openlocfilehash: 2355770dfdae2209d61903e7160527a57d4e5203
ms.sourcegitcommit: 5a43129dbf705f2d1a6afcff36af9f41ecee026d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2022
ms.locfileid: "64704419"
---
# <a name="unifiedrole-resource-type"></a>Тип ресурса unifiedRole
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Роли каталога, которые можно назначить партнеру Майкрософт через делегированное отношение администратора.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|roleDefinitionId|String|Идентификатор определения единой роли роли каталога. Обратитесь [к ресурсу unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) .|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.unifiedRole"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRole",
  "roleDefinitionId": "String"
}
```

