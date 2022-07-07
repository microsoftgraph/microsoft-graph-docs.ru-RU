---
title: Тип ресурса deviceEnrollmentWindowsHelloForBusinessConfiguration
description: Windows Hello для бизнеса позволяет пользователям получать доступ к своим устройствам с помощью жеста, например биометрической проверки подлинности или ПИН-кода. Настройте параметры для зарегистрированных Windows 10, Windows 10 Mobile и более поздних версий.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3739ae61fd3724d3d850dae83fc1a078a12609c1
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2022
ms.locfileid: "66666853"
---
# <a name="deviceenrollmentwindowshelloforbusinessconfiguration-resource-type"></a>Тип ресурса deviceEnrollmentWindowsHelloForBusinessConfiguration

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Windows Hello для бизнеса позволяет пользователям получать доступ к своим устройствам с помощью жеста, например биометрической проверки подлинности или ПИН-кода. Настройте параметры для зарегистрированных Windows 10, Windows 10 Mobile и более поздних версий.


Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов deviceEnrollmentWindowsHelloForBusinessConfiguration](../api/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration-list.md)|Коллекция [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)|Список свойств и связей объектов [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).|
|[Получение объекта deviceEnrollmentWindowsHelloForBusinessConfiguration](../api/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration-get.md)|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)|Чтение свойств и связей объекта [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).|
|[Создание объекта deviceEnrollmentWindowsHelloForBusinessConfiguration](../api/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration-create.md)|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)|Создание объекта [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).|
|[Удаление объекта deviceEnrollmentWindowsHelloForBusinessConfiguration](../api/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration-delete.md)|Нет|Удаляет объект [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).|
|[Обновление объекта deviceEnrollmentWindowsHelloForBusinessConfiguration](../api/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration-update.md)|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)|Обновление свойств объекта [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор учетной записи, унаследованного от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|displayName|String|Отображаемое имя конфигурации регистрации устройства, унаследованного от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|description|String|Описание конфигурации регистрации устройства, унаследованного от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|priority|Int32|Приоритет используется, когда пользователь существует в нескольких группах, для которых назначена конфигурация регистрации. На пользователей распространяется только конфигурация с наименьшим значением приоритета. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|createdDateTime|DateTimeOffset|Дата создания в формате UTC конфигурации регистрации устройства, унаследованного от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|Дата последнего изменения в формате UTC конфигурации регистрации устройства, унаследованного от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|version|Int32|Версия конфигурации регистрации устройства, унаследованного от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|Идентификаторы roleScopeTagId|Коллекция String|Необязательные теги области роли для ограничений регистрации. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|DeviceEnrollmentConfigurationType|[DeviceEnrollmentConfigurationType](../resources/intune-onboarding-deviceenrollmentconfigurationtype.md)|Поддержка типа конфигурации регистрации, унаследованного [от deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md). Возможные значения: `unknown`, `limit`, `platformRestrictions`, `windowsHelloForBusiness`, `defaultLimit`, `defaultPlatformRestrictions`, `defaultWindowsHelloForBusiness`, `defaultWindows10EnrollmentCompletionPageConfiguration`, `windows10EnrollmentCompletionPageConfiguration`, `deviceComanagementAuthorityConfiguration`, `singlePlatformRestriction`, `unknownFutureValue`, `enrollmentNotificationsConfiguration`.|
|pinMinimumLength|Int32|Управляет минимальным количеством символов, необходимых для Windows Hello для бизнеса ПИН-кода.  Это значение должно быть в диапазоне от 4 до 127 включительно и меньше или равно значению, заданного для максимального ПИН-кода.|
|pinMaximumLength|Int32|Управляет максимальным количеством символов, разрешенных для Windows Hello для бизнеса ПИН-кода. Это значение должно быть в диапазоне от 4 до 127 включительно. Это значение должно быть больше или равно значению, заданным для минимального ПИН-кода.|
|pinUppercaseCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|Управляет возможностью использовать прописные буквы в Windows Hello для бизнеса ПИН-коде.  Разрешено использовать прописные буквы, в то время как обязательное гарантирует, что они присутствуют. Если задано значение "Запрещено", прописные буквы не будут разрешены. Возможные значения: `allowed`, `required`, `disallowed`.|
|pinLowercaseCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|Управляет возможностью использовать строчные буквы в Windows Hello для бизнеса ПИН-коде.  Разрешено использовать строчные буквы, в то время как обязательное гарантирует, что они присутствуют. Если задано значение "Запрещено", строчные буквы не будут разрешены. Возможные значения: `allowed`, `required`, `disallowed`.|
|pinSpecialCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|Управляет возможностью использовать специальные символы в Windows Hello для бизнеса ПИН-коде.  Разрешено использовать специальные символы, в то время как обязательное гарантирует, что они присутствуют. Если задано значение "Запрещено", специальные символы не будут разрешены. Возможные значения: `allowed`, `required`, `disallowed`.|
|state|[Включения](../resources/intune-onboarding-enablement.md)|Определяет, следует ли разрешить настройку устройства для Windows Hello для бизнеса. Если этот параметр отключен, пользователь не может подготовить Windows Hello для бизнеса, кроме мобильных телефонов, присоединенных к Azure Active Directory, если это необходимо. Если задано значение "Не настроено", Intune не будут переопределять значения по умолчанию для клиента. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|securityDeviceRequired|Boolean|Определяет, требуется ли доверенный платформенный модуль (TPM) для подготовки Windows Hello для бизнеса. TPM предоставляет дополнительное преимущество безопасности в том, что хранящиеся на нем данные не могут использоваться на других устройствах. Если задано значение False, все устройства могут Windows Hello для бизнеса, даже если нет доверенного платформенного модуля.|
|unlockWithBiometricsEnabled|Boolean|Управляет использованием биометрических жестов, таких как лицо и отпечаток пальца, в качестве альтернативы Windows Hello для бизнеса ПИН-коду.  Если задано значение False, биометрические жесты не допускаются. Пользователи по-прежнему должны настраивать ПИН-код в качестве резервной копии в случае сбоев.|
|remotePassportEnabled|Boolean|Управляет использованием удаленного Windows Hello для бизнеса. Удаленные Windows Hello для бизнеса позволяют использовать переносимое зарегистрированное устройство в качестве компаньона для проверки подлинности на рабочем столе. Рабочий стол должен быть Azure AD, а устройство-компаньон должно иметь Windows Hello для бизнеса ПИН-код.|
|pinPreviousBlockCount|Int32|Управляет возможностью запретить пользователям использовать прошлые ПИН-коды. Это значение должно быть задано в диапазоне от 0 до 50 включительно, и текущий ПИН-код пользователя будет включен в это число. Если задано значение 0, предыдущие ПИН-коды не сохраняются. Журнал ПИН-кодов не сохраняется при сбросе ПИН-кода.|
|pinExpirationInDays|Int32|Управляет периодом времени (в днях), в течение которого ПИН-код может использоваться до того, как система требует от пользователя изменить его. Это значение должно быть задано в диапазоне от 0 до 730 включительно. Если задано значение 0, пин-код пользователя никогда не истечет|
|enhancedBiometricsState|[Включения](../resources/intune-onboarding-enablement.md)|Управляет возможностью использовать функции защиты от спуфинга для распознавания лиц на устройствах, которые ее поддерживают. Если задано значение "Отключено", функции защиты от спуфинга не допускаются. Если задано значение "Не настроено", пользователь может выбрать, следует ли использовать защиту от спуфинга. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|securityKeyForSignIn|[Включения](../resources/intune-onboarding-enablement.md)|Ключ безопасности для входа предоставляет емкость для удаленного включения и отключения Windows Hello Sercurity Keyl Not configured будет учитывать конфигурации, выполняемые в CLINET. Возможные значения: `notConfigured`, `enabled`, `disabled`.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|Коллекция [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)|Список назначений групп для профиля конфигурации устройства, унаследованного от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
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
  "pinMinimumLength": 1024,
  "pinMaximumLength": 1024,
  "pinUppercaseCharactersUsage": "String",
  "pinLowercaseCharactersUsage": "String",
  "pinSpecialCharactersUsage": "String",
  "state": "String",
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "remotePassportEnabled": true,
  "pinPreviousBlockCount": 1024,
  "pinExpirationInDays": 1024,
  "enhancedBiometricsState": "String",
  "securityKeyForSignIn": "String"
}
```




