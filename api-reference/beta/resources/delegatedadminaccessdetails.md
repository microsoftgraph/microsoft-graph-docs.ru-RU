---
title: Тип ресурса delegatedAdminAccessDetails
description: Представляет административные роли, которые партнер Майкрософт имеет в клиенте клиента через делегированные отношения администратора и делегированное назначение доступа администратора.
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: resourcePageType
ms.openlocfilehash: c67f7792ea1124228a23fdc5b642dc3de47739a8
ms.sourcegitcommit: 5a43129dbf705f2d1a6afcff36af9f41ecee026d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2022
ms.locfileid: "64704199"
---
# <a name="delegatedadminaccessdetails-resource-type"></a>Тип ресурса delegatedAdminAccessDetails

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет административные роли, которые партнер Майкрософт имеет в клиенте клиента через делегированные отношения администратора и делегированное назначение доступа администратора.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|unifiedRoles|[Коллекция unifiedRole](../resources/unifiedrole.md)|Роли каталога, назначенные партнеру Майкрософт в клиенте клиента.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.delegatedAdminAccessDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.delegatedAdminAccessDetails",
  "unifiedRoles": [
    {
      "@odata.type": "microsoft.graph.unifiedRole"
    }
  ]
}
```

