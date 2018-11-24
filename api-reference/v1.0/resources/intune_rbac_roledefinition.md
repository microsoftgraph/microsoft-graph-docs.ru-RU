# <a name="roledefinition-resource-type"></a>Тип ресурса roleDefinition

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Ресурс "Определение роли". Определение роли лежит в основе доступа на основе ролей в Intune. Роль сочетает в себе ресурс Intune, например мобильное приложение, и связанные разрешения роли для ресурса, такие как создание или чтение. Есть роли двух типов: встроенные и настраиваемые. Встроенные роли невозможно изменить. Как встроенные, так и настраиваемые роли должны включать применяемые назначения. Создайте настраиваемые роли, чтобы определить роль, которая позволяет объединить любые доступные ресурсы и разрешения роли.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов roleDefinition](../api/intune_rbac_roledefinition_list.md)|Коллекция [roleDefinition](../resources/intune_rbac_roledefinition.md)|Список свойств и связей объектов [roleDefinition](../resources/intune_rbac_roledefinition.md).|
|[Получение объекта roleDefinition](../api/intune_rbac_roledefinition_get.md)|[roleDefinition](../resources/intune_rbac_roledefinition.md)|Чтение свойств и связей объекта [roleDefinition](../resources/intune_rbac_roledefinition.md).|
|[Создание объекта roleDefinition](../api/intune_rbac_roledefinition_create.md)|[roleDefinition](../resources/intune_rbac_roledefinition.md)|Создание объекта [roleDefinition](../resources/intune_rbac_roledefinition.md).|
|[Удаление объекта roleDefinition](../api/intune_rbac_roledefinition_delete.md)|Нет|Удаление объекта [roleDefinition](../resources/intune_rbac_roledefinition.md).|
|[Обновление объекта roleDefinition](../api/intune_rbac_roledefinition_update.md)|[roleDefinition](../resources/intune_rbac_roledefinition.md)|Обновление свойств объекта [roleDefinition](../resources/intune_rbac_roledefinition.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Это свойство доступно только для чтения и создается автоматически.|
|displayName|String|Отображаемое имя определения роли.|
|description|String|Описание определения роли.|
|rolePermissions|Коллекция объектов [rolePermission](../resources/intune_rbac_rolepermission.md)|Список разрешений, активированных для роли. Они должны соответствовать объекту actionName, который определен как часть rolePermission.|
|isBuiltIn|Boolean|Тип роли. Для встроенного определения роли задается значение True, а для настраиваемого — False.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|roleAssignments|Коллекция объектов [roleAssignment](../resources/intune_rbac_roleassignment.md)|Список назначений ролей для определения роли.|

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



