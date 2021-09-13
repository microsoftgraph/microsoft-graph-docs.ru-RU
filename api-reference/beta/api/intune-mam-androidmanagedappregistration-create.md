---
title: Создание объекта androidManagedAppRegistration
description: Создание объекта androidManagedAppRegistration.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 26cb767ae744866da8924c7e0206e1aae5e02dc9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59065150"
---
# <a name="create-androidmanagedappregistration"></a>Создание объекта androidManagedAppRegistration

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание объекта [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md).

## <a name="prerequisites"></a>Предварительные условия
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementApps.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementApps.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса добавьте представление объекта androidManagedAppRegistration в формате JSON.

В приведенной ниже таблице указаны свойства, необходимые при создании объекта androidManagedAppRegistration.

|Свойство|Тип|Описание|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Дата и время создания. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|lastSyncDateTime|DateTimeOffset|Дата и время последней синхронизации приложения со службой управления. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|applicationVersion|String|Версия приложения. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|managementSdkVersion|String|Версия пакета SDK для управления приложениями. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|platformVersion|String|Версия операционной системы. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|deviceType|String|Тип устройства узла. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|deviceTag|String|Тег, который создан с использованием пакета SDK для управления приложениями и позволяет связать приложения, размещенные на одном устройстве. Мы не гарантируем, что приложения будут связаны во всех состояниях. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|deviceName|String|Имя устройства узла. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|managedDeviceId|String|Идентификатор управляемого устройства хост-устройства. Значение может быть пустым даже при управляемом устройстве хост-устройства. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|azureADDeviceId|String|Идентификатор Azure Active Directory устройства хост-устройства. Значение может быть пустым даже при регистрации Azure Active Directory устройства. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|deviceModel|String|Модель устройства для текущей регистрации приложений, унаследованной от [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|deviceManufacturer|Строка|Производитель устройств для текущей регистрации приложений, унаследованных от [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|flaggedReasons|[коллекция managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)|Нуль или более причин, по которым помечается регистрация приложения (например, приложение, запущенное на корневом устройстве, унаследовано от [управляемогоAppRegistration](../resources/intune-mam-managedappregistration.md). Возможные значения: `none`, `rootedDevice`, `androidBootloaderUnlocked`, `androidFactoryRomModified`.|
|userId|String|Идентификатор пользователя, к которому относится эта регистрация приложения. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|appIdentifier|[mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)|Идентификатор пакета приложения. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|id|String|Ключ объекта. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|version|String|Версия объекта. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|patchVersion|Строка|Версия патча для текущей регистрации android-приложений|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) в теле отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations
Content-type: application/json
Content-length: 879

{
  "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "applicationVersion": "Application Version value",
  "managementSdkVersion": "Management Sdk Version value",
  "platformVersion": "Platform Version value",
  "deviceType": "Device Type value",
  "deviceTag": "Device Tag value",
  "deviceName": "Device Name value",
  "managedDeviceId": "Managed Device Id value",
  "azureADDeviceId": "Azure ADDevice Id value",
  "deviceModel": "Device Model value",
  "deviceManufacturer": "Device Manufacturer value",
  "flaggedReasons": [
    "rootedDevice"
  ],
  "userId": "User Id value",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "Package Id value"
  },
  "version": "Version value",
  "patchVersion": "Patch Version value"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 987

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
  "managedDeviceId": "Managed Device Id value",
  "azureADDeviceId": "Azure ADDevice Id value",
  "deviceModel": "Device Model value",
  "deviceManufacturer": "Device Manufacturer value",
  "flaggedReasons": [
    "rootedDevice"
  ],
  "userId": "User Id value",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "Package Id value"
  },
  "id": "0e064997-4997-0e06-9749-060e9749060e",
  "version": "Version value",
  "patchVersion": "Patch Version value"
}
```



