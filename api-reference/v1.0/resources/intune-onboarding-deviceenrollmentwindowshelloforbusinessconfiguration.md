---
title: Тип ресурса deviceEnrollmentWindowsHelloForBusinessConfiguration
description: Windows Параметры Hello for Business позволяют пользователям получать доступ к своим устройствам с помощью жеста, например биометрической проверки подлинности или ПИН-кода. Настройка параметров для зарегистрированных Windows 10, Windows 10 Mobile и более поздней.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cb1e1533f37be13eb40e0775e34879bd721c3319
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751603"
---
# <a name="deviceenrollmentwindowshelloforbusinessconfiguration-resource-type"></a>Тип ресурса deviceEnrollmentWindowsHelloForBusinessConfiguration

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Windows Параметры Hello for Business позволяют пользователям получать доступ к своим устройствам с помощью жеста, например биометрической проверки подлинности или ПИН-кода. Настройка параметров для зарегистрированных Windows 10, Windows 10 Mobile и более поздней.


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
|id|String|Уникальный идентификатор учетной записи, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|displayName|String|Отображающее имя конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|description|String|Описание конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|priority|Int32|Приоритет используется, когда пользователь существует в нескольких группах, которые назначены конфигурации регистрации. Пользователи подчиняются только конфигурации с наименьшим значением приоритета. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|createdDateTime|DateTimeOffset|Создано время даты в UTC конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|Последнее измененное время даты в UTC конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|version|Int32|Версия конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|pinMinimumLength|Int32|Управляет минимальным количеством символов, необходимых для пин Windows Hello для бизнеса.  Это значение должно быть от 4 до 127 включительно и меньше или равно значению, заданной для максимального ПИН-кода.|
|pinMaximumLength|Int32|Контролирует максимальное количество символов, разрешенных для пин Windows Hello для бизнеса. Это значение должно быть от 4 до 127 включительно. Это значение должно быть больше или равно значению, заданной для минимального ПИН-кода.|
|pinUppercaseCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|Управление возможностью использования букв верхнего шкафа в пин Windows Hello для бизнеса.  Разрешено использование верхнего регистра буквы(ы), в то время как Required гарантирует, что они присутствуют. Если установлено, что не разрешено, верхние буквы не будут разрешены. Возможные значения: `allowed`, `required`, `disallowed`.|
|pinLowercaseCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|Управление возможностью использования букв нижнего регистра в пин Windows Hello для бизнеса.  Разрешено использование нижней части буквы(ы), в то время как Required гарантирует, что они присутствуют. Если установлено, что не разрешено, буквы нижнего регистра не будут разрешены. Возможные значения: `allowed`, `required`, `disallowed`.|
|pinSpecialCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|Управление возможностью использования специальных символов в пин Windows Hello для бизнеса.  Разрешено использование специальных символов(ы), в то время как Required гарантирует, что они присутствуют. Если установлено запрещение, специальный символ (s) не будет разрешен. Возможные значения: `allowed`, `required`, `disallowed`.|
|состояние|[включить](../resources/intune-onboarding-enablement.md)|Контролирует, следует ли разрешить настройку устройства для Windows Hello для бизнеса. Если установлено отключение, пользователь не может Windows Hello для бизнеса, за исключением Azure Active Directory мобильных телефонов, если это необходимо. Если значение Не настроено, Intune не будет переопределять по умолчанию клиента. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|securityDeviceRequired|Boolean|Управление, необходимо ли требовать доверенный модуль платформы (TPM) для Windows Hello для бизнеса. TPM предоставляет дополнительные преимущества безопасности в том, что данные, хранимые на нем, не могут использоваться на других устройствах. Если установлено false, все устройства могут Windows Hello для бизнеса, даже если нет необходимого TPM.|
|unlockWithBiometricsEnabled|Boolean|Управление использованием биометрических жестов, таких как лицо и отпечатки пальцев, в качестве альтернативы пин Windows Hello для бизнеса.  Если установлено false, биометрические жесты не допускаются. Пользователи по-прежнему должны настраивать ПИН-код в качестве резервного копирования в случае сбоев.|
|remotePassportEnabled|Boolean|Управление использованием удаленного Windows Hello для бизнеса. Удаленное Windows Hello для бизнеса предоставляет возможность для переносного зарегистрированного устройства, которое можно использовать в качестве компаньона для проверки подлинности на рабочем столе. Настольный компьютер должен быть соединен с Azure AD, а на устройстве-компаньоне должен быть пин Windows Hello for Business PIN-код.|
|pinPreviousBlockCount|Int32|Контролирует возможность предотвращения использования пользователями прошлых ПИН-данных. Это должно быть установлено между 0 и 50 включительно, и текущий ПИН-код пользователя включен в это число. Если установлено 0, предыдущие ПИН-данные не сохраняются. История ПИН-кода не сохраняется с помощью сброса ПИН-кода.|
|pinExpirationInDays|Int32|Контролирует период времени (в днях), который пин-код можно использовать до того, как система требует от пользователя его изменить. Это должно быть установлено между 0 и 730 включительно. Если установлено 0, пин-код пользователя никогда не истекает|
|enhancedBiometricsState|[включить](../resources/intune-onboarding-enablement.md)|Контролирует возможность использования функций по борьбе с подменой для распознавания лиц на поддерживаемых устройствах. Если установлено отключение, не допускаются функции по борьбе с спуфингом. Если установлено, что не настроено, пользователь может выбрать, следует ли использовать подмену. Возможные значения: `notConfigured`, `enabled`, `disabled`.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|Коллекция [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)|Список групповых назначений для профиля конфигурации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|

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
  "enhancedBiometricsState": "String"
}
```




