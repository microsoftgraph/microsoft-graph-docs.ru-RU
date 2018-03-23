# <a name="update-androidmanagedappregistration"></a>Обновление объекта androidManagedAppRegistration

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Обновление свойств объекта [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md).
## <a name="prerequisites"></a>Предварительные условия
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementApps.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Тело запроса
В теле запроса добавьте представление объекта [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md) в формате JSON.

В приведенной ниже таблице указаны свойства, необходимые при создании объекта [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Дата и время создания. Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|lastSyncDateTime|DateTimeOffset|Дата и время последней синхронизации приложения со службой управления. Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|applicationVersion|String|Версия приложения. Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|managementSdkVersion|String|Версия пакета SDK для управления приложениями. Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|platformVersion|String|Версия операционной системы. Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|deviceType|String|Тип устройства узла. Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|deviceTag|String|Тег, который создан с использованием пакета SDK для управления приложениями и позволяет связать приложения, размещенные на одном устройстве. Мы не гарантируем, что приложения будут связаны во всех состояниях. Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|deviceName|String|Имя устройства узла. Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|flaggedReasons|Коллекция String|Нуль или более причин, по которым помечается регистрация приложения (например, приложение запускается на рутованном устройстве). Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md). Возможные значения: `none`, `rootedDevice`.|
|userId|String|Идентификатор пользователя, к которому относится эта регистрация приложения. Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|appIdentifier|[mobileAppIdentifier](../resources/intune_mam_mobileappidentifier.md)|Идентификатор пакета приложения. Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|id|String|Ключ объекта. Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|
|version|String|Версия объекта. Наследуется от объекта [managedAppRegistration](../resources/intune_mam_managedappregistration.md).|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md) в теле отклика.

## <a name="example"></a>Пример
### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
Content-type: application/json
Content-length: 577

{
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "applicationVersion": "Application Version value",
  "managementSdkVersion": "Management Sdk Version value",
  "platformVersion": "Platform Version value",
  "deviceType": "Device Type value",
  "deviceTag": "Device Tag value",
  "deviceName": "Device Name value",
  "flaggedReasons": [
    "rootedDevice"
  ],
  "userId": "User Id value",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "Package Id value"
  },
  "version": "Version value"
}
```

### <a name="response"></a>Ответ
Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 753

{
  "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "applicationVersion": "Application Version value",
  "managementSdkVersion": "Management Sdk Version value",
  "platformVersion": "Platform Version value",
  "deviceType": "Device Type value",
  "deviceTag": "Device Tag value",
  "deviceName": "Device Name value",
  "flaggedReasons": [
    "rootedDevice"
  ],
  "userId": "User Id value",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "Package Id value"
  },
  "id": "0e064997-4997-0e06-9749-060e9749060e",
  "version": "Version value"
}
```



