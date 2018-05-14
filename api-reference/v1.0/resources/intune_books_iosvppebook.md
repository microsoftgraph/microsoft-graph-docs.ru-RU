# <a name="iosvppebook-resource-type"></a>Тип ресурса iosVppEBook

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Класс, содержащий свойства электронной книги VPP для iOS.

Наследуется от [managedEBook](../resources/intune_books_managedebook.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление iosVppEBooks](../api/intune_books_iosvppebook_list.md)|Коллекция [iosVppEBook](../resources/intune_books_iosvppebook.md)|Список свойств и связей объектов [iosVppEBook](../resources/intune_books_iosvppebook.md).|
|[Получение iosVppEBook](../api/intune_books_iosvppebook_get.md)|[iosVppEBook](../resources/intune_books_iosvppebook.md)|Считывание свойств и связей объекта [iosVppEBook](../resources/intune_books_iosvppebook.md).|
|[Создание iosVppEBook](../api/intune_books_iosvppebook_create.md)|[iosVppEBook](../resources/intune_books_iosvppebook.md)|Создание объекта [iosVppEBook](../resources/intune_books_iosvppebook.md).|
|[Удаление iosVppEBook](../api/intune_books_iosvppebook_delete.md)|None|Удаление экземпляра [iosVppEBook](../resources/intune_books_iosvppebook.md).|
|[Обновление iosVppEBook](../api/intune_books_iosvppebook_update.md)|[iosVppEBook](../resources/intune_books_iosvppebook.md)|Обновление свойств объекта [iosVppEBook](../resources/intune_books_iosvppebook.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от [managedEBook](../resources/intune_books_managedebook.md).|
|displayName|String|Имя электронной книги. Наследуется от [managedEBook](../resources/intune_books_managedebook.md).|
|description|String|Описание. Наследуется от [managedEBook](../resources/intune_books_managedebook.md).|
|publisher|String|Издатель. Наследуется от [managedEBook](../resources/intune_books_managedebook.md).|
|publishedDateTime|DateTimeOffset|Дата и время публикации электронной книги. Наследуется от [managedEBook](../resources/intune_books_managedebook.md).|
|largeCover|[mimeContent](../resources/intune_shared_mimecontent.md)|Обложка книги. Наследуется от [managedEBook](../resources/intune_books_managedebook.md).|
|createdDateTime|DateTimeOffset|Дата и время создания электронной книги. Наследуется от [managedEBook](../resources/intune_books_managedebook.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения электронной книги. Унаследован от объекта [managedEBook](../resources/intune_books_managedebook.md)|
|informationUrl|String|URL-адрес страницы с дополнительными сведениями. Наследуется от [managedEBook](../resources/intune_books_managedebook.md).|
|privacyInformationUrl|String|URL-адрес заявления о конфиденциальности. Наследуется от [managedEBook](../resources/intune_books_managedebook.md).|
|vppTokenId|Guid|Идентификатор токена VPP.|
|appleId|String|Идентификатор Apple ID, связанный с токеном VPP.|
|vppOrganizationName|String|Название организации для токена VPP.|
|genres|Коллекция String|Жанры.|
|language|String|Язык.|
|seller|String|Продавец.|
|totalLicenseCount|Int32|Общее число лицензий.|
|usedLicenseCount|Int32|Число используемых лицензий.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|Коллекция [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)|Список назначений для этой электронной книги. Наследуется от [managedEBook](../resources/intune_books_managedebook.md).|
|installSummary|[eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md)|Сводка по установке мобильного приложения. Наследуется от [managedEBook](../resources/intune_books_managedebook.md).|
|deviceStates|Коллекция [deviceInstallState](../resources/intune_books_deviceinstallstate.md)|Список состояний установки для этой электронной книги. Наследуется от [managedEBook](../resources/intune_books_managedebook.md).|
|userStateSummary|Коллекция [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md)|Список состояний установки для этой электронной книги. Наследуется от [managedEBook](../resources/intune_books_managedebook.md).|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosVppEBook"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppEBook",
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
  "privacyInformationUrl": "String",
  "vppTokenId": "<Unknown Primitive Type Edm.Guid>",
  "appleId": "String",
  "vppOrganizationName": "String",
  "genres": [
    "String"
  ],
  "language": "String",
  "seller": "String",
  "totalLicenseCount": 1024,
  "usedLicenseCount": 1024
}
```



