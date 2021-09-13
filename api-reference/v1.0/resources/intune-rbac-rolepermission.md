---
title: Тип ресурса rolePermission
description: Содержит набор ResourceActions, определяющий разрешенные и не разрешенные разрешения для каждой роли.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: da71e58f953fc1a0f23dc0f0944ea0f1a7564050
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59126788"
---
# <a name="rolepermission-resource-type"></a>Тип ресурса rolePermission

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит набор ResourceActions, определяющий разрешенные и не разрешенные разрешения для каждой роли.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|resourceActions|Коллекция объектов [resourceAction](../resources/intune-rbac-resourceaction.md)|Действия ресурса, каждый из которых содержит набор разрешенных и не разрешенных разрешений.|

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




