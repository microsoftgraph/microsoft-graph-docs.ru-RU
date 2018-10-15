# <a name="managedappregistration-resource-type"></a>Тип ресурса managedAppRegistration

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

ManagedAppEntity — это базовый тип для всех остальных типов объектов в рабочем процессе управления приложениями.
Ресурс ManagedAppRegistration представляет собой сведения об управляемом приложении, используемом членом организации.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов managedAppRegistration](../api/intune_mam_managedappregistration_list.md)|Коллекция объектов [managedAppRegistration](../resources/intune_mam_managedappregistration.md)|Список свойств и связей объектов [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|[Получение объекта managedAppRegistration](../api/intune_mam_managedappregistration_get.md)|[managedAppRegistration](../resources/intune_mam_managedappregistration.md)|Чтение свойств и связей объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|[Функция getUserIdsWithFlaggedAppRegistration](../api/intune_mam_managedappregistration_getuseridswithflaggedappregistration.md)|Коллекция объектов string|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Дата и время создания.|
|lastSyncDateTime|DateTimeOffset|Дата и время последней синхронизации приложения со службой управления.|
|applicationVersion|String (строка)|Версия приложения.|
|managementSdkVersion|String (строка)|Версия пакета SDK для управления приложениями.|
|platformVersion|String (строка)|Версия операционной системы.|
|deviceType|String (строка)|Тип главного устройства.|
|deviceTag|String (строка)|Тег, который создан с использованием пакета SDK для управления приложениями и помогает связывать приложения, размещенные на одном устройстве. Мы не гарантируем, что приложения будут связаны во всех состояниях.|
|deviceName|String (строка)|Имя главного устройства.|
|flaggedReasons|Коллекция [managedAppFlaggedReason](../resources/intune_mam_managedappflaggedreason.md)|Причины, по которым помечается регистрация приложения (если они есть). например приложения, запущенного на устройстве с административным доступом.|
|userId|String (строка)|ИД пользователя, к которому относится эта регистрация приложения.|
|appIdentifier|[mobileAppIdentifier](../resources/intune_mam_mobileappidentifier.md)|Идентификатор пакета приложения.|
|id|Строка|Ключ объекта.|
|version|String (строка)|Версия объекта.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|appliedPolicies|Коллекция объектов [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|Нуль или более политик, примененных к зарегистрированному приложению, когда оно в последний раз синхронизировалось со службой управления.|
|intendedPolicies|Коллекция объектов [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|Нуль или более политик, которые на текущий момент администратор использует для приложения.|
|operations|Коллекция объектов [managedAppOperation](../resources/intune_mam_managedappoperation.md)|Нуль или более долговременных операций, запускаемых для регистрации приложения.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppRegistration"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppRegistration",
  "createdDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "applicationVersion": "String",
  "managementSdkVersion": "String",
  "platformVersion": "String",
  "deviceType": "String",
  "deviceTag": "String",
  "deviceName": "String",
  "flaggedReasons": [
    "String"
  ],
  "userId": "String",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "id": "String (identifier)",
  "version": "String"
}
```








