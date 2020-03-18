---
title: Тип ресурса windows10EnrollmentCompletionPageConfiguration
description: Конфигурация страницы состояния регистрации Windows 10
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 06463e7757a0cc20ef53606b674759ab30736da0
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42777252"
---
# <a name="windows10enrollmentcompletionpageconfiguration-resource-type"></a>Тип ресурса windows10EnrollmentCompletionPageConfiguration

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Конфигурация страницы состояния регистрации Windows 10


Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список windows10EnrollmentCompletionPageConfigurations](../api/intune-onboarding-windows10enrollmentcompletionpageconfiguration-list.md)|Коллекция [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)|Список свойств и связей объектов [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) .|
|[Получение windows10EnrollmentCompletionPageConfiguration](../api/intune-onboarding-windows10enrollmentcompletionpageconfiguration-get.md)|[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)|Чтение свойств и связей объекта [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) .|
|[Создание windows10EnrollmentCompletionPageConfiguration](../api/intune-onboarding-windows10enrollmentcompletionpageconfiguration-create.md)|[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)|Создание нового объекта [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) .|
|[Удаление windows10EnrollmentCompletionPageConfiguration](../api/intune-onboarding-windows10enrollmentcompletionpageconfiguration-delete.md)|Нет|Удаляет объект [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md).|
|[Обновление windows10EnrollmentCompletionPageConfiguration](../api/intune-onboarding-windows10enrollmentcompletionpageconfiguration-update.md)|[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)|Обновление свойств объекта [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для учетной записи, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|displayName|Строка|Отображаемое имя конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|description|String|Описание конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|priority|Int32|Priority используется, когда пользователь существует в нескольких группах, которым назначена Настройка регистрации. Пользователи подчиняются только конфигурации с наименьшим значением приоритета. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|createdDateTime|DateTimeOffset|Созданная Дата и время в формате UTC для настройки регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|version|Int32|Версия конфигурации регистрации устройств, унаследованная от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|шовинсталлатионпрогресс|Логический|Отображение или скрытие хода установки для пользователя|
|блоккдевицесетупретрибюсер|Логический|Разрешить пользователю повторно выполнить установку при сбое установки|
|алловдевицересетонинсталлфаилуре|Логический|Разрешение или блокировка сброса устройства при сбое установки|
|алловлогколлектиононинсталлфаилуре|Логический|Разрешение или блокировка сбора журналов при сбое установки|
|кустомеррормессаже|String|Задать настраиваемое сообщение об ошибке, которое будет отображаться после сбоя установки|
|инсталлпрогресстимеаутинминутес|Int32|Задать время ожидания установки (в минутах)|
|алловдевицеусеонинсталлфаилуре|Логический|Разрешить пользователю продолжать использовать устройство при сбое установки|
|селектедмобилеаппидс|Коллекция String|Выбранные приложения для отслеживания состояния установки|
|траккинсталлпрогрессфораутопилотонли|Логический|Показывать только ход выполнения установки для сценариев автоматической пилотной установки|
|дисаблеусерстатустраккингафтерфирстусер|Логический|Показывать только сведения о ходе установки для первой процедуры регистрации пользователя|

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



