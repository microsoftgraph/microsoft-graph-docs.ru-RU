---
title: Тип ресурса rolePermission
description: Содержит набор Ресаурцеактионс, определяющих разрешения "разрешено" и "не разрешено" для каждой роли.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8cbe41bae81d165d0800a5184e1f7babedebc09d
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993524"
---
# <a name="rolepermission-resource-type"></a>Тип ресурса rolePermission

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит набор Ресаурцеактионс, определяющих разрешения "разрешено" и "не разрешено" для каждой роли.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|actions|Коллекция строк|Разрешенные действия — устарело|
|resourceActions|Коллекция объектов [resourceAction](../resources/intune-rbac-resourceaction.md)|Действия с ресурсами, содержащие набор разрешенных и запрещенных разрешений.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.rolePermission"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rolePermission",
  "actions": [
    "String"
  ],
  "resourceActions": [
    {
      "@odata.type": "microsoft.graph.resourceAction",
      "allowedResourceActions": [
        "String"
      ],
      "notAllowedResourceActions": [
        "String"
      ]
    }
  ]
}
```





