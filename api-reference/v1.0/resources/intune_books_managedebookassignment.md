# <a name="managedebookassignment-resource-type"></a>Тип ресурса managedEBookAssignment

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Содержит свойства, используемые при назначении электронной книги группе.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов managedEBookAssignment](../api/intune_books_managedebookassignment_list.md)|Коллекция [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)|Список свойств и связей объектов [managedEBookAssignment](../resources/intune_books_managedebookassignment.md).|
|[Получение объекта managedEBookAssignment](../api/intune_books_managedebookassignment_get.md)|[managedEBookAssignment](../resources/intune_books_managedebookassignment.md)|Чтение свойств и связей объекта [managedEBookAssignment](../resources/intune_books_managedebookassignment.md).|
|[Создание объекта managedEBookAssignment](../api/intune_books_managedebookassignment_create.md)|[managedEBookAssignment](../resources/intune_books_managedebookassignment.md)|Создание объекта [managedEBookAssignment](../resources/intune_books_managedebookassignment.md).|
|[Удаление объекта managedEBookAssignment](../api/intune_books_managedebookassignment_delete.md)|Нет|Удаляет объект [managedEBookAssignment](../resources/intune_books_managedebookassignment.md).|
|[Обновление объекта managedEBookAssignment](../api/intune_books_managedebookassignment_update.md)|[managedEBookAssignment](../resources/intune_books_managedebookassignment.md)|Обновление свойств объекта [managedEBookAssignment](../resources/intune_books_managedebookassignment.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|Цель назначения электронной книги.|
|installIntent|[installIntent](../resources/intune_shared_installintent.md)|Цель установки электронной книги. Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedEBookAssignment"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "String"
}
```








