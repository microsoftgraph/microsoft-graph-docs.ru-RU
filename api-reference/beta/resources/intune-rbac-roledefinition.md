---
title: Тип ресурса roleDefinition
description: 'Ресурс "Определение роли". Определение роли лежит в основе доступа на основе ролей в Intune. Роль сочетает в себе ресурс Intune, например мобильное приложение, и связанные разрешения роли для ресурса, такие как создание или чтение. Есть роли двух типов: встроенные и настраиваемые. Встроенные роли невозможно изменить. Как встроенные, так и настраиваемые роли должны включать применяемые назначения. Создайте настраиваемые роли, чтобы определить роль, которая позволяет объединить любые доступные ресурсы и разрешения роли.'
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c153ce5f0efde38f92684c688019e531d8c0a2b4
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58783178"
---
# <a name="roledefinition-resource-type"></a>Тип ресурса roleDefinition

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс "Определение роли". Определение роли лежит в основе доступа на основе ролей в Intune. Роль сочетает в себе ресурс Intune, например мобильное приложение, и связанные разрешения роли для ресурса, такие как создание или чтение. Есть роли двух типов: встроенные и настраиваемые. Встроенные роли невозможно изменить. Как встроенные, так и настраиваемые роли должны включать применяемые назначения. Создайте настраиваемые роли, чтобы определить роль, которая позволяет объединить любые доступные ресурсы и разрешения роли.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов roleDefinition](../api/intune-rbac-roledefinition-list.md)|Коллекция [roleDefinition](../resources/intune-rbac-roledefinition.md)|Список свойств и связей объектов [roleDefinition](../resources/intune-rbac-roledefinition.md).|
|[Получение объекта roleDefinition](../api/intune-rbac-roledefinition-get.md)|[roleDefinition](../resources/intune-rbac-roledefinition.md)|Чтение свойств и связей объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).|
|[Создание объекта roleDefinition](../api/intune-rbac-roledefinition-create.md)|[roleDefinition](../resources/intune-rbac-roledefinition.md)|Создание объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).|
|[Удаление объекта roleDefinition](../api/intune-rbac-roledefinition-delete.md)|Нет|Удаление объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).|
|[Обновление объекта roleDefinition](../api/intune-rbac-roledefinition-update.md)|[roleDefinition](../resources/intune-rbac-roledefinition.md)|Обновление свойств объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Это свойство доступно только для чтения и создается автоматически.|
|displayName|Строка|Отображаемое имя определения роли.|
|description|Строка|Описание определения роли.|
|permissions|Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)|Список разрешений, активированных для роли. Они должны соответствовать объекту actionName, который определен как часть rolePermission.|
|rolePermissions|Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)|Список разрешений, активированных для роли. Они должны соответствовать объекту actionName, который определен как часть rolePermission.|
|isBuiltInRoleDefinition|Boolean|Тип роли. Для встроенного определения роли задается значение True, а для настраиваемого — False.|
|isBuiltIn|Boolean|Тип роли. Для встроенного определения роли задается значение True, а для настраиваемого — False.|
|roleScopeTagIds|Коллекция String|Список тегов области для этого экземпляра Entity.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|roleAssignments|Коллекция объектов [roleAssignment](../resources/intune-rbac-roleassignment.md)|Список назначений ролей для определения роли.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleDefinition",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "permissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
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
  ],
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
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
  ],
  "isBuiltInRoleDefinition": true,
  "isBuiltIn": true,
  "roleScopeTagIds": [
    "String"
  ]
}
```



