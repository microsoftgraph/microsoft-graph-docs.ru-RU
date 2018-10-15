# <a name="resourceoperation-resource-type"></a>Тип ресурса resourceOperation

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Определяет операцию или действие, которые можно выполнять с ресурсом (или объектом) Intune.  Распространенные операции — чтение, удаление, обновление и создание.  Они обеспечивают основные возможности управления базовым ресурсом Intune.  В некоторых случаях ресурс Intune может включать операции, выполняемые в сочетании с другими ресурсами.  Например, операция Assign позволяет назначить ресурс MobileApp группе безопасности AAD.  Операции с ресурсами невозможно изменить для встроенных ролей. Это определяет операцию или действие, которые можно выполнить с ресурсом (или объектом) Intune.  Распространенные операции — получение, перечисление, обновление и создание.  Они обеспечивают основные возможности управления базовым ресурсом Intune.  В некоторых случаях ресурс Intune может включать операции, выполняемые в сочетании с другими ресурсами.  Например, операция Assign позволяет назначить ресурс MobileApp группе безопасности AAD.  Операции с ресурсами невозможно изменить для встроенных ролей.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов resourceOperation](../api/intune_rbac_resourceoperation_list.md)|Коллекция объектов [resourceOperation](../resources/intune_rbac_resourceoperation.md)|Список свойств и связей объектов [resourceOperation](../resources/intune_rbac_resourceoperation.md).|
|[Получение объекта resourceOperation](../api/intune_rbac_resourceoperation_get.md)|[resourceOperation](../resources/intune_rbac_resourceoperation.md)|Чтение свойств и связей объекта [resourceOperation](../resources/intune_rbac_resourceoperation.md).|
|[Создание объекта resourceOperation](../api/intune_rbac_resourceoperation_create.md)|[resourceOperation](../resources/intune_rbac_resourceoperation.md)|Создание объекта [resourceOperation](../resources/intune_rbac_resourceoperation.md).|
|[Удаление объекта resourceOperation](../api/intune_rbac_resourceoperation_delete.md)|Нет|Удаление объекта [resourceOperation](../resources/intune_rbac_resourceoperation.md).|
|[Обновление объекта resourceOperation](../api/intune_rbac_resourceoperation_update.md)|[resourceOperation](../resources/intune_rbac_resourceoperation.md)|Обновление свойств объекта [resourceOperation](../resources/intune_rbac_resourceoperation.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|ид|Строка|Ключ операции с ресурсом. Доступен только для чтения и создается автоматически.|
|resourceName|Строка|Имя ресурса, с которым выполняется эта операция.|
|actionName|Строка|Тип действия, которое выполнит эта операция. Свойство actionName должно быть максимально кратким (только несколько слов).|
|описание|Строка|Описание операции с ресурсом. Используется в тексте, который отображается над операцией при наведении указателя мыши на портале Azure.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.resourceOperation"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceOperation",
  "id": "String (identifier)",
  "resourceName": "String",
  "actionName": "String",
  "description": "String"
}
```








