---
title: Тип ресурса user
description: Представляет объект пользователя Azure Active Directory.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2b6903b9d6c81b05e667bfa35cb2ee4955e6f479
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51864951"
---
# <a name="user-resource-type"></a>Тип ресурса user

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет объект пользователя Azure Active Directory.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов](../api/intune-shared-user-list.md) пользователей.|Коллекция объектов [user](../resources/intune-shared-user.md)|Список свойств и связей объектов [user](../resources/intune-shared-user.md).|
|[Получите объект](../api/intune-shared-user-get.md) пользователя.|[user](../resources/intune-shared-user.md)|Чтение свойств и связей объекта [user](../resources/intune-shared-user.md).|
|[Создание объекта](../api/intune-shared-user-create.md) пользователя.|[user](../resources/intune-shared-user.md)|Создание объекта [user](../resources/intune-shared-user.md).|
|[Удаление пользователя](../api/intune-shared-user-delete.md).|Нет|Удаляет объект [user](../resources/intune-shared-user.md).|
|[Обновление объекта](../api/intune-shared-user-update.md) пользователя.|[user](../resources/intune-shared-user.md)|Обновление свойств объекта [user](../resources/intune-shared-user.md).|
|**Управление устройствами**|
|[функция getLoggedOnManagedDevices](../api/intune-shared-user-getloggedonmanageddevices.md)|Коллекция [managedDevice](../resources/intune-devices-manageddevice.md)|Пока не задокументировано.|
|[Действие removeAllDevicesFromManagement](../api/intune-shared-user-removealldevicesfrommanagement.md)|Нет|Прекращение управления всеми устройствами для этого пользователя|
|**Управление мобильными приложениями (MAM)**|
|[Функция getManagedAppDiagnosticStatuses](../api/intune-shared-user-getmanagedappdiagnosticstatuses.md)|Коллекция [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md)|Получает состояние диагностической проверки определенного пользователя.|
|[Функция getManagedAppPolicies](../api/intune-shared-user-getmanagedapppolicies.md)|Коллекция [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|Получает ограничения приложений для определенного пользователя.|
|[Действие wipeManagedAppRegistrationByDeviceTag](../api/intune-shared-user-wipemanagedappregistrationbydevicetag.md)|Нет|Стирает данные о регистрации приложений с указанным тегом приложения.|
|[Действие wipeManagedAppRegistrationsByDeviceTag](../api/intune-shared-user-wipemanagedappregistrationsbydevicetag.md)|Нет|Стирает данные о регистрации приложений с указанным тегом приложения.|
|**Адаптация**|
|[exportDeviceAndAppManagementData](../api/intune-shared-user-exportdeviceandappmanagementdata.md)|[deviceAndAppManagementData](../resources/intune-onboarding-deviceandappmanagementdata.md);|Пока не задокументировано.|
|[функция getEffectiveDeviceEnrollmentConfigurations](../api/intune-shared-user-geteffectivedeviceenrollmentconfigurations.md)|Коллекция объектов [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|Пока не задокументировано.|
|**Устранение неполадок**|
|[функция getManagedDevicesWithAppFailures](../api/intune-shared-user-getmanageddeviceswithappfailures.md)|Коллекция String|Извлекает список устройств с сбойными приложениями.|


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор пользователя.|
|**Адаптация**|
|deviceEnrollmentLimit|Int32|Максимальное количество устройств, которые разрешено зарегистрировать пользователю. Допустимые значения: 5 или 1000.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|**Управление устройствами**|
|managedDevices|Коллекция [managedDevice](../resources/intune-devices-manageddevice.md)|Управляемые устройства, связанные с пользователем.|
|**Управление мобильными приложениями (MAM)**|
|managedAppRegistrations|Коллекция [managedAppRegistration](../resources/intune-mam-managedappregistration.md)|Любое количество объектов регистрации управляемых приложений, принадлежащих пользователю.|
|**Адаптация**|
|Объекты deviceEnrollmentConfiguration|Коллекция объектов [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|Настройка регистрации, ориентированная на пользователя|
|**Устранение неполадок**|
|deviceManagementTroubleshootingEvents|Коллекция [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|Список событий устранения неполадок для этого пользователя.|
|mobileAppIntentAndStates|[коллекция mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)|Список событий устранения неполадок для этого пользователя.|
|mobileAppTroubleshootingEvents|[коллекция mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)|Список событий устранения неполадок мобильных приложений для этого пользователя.|

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




