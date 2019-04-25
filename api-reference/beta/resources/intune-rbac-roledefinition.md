---
title: Тип ресурса roleDefinition
description: 'Ресурс "Определение роли". Определение роли лежит в основе доступа на основе ролей в Intune. Роль сочетает в себе ресурс Intune, например мобильное приложение, и связанные разрешения роли для ресурса, такие как создание или чтение. Есть роли двух типов: встроенные и настраиваемые. Встроенные роли невозможно изменить. Как встроенные, так и настраиваемые роли должны включать применяемые назначения. Создайте настраиваемые роли, чтобы определить роль, которая позволяет объединить любые доступные ресурсы и разрешения роли.'
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fca5f91c5ca708f715b1438f2fe8508060e3b91c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566334"
---
# <a name="roledefinition-resource-type"></a>Тип ресурса roleDefinition

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс "Определение роли". Определение роли лежит в основе доступа на основе ролей в Intune. Роль сочетает в себе ресурс Intune, например мобильное приложение, и связанные разрешения роли для ресурса, такие как создание или чтение. Есть роли двух типов: встроенные и настраиваемые. Встроенные роли невозможно изменить. Как встроенные, так и настраиваемые роли должны включать применяемые назначения. Создайте настраиваемые роли, чтобы определить роль, которая позволяет объединить любые доступные ресурсы и разрешения роли.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов roleDefinition](../api/intune-rbac-roledefinition-list.md)|Коллекция [roleDefinition](../resources/intune-rbac-roledefinition.md)|Список свойств и связей объектов [roleDefinition](../resources/intune-rbac-roledefinition.md).|
|[Получение объекта roleDefinition](../api/intune-rbac-roledefinition-get.md)|[roleDefinition](../resources/intune-rbac-roledefinition.md);|Чтение свойств и связей объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).|
|[Создание объекта roleDefinition](../api/intune-rbac-roledefinition-create.md)|[roleDefinition](../resources/intune-rbac-roledefinition.md);|Создание объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).|
|[Удаление объекта roleDefinition](../api/intune-rbac-roledefinition-delete.md)|Нет|Удаление объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).|
|[Обновление объекта roleDefinition](../api/intune-rbac-roledefinition-update.md)|[roleDefinition](../resources/intune-rbac-roledefinition.md)|Обновление свойств объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Это свойство доступно только для чтения и создается автоматически.|
|displayName|String|Отображаемое имя определения роли.|
|description|String|Описание определения роли.|
|permissions|Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)|Список разрешений, активированных для роли. Они должны соответствовать объекту actionName, который определен как часть rolePermission.|
|rolePermissions|Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)|Список разрешений, активированных для роли. Они должны соответствовать объекту actionName, который определен как часть rolePermission.|
|Исбуилтинроледефинитион|Boolean|Тип роли. Для встроенного определения роли задается значение True, а для настраиваемого — False.|
|isBuiltIn|Boolean|Тип роли. Для встроенного определения роли задается значение True, а для настраиваемого — False.|
|roleScopeTagIds|Коллекция String|Список тегов областей для этого экземпляра сущности.|

## <a name="relationships"></a>Связи
|Отношение|Тип|Описание|
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





