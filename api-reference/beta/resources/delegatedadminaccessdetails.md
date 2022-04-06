---
title: delegatedAdminAccessDetails type
description: Представляет административные роли, которые партнер Майкрософт имеет в клиенте клиента через делегированную связь администратора и делегированную назначение доступа администратора.
author: adtangir
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: a817e2f0814c19c519475d6fe4c049036ca8c3d2
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589860"
---
# <a name="delegatedadminaccessdetails-resource-type"></a>delegatedAdminAccessDetails type

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет административные роли, которые партнер Майкрософт имеет в клиенте клиента через делегированную связь администратора и делегированную назначение доступа администратора.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|unifiedRoles|[коллекция unifiedRole](../resources/unifiedrole.md)|Роли каталога, назначенные партнеру Майкрософт в клиенте клиента.|

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

