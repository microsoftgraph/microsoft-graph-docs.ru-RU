---
title: Тип ресурса windows10EnrollmentCompletionPageConfiguration
description: Windows 10 конфигурации страницы состояния регистрации
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 19ff052b64aff545d4030d7f4491084ef9009d64
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209200"
---
# <a name="windows10enrollmentcompletionpageconfiguration-resource-type"></a>Тип ресурса windows10EnrollmentCompletionPageConfiguration

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Windows 10 конфигурации страницы состояния регистрации


Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов windows10EnrollmentCompletionPageConfiguration](../api/intune-onboarding-windows10enrollmentcompletionpageconfiguration-list.md)|[Коллекция windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)|Список свойств и связей объектов [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) .|
|[Получение объекта windows10EnrollmentCompletionPageConfiguration](../api/intune-onboarding-windows10enrollmentcompletionpageconfiguration-get.md)|[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)|Чтение свойств и связей объекта [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) .|
|[Создание объекта windows10EnrollmentCompletionPageConfiguration](../api/intune-onboarding-windows10enrollmentcompletionpageconfiguration-create.md)|[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)|Создайте объект [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) .|
|[Удаление объекта windows10EnrollmentCompletionPageConfiguration](../api/intune-onboarding-windows10enrollmentcompletionpageconfiguration-delete.md)|Нет|Удаляет объект [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md).|
|[Обновление объекта windows10EnrollmentCompletionPageConfiguration](../api/intune-onboarding-windows10enrollmentcompletionpageconfiguration-update.md)|[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)|Обновление свойств объекта [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор учетной записи, унаследованного от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|displayName|Строка|Отображаемое имя конфигурации регистрации устройства, унаследованного от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|description|Строка|Описание конфигурации регистрации устройства, унаследованного от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|priority|Int32|Приоритет используется, когда пользователь существует в нескольких группах, для которых назначена конфигурация регистрации. На пользователей распространяется только конфигурация с наименьшим значением приоритета. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|createdDateTime|DateTimeOffset|Дата создания в формате UTC конфигурации регистрации устройства, унаследованного от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|Дата последнего изменения в формате UTC конфигурации регистрации устройства, унаследованного от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|version|Int32|Версия конфигурации регистрации устройства, унаследованного от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|Идентификаторы roleScopeTagId|Коллекция объектов string|Необязательные теги области роли для ограничений регистрации. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|DeviceEnrollmentConfigurationType|[DeviceEnrollmentConfigurationType](../resources/intune-onboarding-deviceenrollmentconfigurationtype.md)|Поддержка типа конфигурации регистрации, унаследованного [от deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md). Возможные значения: `unknown`, `limit`, `platformRestrictions`, `windowsHelloForBusiness`, `defaultLimit`, `defaultPlatformRestrictions`, `defaultWindowsHelloForBusiness`, `defaultWindows10EnrollmentCompletionPageConfiguration`, `windows10EnrollmentCompletionPageConfiguration`, `deviceComanagementAuthorityConfiguration`, `singlePlatformRestriction`, `unknownFutureValue`, `enrollmentNotificationsConfiguration`.|
|showInstallationProgress|Логическое|Отображение или скрытие хода установки для пользователя|
|blockDeviceSetupRetryByUser|Логическое|Разрешить пользователю повторить установку при сбое установки|
|allowDeviceResetOnInstallFailure|Логическое|Разрешить или заблокировать сброс устройства при сбое установки|
|allowLogCollectionOnInstallFailure|Логический|Разрешить или заблокировать сбор журналов при сбое установки|
|customErrorMessage|String|Настройка настраиваемого сообщения об ошибке, отображаемого при сбое установки|
|installProgressTimeoutInMinutes|Int32|Задание времени ожидания хода выполнения установки в минутах|
|allowDeviceUseOnInstallFailure|Логический|Разрешить пользователю продолжать использовать устройство при сбое установки|
|selectedMobileAppIds|Коллекция String|Выбранные приложения для отслеживания состояния установки|
|trackInstallProgressForAutopilotOnly|Логическое|Отображение хода установки только для сценариев регистрации Autopilot|
|disableUserStatusTrackingAfterFirstUser|Логический|Отображение хода установки только для первого пользователя после регистрации|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|Коллекция [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)|Список назначений групп для профиля конфигурации устройства, унаследованного от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10EnrollmentCompletionPageConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10EnrollmentCompletionPageConfiguration",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "priority": 1024,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": 1024,
  "roleScopeTagIds": [
    "String"
  ],
  "deviceEnrollmentConfigurationType": "String",
  "showInstallationProgress": true,
  "blockDeviceSetupRetryByUser": true,
  "allowDeviceResetOnInstallFailure": true,
  "allowLogCollectionOnInstallFailure": true,
  "customErrorMessage": "String",
  "installProgressTimeoutInMinutes": 1024,
  "allowDeviceUseOnInstallFailure": true,
  "selectedMobileAppIds": [
    "String"
  ],
  "trackInstallProgressForAutopilotOnly": true,
  "disableUserStatusTrackingAfterFirstUser": true
}
```




