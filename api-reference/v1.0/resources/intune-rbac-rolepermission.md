---
title: Тип ресурса rolePermission
description: Содержит набор ResourceActions, определяющий разрешенные и не разрешенные разрешения для каждой роли.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 308443ae14e1069a3196a9cd41d3a0e7ba9dc25f
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2021
ms.locfileid: "60448964"
---
# <a name="rolepermission-resource-type"></a>Тип ресурса rolePermission

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит набор ResourceActions, определяющий разрешенные и не разрешенные разрешения для каждой роли.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|resourceActions|Коллекция объектов [resourceAction](../resources/intune-rbac-resourceaction.md)|Действия ресурса, каждый из которых содержит набор разрешенных и не разрешенных разрешений.|

## <a name="relationships"></a>Связи
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



