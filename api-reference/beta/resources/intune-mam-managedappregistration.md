---
title: Тип ресурса managedAppRegistration
description: ManagedAppEntity — это базовый тип для всех остальных типов объектов в рабочем процессе управления приложениями. Ресурс ManagedAppRegistration представляет собой сведения об управляемом приложении, используемом членом организации.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1e97a238c758f4fdc3130c2527f82ce4445980fc
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178222"
---
# <a name="managedappregistration-resource-type"></a>Тип ресурса managedAppRegistration

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

ManagedAppEntity — это базовый тип для всех остальных типов объектов в рабочем процессе управления приложениями.
Ресурс ManagedAppRegistration представляет собой сведения об управляемом приложении, используемом членом организации.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов managedAppRegistration](../api/intune-mam-managedappregistration-list.md)|Коллекция объектов [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|Список свойств и связей объектов [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|[Получение объекта managedAppRegistration](../api/intune-mam-managedappregistration-get.md)|[managedAppRegistration](../resources/intune-mam-managedappregistration.md)|Чтение свойств и связей объекта [managedAppRegistration](../resources/intune-mam-managedappregistration.md).|
|[Функция getUserIdsWithFlaggedAppRegistration](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|Коллекция объектов string|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Дата и время создания.|
|lastSyncDateTime|DateTimeOffset|Дата и время последней синхронизации приложения со службой управления.|
|applicationVersion|Строка|Версия приложения.|
|managementSdkVersion|Строка|Версия пакета SDK для управления приложениями.|
|platformVersion|Строка|Версия операционной системы.|
|deviceType|Строка|Тип главного устройства.|
|deviceTag|String|Тег, который создан с использованием пакета SDK для управления приложениями и позволяет связать приложения, размещенные на одном устройстве. Мы не гарантируем, что приложения будут связаны во всех состояниях.|
|deviceName|String|Имя главного устройства.|
|манажеддевицеид|Строка|Управляемый идентификатор устройства хоста. Значение может быть пустым, даже если ведущее устройство управляется.|
|azureADDeviceId|Строка|Идентификатор устройства Azure Active Directory ведущего устройства. Значение может быть пустым, даже если ведущее устройство является зарегистрированным Azure Active Directory.|
|deviceModel|Строка|Модель устройства для регистрации текущего приложения |
|девицемануфактурер|Строка|Производитель устройства для регистрации текущего приложения |
|flaggedReasons|Коллекция [манажедаппфлагжедреасон](../resources/intune-mam-managedappflaggedreason.md)|Нуль или более причин, по которым помечается регистрация приложения например приложения, запущенного на устройстве с административным доступом.|
|userId|String|ИД пользователя, к которому относится эта регистрация приложения.|
|appIdentifier|[mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)|Идентификатор пакета приложения.|
|id|Строка|Ключ объекта.|
|version|Строка|Версия объекта.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|appliedPolicies|Коллекция [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|Нуль или более политик, примененных к зарегистрированному приложению, когда оно в последний раз синхронизировалось со службой управления.|
|intendedPolicies|Коллекция объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|Нуль или более политик, которые на текущий момент администратор использует для приложения.|
|operations|Коллекция объектов [managedAppOperation](../resources/intune-mam-managedappoperation.md)|Нуль или более долговременных операций, запускаемых для регистрации приложения.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppRegistration"
}
-->
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
  "managedDeviceId": "String",
  "azureADDeviceId": "String",
  "deviceModel": "String",
  "deviceManufacturer": "String",
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



