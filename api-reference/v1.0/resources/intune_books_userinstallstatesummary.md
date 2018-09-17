# <a name="userinstallstatesummary-resource-type"></a>Тип ресурса userInstallStateSummary

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Содержит свойства сводки по состоянию установки для пользователя.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов userInstallStateSummary](../api/intune_books_userinstallstatesummary_list.md)|Коллекция [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md)|Список свойств и связей объектов [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md).|
|[Получение объекта userInstallStateSummary](../api/intune_books_userinstallstatesummary_get.md)|[userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md)|Чтение свойств и связей объекта [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md).|
|[Создание объекта userInstallStateSummary](../api/intune_books_userinstallstatesummary_create.md)|[userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md)|Создание объекта [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md).|
|[Удаление объекта userInstallStateSummary](../api/intune_books_userinstallstatesummary_delete.md)|Нет|Удаляет объект [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md).|
|[Обновление объекта userInstallStateSummary](../api/intune_books_userinstallstatesummary_update.md)|[userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md)|Обновление свойств объекта [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|ИД|Строка|Ключ объекта.|
|userName|Строка|Имя пользователя.|
|installedDeviceCount|Int32|Количество установленных устройств.|
|failedDeviceCount|Int32|Количество устройств со сбоями.|
|notInstalledDeviceCount|Int32|Количество не установленных устройств.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|deviceStates|Коллекция [deviceInstallState](../resources/intune_books_deviceinstallstate.md)|Состояние установки электронной книги.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userInstallStateSummary"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.userInstallStateSummary",
  "id": "String (identifier)",
  "userName": "String",
  "installedDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "notInstalledDeviceCount": 1024
}
```








