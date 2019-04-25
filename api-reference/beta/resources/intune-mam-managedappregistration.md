---
title: Тип ресурса managedAppRegistration
description: ManagedAppEntity — это базовый тип для всех остальных типов объектов в рабочем процессе управления приложениями. Ресурс ManagedAppRegistration представляет собой сведения об управляемом приложении, используемом членом организации.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3be91dd094258f0bf998521c058f1c62659fbcc8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581032"
---
# <a name="managedappregistration-resource-type"></a>Тип ресурса managedAppRegistration

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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
|applicationVersion|String|Версия приложения.|
|managementSdkVersion|String|Версия пакета SDK для управления приложениями.|
|platformVersion|String|Версия операционной системы.|
|deviceType|String|Тип главного устройства.|
|deviceTag|String|Тег, который создан с использованием пакета SDK для управления приложениями и позволяет связать приложения, размещенные на одном устройстве. Мы не гарантируем, что приложения будут связаны во всех состояниях.|
|deviceName|String|Имя главного устройства.|
|Манажеддевицеид|String|Управляемый идентификатор устройства хоста. Значение может быть пустым, даже если ведущее устройство управляется.|
|azureADDeviceId|String|Идентификатор устройства Azure Active Directory ведущего устройства. Значение может быть пустым, даже если ведущее устройство является зарегистрированным Azure Active Directory.|
|deviceModel|String|Модель устройства для регистрации текущего приложения |
|Девицемануфактурер|String|Производитель устройства для регистрации текущего приложения |
|flaggedReasons|Коллекция [манажедаппфлагжедреасон](../resources/intune-mam-managedappflaggedreason.md)|Нуль или более причин, по которым помечается регистрация приложения например приложения, запущенного на устройстве с административным доступом.|
|userId|String|ИД пользователя, к которому относится эта регистрация приложения.|
|appIdentifier|[mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)|Идентификатор пакета приложения.|
|id|String|Ключ объекта.|
|version|Строка|Версия объекта.|

## <a name="relationships"></a>Связи
|Отношение|Тип|Описание|
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
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "id": "String (identifier)",
  "version": "String"
}
```





