---
title: Тип ресурса deviceEnrollmentWindowsHelloForBusinessConfiguration
description: Windows Hello для бизнеса позволяет пользователям получать доступ к своим устройствам с помощью жеста, например биометрической проверки подлинности или ПИН-кода. Настройка параметров для зарегистрированных Windows 10, Windows 10 Mobile и более поздней.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b88a8dde9dc4046c74d4eb5f73b5643da6460aa9
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58782044"
---
# <a name="deviceenrollmentwindowshelloforbusinessconfiguration-resource-type"></a>Тип ресурса deviceEnrollmentWindowsHelloForBusinessConfiguration

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Windows Hello для бизнеса позволяет пользователям получать доступ к своим устройствам с помощью жеста, например биометрической проверки подлинности или ПИН-кода. Настройка параметров для зарегистрированных Windows 10, Windows 10 Mobile и более поздней.


Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)

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
|id|Строка|Уникальный идентификатор учетной записи, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|displayName|Строка|Отображающее имя конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|description|Строка|Описание конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|priority|Int32|Приоритет используется, когда пользователь существует в нескольких группах, которые назначены конфигурации регистрации. Пользователи подчиняются только конфигурации с наименьшим значением приоритета. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|createdDateTime|DateTimeOffset|Создано время даты в UTC конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|Последнее измененное время даты в UTC конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|version|Int32|Версия конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|roleScopeTagIds|Коллекция String|Необязательные теги области ролей для ограничений регистрации. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|pinMinimumLength|Int32|Управляет минимальным количеством символов, необходимых для Windows Hello для бизнес-ПИН-кода.  Это значение должно быть от 4 до 127 включительно и меньше или равно значению, заданной для максимального ПИН-кода.|
|pinMaximumLength|Int32|Управляет максимальным количеством символов, разрешенных для пин-Windows Hello для бизнеса. Это значение должно быть от 4 до 127 включительно. Это значение должно быть больше или равно значению, заданной для минимального ПИН-кода.|
|pinUppercaseCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|Управление возможностью использования букв верхнего регистра в Windows Hello для бизнеса PIN-код.  Разрешено использование верхнего регистра буквы(ы), в то время как Required гарантирует, что они присутствуют. Если установлено, что не разрешено, верхние буквы не будут разрешены. Возможные значения: `allowed`, `required`, `disallowed`.|
|pinLowercaseCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|Управление возможностью использования букв нижнего регистра в Windows Hello для бизнеса PIN-код.  Разрешено использование нижней части буквы(ы), в то время как Required гарантирует, что они присутствуют. Если установлено, что не разрешено, буквы нижнего регистра не будут разрешены. Возможные значения: `allowed`, `required`, `disallowed`.|
|pinSpecialCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|Управление возможностью использования специальных символов в Windows Hello для бизнеса PIN-код.  Разрешено использование специальных символов(ы), в то время как Required гарантирует, что они присутствуют. Если установлено запрещение, специальный символ (s) не будет разрешен. Возможные значения: `allowed`, `required`, `disallowed`.|
|state|[включить](../resources/intune-shared-enablement.md)|Контролирует, следует ли разрешить настраивать устройство для Windows Hello для бизнеса. Если установлено отключение, пользователь не может Windows Hello для бизнеса, за исключением Azure Active Directory мобильных телефонов, если это необходимо. Если значение Не настроено, Intune не будет переопределять по умолчанию клиента. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|securityDeviceRequired|Boolean|Управление, необходимо ли требовать доверенный модуль платформы (TPM) для Windows Hello для бизнеса. TPM предоставляет дополнительные преимущества безопасности в том, что данные, хранимые на нем, не могут использоваться на других устройствах. Если установлено false, все устройства могут Windows Hello для бизнеса, даже если нет необходимого TPM.|
|unlockWithBiometricsEnabled|Boolean|Управление использованием биометрических жестов, таких как лицо и отпечатки пальцев, в качестве альтернативы Windows Hello для бизнеса PIN-код.  Если установлено false, биометрические жесты не допускаются. Пользователи по-прежнему должны настраивать ПИН-код в качестве резервного копирования в случае сбоев.|
|remotePassportEnabled|Boolean|Управление использованием удаленных Windows Hello для бизнеса. Удаленные Windows Hello для бизнеса предоставляют возможность для переносного зарегистрированного устройства, которое будет использовать в качестве компаньона для проверки подлинности на рабочем столе. Настольный компьютер должен быть соединен с Azure AD, а устройство-компаньон должно иметь Windows Hello для бизнес-ПИН-кода.|
|pinPreviousBlockCount|Int32|Контролирует возможность предотвращения использования пользователями прошлых ПИН-данных. Это должно быть установлено между 0 и 50 включительно, и текущий ПИН-код пользователя включен в это число. Если установлено 0, предыдущие ПИН-данные не сохраняются. История ПИН-кода не сохраняется с помощью сброса ПИН-кода.|
|pinExpirationInDays|Int32|Контролирует период времени (в днях), который пин-код можно использовать до того, как система требует от пользователя его изменить. Это должно быть установлено между 0 и 730 включительно. Если установлено 0, пин-код пользователя никогда не истекает|
|enhancedBiometricsState|[включить](../resources/intune-shared-enablement.md)|Контролирует возможность использования функций по борьбе с подменой для распознавания лиц на поддерживаемых устройствах. Если установлено отключение, не допускаются функции по борьбе с спуфингом. Если установлено, что не настроено, пользователь может выбрать, следует ли использовать подмену. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|securityKeyForSignIn|[включить](../resources/intune-shared-enablement.md)|Ключ безопасности для sign In предоставляет возможность удаленного отключения on/OFF Windows Hello Sercurity Keyl Not configured будет соблюдать конфигурации, которые делаются на clinet. Возможные значения: `notConfigured`, `enabled`, `disabled`.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|Коллекция [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)|Список групповых назначений для профиля конфигурации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|

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



