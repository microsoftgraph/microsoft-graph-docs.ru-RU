---
title: Тип ресурса user
description: Представляет объект пользователя Azure Active Directory.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d5aef878787f0bf9b8a7a2cd95810e54d1e8f166
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811881"
---
# <a name="user-resource-type"></a>Тип ресурса user

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Представляет объект пользователя Azure Active Directory.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|Объекты [список пользователей](../api/intune-shared-user-list.md) .|Коллекция объектов [user](../resources/intune-shared-user.md)|Список свойств и связей объектов [user](../resources/intune-shared-user.md).|
|[Получение пользовательского](../api/intune-shared-user-get.md) объекта.|[user](../resources/intune-shared-user.md)|Чтение свойств и связей объекта [user](../resources/intune-shared-user.md).|
|Объект [Создать пользователя](../api/intune-shared-user-create.md) .|[user](../resources/intune-shared-user.md)|Создание объекта [user](../resources/intune-shared-user.md).|
|[Удаление пользователя](../api/intune-shared-user-delete.md).|Нет|Удаляет объект [user](../resources/intune-shared-user.md).|
|Объект [пользователя обновления](../api/intune-shared-user-update.md) .|[user](../resources/intune-shared-user.md)|Обновление свойств объекта [user](../resources/intune-shared-user.md).|
|**Управление устройствами**|
|[функция getLoggedOnManagedDevices](../api/intune-shared-user-getloggedonmanageddevices.md)|Коллекция [managedDevice](../resources/intune-devices-manageddevice.md)|Н/Д|
|[Действие removeAllDevicesFromManagement](../api/intune-shared-user-removealldevicesfrommanagement.md)|Нет|Прекращение управления всеми устройствами для этого пользователя|
|**Мобильное приложение управления (MAM)**|
|[Функция getManagedAppDiagnosticStatuses](../api/intune-shared-user-getmanagedappdiagnosticstatuses.md)|Коллекция [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md)|Получает состояние диагностической проверки определенного пользователя.|
|[Функция getManagedAppPolicies](../api/intune-shared-user-getmanagedapppolicies.md)|Коллекция [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|Получает ограничения приложений для определенного пользователя.|
|[Действие wipeManagedAppRegistrationByDeviceTag](../api/intune-shared-user-wipemanagedappregistrationbydevicetag.md)|Нет|Стирает данные о регистрации приложений с указанным тегом приложения.|
|[Действие wipeManagedAppRegistrationsByDeviceTag](../api/intune-shared-user-wipemanagedappregistrationsbydevicetag.md)|Нет|Стирает данные о регистрации приложений с указанным тегом приложения.|
|**Адаптация новых сотрудников**|
|[функция exportDeviceAndAppManagementData](../api/intune-shared-user-exportdeviceandappmanagementdata.md)|[deviceAndAppManagementData](../resources/intune-onboarding-deviceandappmanagementdata.md);|Н/Д|
|[функция getEffectiveDeviceEnrollmentConfigurations](../api/intune-shared-user-geteffectivedeviceenrollmentconfigurations.md)|Коллекция объектов [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|Н/Д|
|**Устранение неполадок**|
|[функция getManagedDevicesWithAppFailures](../api/intune-shared-user-getmanageddeviceswithappfailures.md)|Коллекция String|Получает список устройств, при помощи неудачных приложений.|


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор пользователя.|
|**Адаптация новых сотрудников**|
|deviceEnrollmentLimit|Int32|Максимальное количество устройств, которые разрешено зарегистрировать пользователю. Допустимые значения: 5 или 1000.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|**Управление устройствами**|
|managedDevices|Коллекция [managedDevice](../resources/intune-devices-manageddevice.md)|Управляемые устройства, связанные с пользователем.|
|**Мобильное приложение управления (MAM)**|
|managedAppRegistrations|Коллекция [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|Любое количество объектов регистрации управляемых приложений, принадлежащих пользователю.|
|**Адаптация новых сотрудников**|
|Объекты deviceEnrollmentConfiguration|Коллекция объектов [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|Получение конфигураций заявок через Интернет, нацелено на пользователя|
|**Устранение неполадок**|
|deviceManagementTroubleshootingEvents|Коллекция [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|Список событий устранения неполадок для этого пользователя.|
|mobileAppIntentAndStates|[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) коллекции|Список событий устранения неполадок для этого пользователя.|
|mobileAppTroubleshootingEvents|[mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md) коллекции|Список мобильного приложения, устранение неполадок события для этого пользователя.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.user"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.user",
  "id": "String (identifier)"
}
```



