---
title: Тип ресурса rolePermission
description: Содержит набор ResourceActions, определяющий разрешенные и не разрешенные разрешения для каждой роли.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ec9fe67ab7cf3af5071f20cddf0775b70d84eddb83d14ef93aa3a376fab7a53a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54192308"
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




