# <a name="roleassignment-resource-type"></a>Тип ресурса roleAssignment

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Ресурс назначения роли. Назначения ролей объединяют определение роли с участниками и областями. Одной роли может соответствовать одно или несколько назначений. Это относится как к пользовательским, так и ко встроенным ролям.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов roleAssignment](../api/intune_rbac_roleassignment_list.md)|Коллекция объектов [roleAssignment](../resources/intune_rbac_roleassignment.md)|Список свойств и связей объектов [roleAssignment](../resources/intune_rbac_roleassignment.md).|
|[Получение объекта roleAssignment](../api/intune_rbac_roleassignment_get.md)|[roleAssignment](../resources/intune_rbac_roleassignment.md)|Чтение свойств и связей объекта [roleAssignment](../resources/intune_rbac_roleassignment.md).|
|[Создание объекта roleAssignment](../api/intune_rbac_roleassignment_create.md)|[roleAssignment](../resources/intune_rbac_roleassignment.md)|Создание объекта [roleAssignment](../resources/intune_rbac_roleassignment.md).|
|[Удаление объекта roleAssignment](../api/intune_rbac_roleassignment_delete.md)|Нет|Удаляет объект [roleAssignment](../resources/intune_rbac_roleassignment.md).|
|[Обновление объекта roleAssignment](../api/intune_rbac_roleassignment_update.md)|[roleAssignment](../resources/intune_rbac_roleassignment.md)|Обновление свойств объекта [roleAssignment](../resources/intune_rbac_roleassignment.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Это свойство доступно только для чтения и создается автоматически.|
|displayName|String|Отображаемое или понятное имя назначения роли.|
|description|String|Описание назначения роли.|
|resourceScopes|Коллекция String|Список идентификаторов групп безопасности с элементами области применения ролей.  Эти идентификаторы берутся из Azure Active Directory.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|roleDefinition|[roleDefinition](../resources/intune_rbac_roledefinition.md)|Определение роли, частью которого является это назначение.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.roleAssignment"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "resourceScopes": [
    "String"
  ]
}
```



