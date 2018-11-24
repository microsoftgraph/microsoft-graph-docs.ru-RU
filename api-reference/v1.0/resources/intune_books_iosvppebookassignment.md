# <a name="iosvppebookassignment-resource-type"></a>Тип ресурса iosVppEBookAssignment

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Содержит свойства, используемые при назначении электронной книги в формате VPP для iOS группе.

Наследуется от [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов iosVppEBookAssignment](../api/intune_books_iosvppebookassignment_list.md)|Коллекция [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md)|Список свойств и связей объектов [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md).|
|[Получение объекта iosVppEBookAssignment](../api/intune_books_iosvppebookassignment_get.md)|[iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md)|Чтение свойств и связей объекта [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md).|
|[Создание объекта iosVppEBookAssignment](../api/intune_books_iosvppebookassignment_create.md)|[iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md)|Создание объекта [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md).|
|[Удаление объекта iosVppEBookAssignment](../api/intune_books_iosvppebookassignment_delete.md)|Нет|Удаляет объект [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md).|
|[Обновление объекта iosVppEBookAssignment](../api/intune_books_iosvppebookassignment_update.md)|[iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md)|Обновление свойств объекта [iosVppEBookAssignment](../resources/intune_books_iosvppebookassignment.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от объекта [managedEBookAssignment](../resources/intune_books_managedebookassignment.md).|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|Цель назначения электронной книги. Наследуется от объекта [managedEBookAssignment](../resources/intune_books_managedebookassignment.md).|
|installIntent|[installIntent](../resources/intune_shared_installintent.md)|Цель установки электронной книги. Наследуется от [managedEBookAssignment](../resources/intune_books_managedebookassignment.md). Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.|

## <a name="relationships"></a>Связи
None
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosVppEBookAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppEBookAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "String"
}
```



