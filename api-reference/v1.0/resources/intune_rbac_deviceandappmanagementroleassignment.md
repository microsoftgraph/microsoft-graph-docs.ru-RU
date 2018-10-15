# <a name="deviceandappmanagementroleassignment-resource-type"></a>Тип ресурса deviceAndAppManagementRoleAssignment

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Ресурс назначения роли. Назначения ролей объединяют определение роли с участниками и областями. Одной роли может соответствовать одно или несколько назначений. Это относится как к настраиваемым, так и ко встроенным ролям.

Наследуется от объекта [roleAssignment](../resources/intune_rbac_roleassignment.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов deviceAndAppManagementRoleAssignment](../api/intune_rbac_deviceandappmanagementroleassignment_list.md)|Коллекция объектов [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md)|Список свойств и связей объектов [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md).|
|[Получение объекта deviceAndAppManagementRoleAssignment](../api/intune_rbac_deviceandappmanagementroleassignment_get.md)|[deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md)|Чтение свойств и связей объекта [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md).|
|[Создание объекта deviceAndAppManagementRoleAssignment](../api/intune_rbac_deviceandappmanagementroleassignment_create.md)|[deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md)|Создание объекта [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md).|
|[Удаление объекта deviceAndAppManagementRoleAssignment](../api/intune_rbac_deviceandappmanagementroleassignment_delete.md)|Нет|Удаление объекта [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md).|
|[Обновление объекта deviceAndAppManagementRoleAssignment](../api/intune_rbac_deviceandappmanagementroleassignment_update.md)|[deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md)|Обновление свойств объекта [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Это свойство доступно только для чтения и создается автоматически. Наследуется от объекта [roleAssignment](../resources/intune_rbac_roleassignment.md).|
|displayName|String (строка)|Отображаемое или понятное имя назначения роли. Наследуется от объекта [roleAssignment](../resources/intune_rbac_roleassignment.md).|
|description|String (строка)|Описание назначения роли. Наследуется от объекта [roleAssignment](../resources/intune_rbac_roleassignment.md).|
|resourceScopes|Коллекция String|Список идентификаторов групп безопасности с элементами области применения ролей.  Эти идентификаторы берутся из Azure Active Directory. Наследуется от объекта [roleAssignment](../resources/intune_rbac_roleassignment.md).|
|members|Коллекция String|Список идентификаторов групп безопасности с элементами ролей. Эти идентификаторы берутся из Azure Active Directory.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|roleDefinition|[roleDefinition](../resources/intune_rbac_roledefinition.md)|Определение роли, частью которого является это назначение. Наследуется от объекта [roleAssignment](../resources/intune_rbac_roleassignment.md).|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.roleAssignment",
  "@odata.type": "microsoft.graph.deviceAndAppManagementRoleAssignment"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "resourceScopes": [
    "String"
  ],
  "members": [
    "String"
  ]
}
```



