---
title: Создание deviceEnrollmentWindowsHelloForBusinessConfiguration
description: Создание объекта deviceEnrollmentWindowsHelloForBusinessConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b07a10f3a3a5e7ceb590c2f56650c03eaa1cad10
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51158859"
---
# <a name="create-deviceenrollmentwindowshelloforbusinessconfiguration"></a>Создание deviceEnrollmentWindowsHelloForBusinessConfiguration

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание объекта [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись)|DeviceManagementServiceConfig.ReadWrite.All|
|Делегированное (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementServiceConfig.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса добавьте представление объекта deviceEnrollmentWindowsHelloForBusinessConfiguration в формате JSON.

В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта deviceEnrollmentWindowsHelloForBusinessConfiguration.

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
|pinMinimumLength|Int32|Управляет минимальным количеством символов, необходимых для ПИН-кода Windows Hello для бизнеса.  Это значение должно быть от 4 до 127 включительно и меньше или равно значению, заданной для максимального ПИН-кода.|
|pinMaximumLength|Int32|Контролирует максимальное количество символов, разрешенных для ПИН-кода Windows Hello для бизнеса. Это значение должно быть от 4 до 127 включительно. Это значение должно быть больше или равно значению, заданной для минимального ПИН-кода.|
|pinUppercaseCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|Управление возможностью использования букв верхнего шкафа в ПИН-коде Windows Hello для бизнеса.  Разрешено использование верхнего регистра буквы(ы), в то время как Required гарантирует, что они присутствуют. Если установлено, что не разрешено, верхние буквы не будут разрешены. Возможные значения: `allowed`, `required`, `disallowed`.|
|pinLowercaseCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|Управление возможностью использования букв нижнего регистра в ПИН-коде Windows Hello для бизнеса.  Разрешено использование нижней части буквы(ы), в то время как Required гарантирует, что они присутствуют. Если установлено, что не разрешено, буквы нижнего регистра не будут разрешены. Возможные значения: `allowed`, `required`, `disallowed`.|
|pinSpecialCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|Управление возможностью использования специальных символов в ПИН-коде Windows Hello для бизнеса.  Разрешено использование специальных символов(ы), в то время как Required гарантирует, что они присутствуют. Если установлено запрещение, специальный символ (s) не будет разрешен. Возможные значения: `allowed`, `required`, `disallowed`.|
|state|[включить](../resources/intune-shared-enablement.md)|Управление настройкой устройства для Windows Hello для бизнеса. Если установлено отключение, пользователь не может представить Windows Hello для бизнеса, за исключением Azure Active Directory, присоединив к мобильным телефонам, если это необходимо. Если значение Не настроено, Intune не будет переопределять по умолчанию клиента. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|securityDeviceRequired|Boolean|Управление, необходимо ли требовать доверенный модуль платформы (TPM) для обеспечения Windows Hello для бизнеса. TPM предоставляет дополнительные преимущества безопасности в том, что данные, хранимые на нем, не могут использоваться на других устройствах. Если установлено false, все устройства могут устанавливать Windows Hello для бизнеса, даже если не существует понятного TPM.|
|unlockWithBiometricsEnabled|Boolean|Управление использованием биометрических жестов, таких как лицо и отпечатки пальцев, в качестве альтернативы ПИН-коду Windows Hello для бизнеса.  Если установлено false, биометрические жесты не допускаются. Пользователи по-прежнему должны настраивать ПИН-код в качестве резервного копирования в случае сбоев.|
|remotePassportEnabled|Boolean|Управление использованием удаленной Windows Hello для бизнеса. Удаленное Windows Hello для бизнеса предоставляет возможность для переносного зарегистрированного устройства, которое можно использовать в качестве компаньона для проверки подлинности на рабочем столе. Настольный компьютер должен быть соединен с Azure AD, а устройство-компаньон должно иметь ПИН-код Windows Hello для бизнеса.|
|pinPreviousBlockCount|Int32|Контролирует возможность предотвращения использования пользователями прошлых ПИН-данных. Это должно быть установлено между 0 и 50 включительно, и текущий ПИН-код пользователя включен в это число. Если установлено 0, предыдущие ПИН-данные не сохраняются. История ПИН-кода не сохраняется с помощью сброса ПИН-кода.|
|pinExpirationInDays|Int32|Контролирует период времени (в днях), который пин-код можно использовать до того, как система требует от пользователя его изменить. Это должно быть установлено между 0 и 730 включительно. Если установлено 0, пин-код пользователя никогда не истекает|
|enhancedBiometricsState|[включить](../resources/intune-shared-enablement.md)|Контролирует возможность использования функций по борьбе с подменой для распознавания лиц на поддерживаемых устройствах. Если установлено отключение, не допускаются функции по борьбе с спуфингом. Если установлено, что не настроено, пользователь может выбрать, следует ли использовать подмену. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|securityKeyForSignIn|[включить](../resources/intune-shared-enablement.md)|Ключ безопасности для входной точки обеспечивает возможность удаленного отключения windows Hello Sercurity Keyl, не настроенного, будет соблюдать конфигурации, которые делаются на clinet. Возможные значения: `notConfigured`, `enabled`, `disabled`.|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) в теле отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 729

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "state": "enabled",
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "remotePassportEnabled": true,
  "pinPreviousBlockCount": 5,
  "pinExpirationInDays": 3,
  "enhancedBiometricsState": "enabled",
  "securityKeyForSignIn": "enabled"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 901

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
  "id": "3068e0cd-e0cd-3068-cde0-6830cde06830",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "state": "enabled",
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "remotePassportEnabled": true,
  "pinPreviousBlockCount": 5,
  "pinExpirationInDays": 3,
  "enhancedBiometricsState": "enabled",
  "securityKeyForSignIn": "enabled"
}
```




