---
title: Тип ресурса managedAppRegistration
description: ManagedAppEntity — это базовый тип для всех остальных типов объектов в рабочем процессе управления приложениями.
ms.openlocfilehash: bf05e7180f27be9c813f8fbb05346893fa6db172
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077783"
---
# <a name="managedappregistration-resource-type"></a>Тип ресурса managedAppRegistration

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

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
|deviceTag|String|Тег, который создан с использованием пакета SDK для управления приложениями и помогает связывать приложения, размещенные на одном устройстве. Мы не гарантируем, что приложения будут связаны во всех состояниях.|
|deviceName|String|Имя главного устройства.|
|managedDeviceId|String|Управляемые устройства идентификатор устройства узла. Значение может быть пустой, даже в том случае, если управляемые устройства узла.|
|azureADDeviceId|String|Идентификатор Azure Active Directory устройства устройства узла. Значение может быть пустым, даже в том случае, если устройство узла — это Azure Active Directory зарегистрирован.|
|deviceModel|String|Модель устройства для текущего Регистрация приложения |
|deviceManufacturer|String|Производитель устройства для текущего Регистрация приложения |
|flaggedReasons|[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) коллекции|Причины, по которым помечается регистрация приложения (если они есть). например приложения, запущенного на устройстве с административным доступом.|
|userId|String|ИД пользователя, к которому относится эта регистрация приложения.|
|appIdentifier|[mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)|Идентификатор пакета приложения.|
|id|String|Ключ объекта.|
|version|String|Версия объекта.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|appliedPolicies|Коллекция объектов [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|Нуль или более политик, примененных к зарегистрированному приложению, когда оно в последний раз синхронизировалось со службой управления.|
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





