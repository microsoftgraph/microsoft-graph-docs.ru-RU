# <a name="androidmanagedappregistration-resource-type"></a>Тип ресурса androidManagedAppRegistration

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Представляет собой сведения о синхронизации управляемого приложения Android для определенного пользователя.
Ресурс ManagedAppRegistration представляет собой сведения об управляемом приложении, используемом членом организации.

Наследуется от [managedAppRegistration](../resources/intune_mam_managedappregistration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление androidManagedAppRegistrations](../api/intune_mam_androidmanagedappregistration_list.md)|Коллекция [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md)|Список свойств и связей объектов [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md).|
|[Получение androidManagedAppRegistration](../api/intune_mam_androidmanagedappregistration_get.md)|[androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md)|Считывание свойств и связей объекта [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md).|
|[Создание androidManagedAppRegistration](../api/intune_mam_androidmanagedappregistration_create.md)|[androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md)|Создание нового объекта [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md).|
|[Удаление androidManagedAppRegistration](../api/intune_mam_androidmanagedappregistration_delete.md)|None|Удаление экземпляра [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md).|
|[Обновление androidManagedAppRegistration](../api/intune_mam_androidmanagedappregistration_update.md)|[androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md)|Обновление свойств объекта [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Дата и время создания. Наследуется от [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|lastSyncDateTime|DateTimeOffset|Дата и время последней синхронизации приложения со службой управления. Наследуется от [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|applicationVersion|String|Версия приложения. Наследуется от [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|managementSdkVersion|String|Версия пакета SDK для управления приложениями. Наследуется от [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|platformVersion|String|Версия операционной системы. Наследуется от [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|deviceType|String|Тип устройства узла. Наследуется от [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|deviceTag|String|Тег, который создан с использованием пакета SDK для управления приложениями и позволяет связать приложения, размещенные на одном устройстве. Мы не гарантируем, что приложения будут связаны во всех состояниях. Наследуется от [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|deviceName|String|Имя устройства узла. Наследуется от [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|flaggedReasons|Коллекция String|Нуль или более причин, по которым помечается регистрация приложения. Пример: приложение запускается на рутованном устройстве. Наследуется от [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|userId|String|ИД пользователя, к которому относится эта регистрация приложения. Наследуется от [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|appIdentifier|[mobileAppIdentifier](../resources/intune_mam_mobileappidentifier.md)|Идентификатор пакета приложения. Наследуется от [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|id|String|Ключ объекта. Наследуется от [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|version|String|Версия объекта. Наследуется от [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|appliedPolicies|Коллекция [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|Нуль или более политик, примененных к зарегистрированному приложению, когда оно в последний раз синхронизировалось со службой управления. Наследуется от [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|intendedPolicies|Коллекция [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|Нуль или более политик, которые на текущий момент администратор использует для приложения. Наследуется от [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|operations|Коллекция [managedAppOperation](../resources/intune_mam_managedappoperation.md)|Нуль или более долговременных операций, запускаемых для регистрации приложения. Наследуется от [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidManagedAppRegistration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
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
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "String"
  },
  "id": "String (identifier)",
  "version": "String"
}
```



