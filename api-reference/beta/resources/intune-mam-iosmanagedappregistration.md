---
title: Тип ресурса iosManagedAppRegistration
description: Представляет собой сведения о синхронизации управляемого приложения iOS для определенного пользователя. Ресурс ManagedAppRegistration представляет собой сведения об управляемом приложении, используемом членом организации.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b892bdd48c88a66d7be03ba95c5695747d957af7
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49297905"
---
# <a name="iosmanagedappregistration-resource-type"></a>Тип ресурса iosManagedAppRegistration

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет собой сведения о синхронизации управляемого приложения iOS для определенного пользователя.
Ресурс ManagedAppRegistration представляет собой сведения об управляемом приложении, используемом членом организации.


Наследуется от [managedAppRegistration](../resources/intune-mam-managedappregistration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление iosManagedAppRegistrations](../api/intune-mam-iosmanagedappregistration-list.md)|Коллекция [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md)|Список свойств и связей объектов [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md).|
|[Получение iosManagedAppRegistration](../api/intune-mam-iosmanagedappregistration-get.md)|[iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md)|Чтение свойств и связей объекта [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md).|

## <a name="properties"></a>Свойства
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
|манажеддевицеид|String|Управляемый идентификатор устройства хоста. Значение может быть пустым, даже если ведущее устройство управляется. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|azureADDeviceId|String|Идентификатор устройства Azure Active Directory ведущего устройства. Значение может быть пустым, даже если ведущее устройство является зарегистрированным Azure Active Directory. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|deviceModel|String|Модель устройства для текущей регистрации приложения наследуется от [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|девицемануфактурер|String|Производитель устройства для текущей регистрации приложения, унаследованный от [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|
|flaggedReasons|Коллекция [манажедаппфлагжедреасон](../resources/intune-mam-managedappflaggedreason.md)|Нуль или более причин, по которым помечается регистрация приложения Пример: приложение запускается на рутованном устройстве. Наследуется от [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|userId|String|Идентификатор пользователя, к которому относится эта регистрация приложения. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|appIdentifier|[mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)|Идентификатор пакета приложения. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|id|String|Ключ объекта. Наследуется от объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|version|String|Версия объекта. Наследуется от [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|appliedPolicies|Коллекция объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|Нуль или более политик, примененных к зарегистрированному приложению, когда оно в последний раз синхронизировалось со службой управления. Наследуется от [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|intendedPolicies|Коллекция объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|Нуль или более политик, которые на текущий момент администратор использует для приложения. Наследуется от [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|operations|Коллекция объектов [managedAppOperation](../resources/intune-mam-managedappoperation.md)|Нуль или более долговременных операций, запускаемых для регистрации приложения. Наследуется от [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosManagedAppRegistration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosManagedAppRegistration",
  "createdDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "applicationVersion": "String",
  "managementSdkVersion": "String",
  "platformVersion": "String",
  "deviceType": "String",
  "deviceTag": "String",
  "deviceName": "String",
  "managedDeviceId": "String",
  "azureADDeviceId": "String",
  "deviceModel": "String",
  "deviceManufacturer": "String",
  "flaggedReasons": [
    "String"
  ],
  "userId": "String",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.iosMobileAppIdentifier",
    "bundleId": "String"
  },
  "id": "String (identifier)",
  "version": "String"
}
```




