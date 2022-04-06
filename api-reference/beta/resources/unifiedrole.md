---
title: тип ресурсов unifiedRole
description: Роли каталога, которые могут быть назначены партнеру Майкрософт через делегированную связь администратора.
author: adtangir
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 8a5c1cc9d450275642e767f7653eea09bcb103f6
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589958"
---
# <a name="unifiedrole-resource-type"></a>тип ресурсов unifiedRole
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Роли каталога, которые могут быть назначены партнеру Майкрософт через делегированную связь администратора.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|roleDefinitionId|Строка|Единый ID определения роли роли каталога. Обратитесь [к ресурсу unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) .|

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

