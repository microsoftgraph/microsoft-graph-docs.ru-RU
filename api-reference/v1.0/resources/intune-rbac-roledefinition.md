---
title: Тип ресурса roleDefinition
description: 'Ресурс "Определение роли". Определение роли лежит в основе доступа на основе ролей в Intune. Роль сочетает в себе ресурс Intune, например мобильное приложение, и связанные разрешения роли для ресурса, такие как создание или чтение. Есть роли двух типов: встроенные и настраиваемые. Встроенные роли невозможно изменить. Как встроенные, так и настраиваемые роли должны включать применяемые назначения. Создайте настраиваемые роли, чтобы определить роль, которая позволяет объединить любые доступные ресурсы и разрешения роли.'
localization_priority: Normal
ms.openlocfilehash: d3f5ef8ddd67302b747b2f35b0e4f62f3f6c00d2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804818"
---
# <a name="roledefinition-resource-type"></a>Тип ресурса roleDefinition

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

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
|displayName|String|Отображаемое имя определения роли.|
|описание|String|Описание определения роли.|
|rolePermissions|Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)|Список разрешений, активированных для роли. Они должны соответствовать объекту actionName, который определен как часть rolePermission.|
|isBuiltIn|Boolean|Тип роли. Для встроенного определения роли задается значение True, а для настраиваемого — False.|

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
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
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
  "isBuiltIn": true
}
```



