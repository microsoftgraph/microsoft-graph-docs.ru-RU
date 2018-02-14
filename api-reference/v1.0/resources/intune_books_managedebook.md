# <a name="managedebook-resource-type"></a>Тип ресурса managedEBook

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Абстрактный класс, содержащий базовые свойства управляемой электронной книги.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список managedEBooks](../api/intune_books_managedebook_list.md)|Коллекция [managedEBook](../resources/intune_books_managedebook.md)|Список свойств и связей объектов [managedEBook](../resources/intune_books_managedebook.md).|
|[Получение объекта managedEBook](../api/intune_books_managedebook_get.md)|[managedEBook](../resources/intune_books_managedebook.md)|Чтение свойств и связей объекта [managedEBook](../resources/intune_books_managedebook.md).|
|[действие назначения](../api/intune_books_managedebook_assign.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|displayName|String|Имя электронной книги.|
|description|String|Описание.|
|publisher|String|Издатель.|
|publishedDateTime|DateTimeOffset|Дата и время публикации электронной книги.|
|largeCover|[mimeContent](../resources/intune_books_mimecontent.md)|Обложка книги.|
|createdDateTime|DateTimeOffset|Дата и время создания электронной книги.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения электронной книги.|
|informationUrl|String|URL-адрес с дополнительными сведениями.|
|privacyInformationUrl|String|URL-адрес заявления о конфиденциальности.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|Коллекция [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)|Список назначений для этой электронной книги.|
|installSummary|[eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md)|Общие сведения по установке мобильного приложения.|
|deviceStates|Коллекция [deviceInstallState](../resources/intune_books_deviceinstallstate.md)|Список состояний установки для этой электронной книги.|
|userStateSummary|Коллекция [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md)|Список состояний установки для этой электронной книги.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedEBook"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBook",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "publishedDateTime": "String (timestamp)",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "informationUrl": "String",
  "privacyInformationUrl": "String"
}
```



