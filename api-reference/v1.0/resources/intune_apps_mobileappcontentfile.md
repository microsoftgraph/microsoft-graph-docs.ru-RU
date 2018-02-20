# <a name="mobileappcontentfile-resource-type"></a>Тип ресурса mobileAppContentFile

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Содержит свойства для одного файла установщика, связанного с заданной версией mobileAppContent.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление mobileAppContentFiles](../api/intune_apps_mobileappcontentfile_list.md)|Коллекция [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md)|Список свойств и связей объектов [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md).|
|[Получение mobileAppContentFile](../api/intune_apps_mobileappcontentfile_get.md)|[mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md)|Считывание свойств и связей объекта [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md).|
|[Создание mobileAppContentFile](../api/intune_apps_mobileappcontentfile_create.md)|[mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md)|Создание объекта [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md).|
|[Удаление mobileAppContentFile](../api/intune_apps_mobileappcontentfile_delete.md)|None|Удаление экземпляра [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md).|
|[Обновление mobileAppContentFile](../api/intune_apps_mobileappcontentfile_update.md)|[mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md)|Обновление свойств объекта [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md).|
|[Действие commit](../api/intune_apps_mobileappcontentfile_commit.md)|None|Подтверждает файл заданного приложения.|
|[Действие renewUpload](../api/intune_apps_mobileappcontentfile_renewupload.md)|None|Обновляет URI SAS для отправки файла приложения.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|azureStorageUri|String|URI службы хранилища Azure.|
|isCommitted|Boolean|Значение, указывающее, является ли файл подтвержденным.|
|id|String|Идентификатор файла.|
|createdDateTime|DateTimeOffset|Время создания файла.|
|name|String|Имя файла.|
|size|Int64|Размер файла до шифрования.|
|sizeEncrypted|Int64|Размер файла после шифрования.|
|azureStorageUriExpirationDateTime|DateTimeOffset|Время, когда заканчивается срок действия URI для службы хранилища Azure.|
|manifest|Binary|Данные манифеста.|
|uploadState|String|Состояние текущего запроса на отправку. Возможные значения: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.|

## <a name="relationships"></a>Связи
None
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppContentFile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppContentFile",
  "azureStorageUri": "String",
  "isCommitted": true,
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "name": "String",
  "size": 1024,
  "sizeEncrypted": 1024,
  "azureStorageUriExpirationDateTime": "String (timestamp)",
  "manifest": "binary",
  "uploadState": "String"
}
```



