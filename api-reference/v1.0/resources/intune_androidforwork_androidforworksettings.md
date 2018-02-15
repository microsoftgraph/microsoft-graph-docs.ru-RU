# <a name="androidforworksettings-resource-type"></a>Тип ресурса androidForWorkSettings

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Параметры Android For Work.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение объекта androidForWorkSettings](../api/intune_androidforwork_androidforworksettings_get.md)|[androidForWorkSettings](../resources/intune_androidforwork_androidforworksettings.md)|Чтение свойств и связей объекта [androidForWorkSettings](../resources/intune_androidforwork_androidforworksettings.md).|
|[Обновление объекта androidForWorkSettings](../api/intune_androidforwork_androidforworksettings_update.md)|[androidForWorkSettings](../resources/intune_androidforwork_androidforworksettings.md)|Обновление свойств объекта [androidForWorkSettings](../resources/intune_androidforwork_androidforworksettings.md).|
|[Действие requestSignupUrl](../api/intune_androidforwork_androidforworksettings_requestsignupurl.md)|String|Создает URL-адрес для регистрации, с помощью которого можно записаться на управление Android for Work.|
|[completeSignup action](../api/intune_androidforwork_androidforworksettings_completesignup.md)|Нет|Завершает поток регистрации для управления Android for Work.|
|[Действие syncApps](../api/intune_androidforwork_androidforworksettings_syncapps.md)|Нет|Синхронизирует утвержденные приложения для предприятия.|
|[Действие unbind](../api/intune_androidforwork_androidforworksettings_unbind.md)|Нет|Отключает управление Android for Work для предприятия.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор параметров Android for Work|
|bindStatus|String|Состояние привязки клиента к API Google EMM. Возможные значения: `notBound`, `bound`, `boundAndValidated`, `unbinding`.|
|lastAppSyncDateTime|DateTimeOffset|Время завершения последней синхронизации приложения|
|lastAppSyncStatus|String|Результат последней синхронизации приложения. Возможные значения: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.|
|ownerUserPrincipalName|String|UPN владельца, создавшего предприятие|
|ownerOrganizationName|String|Имя организации, используемое при входящей миграции Android for Work|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения параметров Android for Work|
|enrollmentTarget|String|Указывает, какие пользователи могут регистрировать устройства для управления с помощью Android for Work. Возможные значения: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.|
|targetGroupIds|Коллекция строк|Указывает, какие группы AAD могут регистрировать устройства для управления с помощью Android for Work, если для параметра enrollmentTarget задано значение Targeted.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidForWorkSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkSettings",
  "id": "String (identifier)",
  "bindStatus": "String",
  "lastAppSyncDateTime": "String (timestamp)",
  "lastAppSyncStatus": "String",
  "ownerUserPrincipalName": "String",
  "ownerOrganizationName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "enrollmentTarget": "String",
  "targetGroupIds": [
    "String"
  ]
}
```



