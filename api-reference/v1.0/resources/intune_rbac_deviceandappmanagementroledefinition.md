# <a name="deviceandappmanagementroledefinition-resource-type"></a>Тип ресурса deviceAndAppManagementRoleDefinition

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Ресурс "Определение роли". Определение роли лежит в основе доступа на основе ролей в Intune. Роль сочетает в себе ресурс Intune, например мобильное приложение, и связанные разрешения роли для ресурса, такие как создание или чтение. Есть роли двух типов: встроенные и настраиваемые. Встроенные роли невозможно изменить. Как встроенные, так и настраиваемые роли должны включать применяемые назначения. Создайте настраиваемые роли, чтобы определить роль, которая позволяет объединить любые доступные ресурсы и разрешения роли.

Наследуется от [roleDefinition](../resources/intune_rbac_roledefinition.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление deviceAndAppManagementRoleDefinitions](../api/intune_rbac_deviceandappmanagementroledefinition_list.md)|Коллекция [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md)|Список свойств и связей объектов [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md).|
|[Получение deviceAndAppManagementRoleDefinition](../api/intune_rbac_deviceandappmanagementroledefinition_get.md)|[deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md)|Считывание свойств и связей объекта [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md).|
|[Создание deviceAndAppManagementRoleDefinition](../api/intune_rbac_deviceandappmanagementroledefinition_create.md)|[deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md)|Создание объекта [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md).|
|[Удаление deviceAndAppManagementRoleDefinition](../api/intune_rbac_deviceandappmanagementroledefinition_delete.md)|Нет|Удаление экземпляра [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md).|
|[Обновление deviceAndAppManagementRoleDefinition](../api/intune_rbac_deviceandappmanagementroledefinition_update.md)|[deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md)|Обновление свойств объекта [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Это свойство доступно только для чтения и создается автоматически. Наследуется от объекта [roleDefinition](../resources/intune_rbac_roledefinition.md).|
|displayName|Строка​|Отображаемое имя определения роли. Наследуется от объекта [roleDefinition](../resources/intune_rbac_roledefinition.md).|
|description|Строка​|Описание определения роли. Наследуется от объекта [roleDefinition](../resources/intune_rbac_roledefinition.md).|
|rolePermissions|Коллекция [rolePermission](../resources/intune_rbac_rolepermission.md)|Список разрешений, активированных для роли. Они должны соответствовать объекту actionName, который определен как часть rolePermission. Наследуется от объекта [roleDefinition](../resources/intune_rbac_roledefinition.md).|
|isBuiltIn|Логический|Тип роли. Для встроенного определения роли задается значение True, а для настраиваемого — False. Наследуется от [roleDefinition](../resources/intune_rbac_roledefinition.md).|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|roleAssignments|Коллекция объектов [roleAssignment](../resources/intune_rbac_roleassignment.md)|Список назначений ролей для определения роли. Наследуется от [roleDefinition](../resources/intune_rbac_roledefinition.md).|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.roleDefinition",
  "@odata.type": "microsoft.graph.deviceAndAppManagementRoleDefinition"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
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



