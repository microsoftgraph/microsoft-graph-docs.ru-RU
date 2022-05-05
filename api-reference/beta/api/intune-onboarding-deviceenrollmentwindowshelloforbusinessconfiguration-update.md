---
title: Обновление deviceEnrollmentWindowsHelloForBusinessConfiguration
description: Обновление свойств объекта deviceEnrollmentWindowsHelloForBusinessConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b71dc8ee4bed610c31064c429046d9f07ce06ef5
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212366"
---
# <a name="update-deviceenrollmentwindowshelloforbusinessconfiguration"></a>Обновление deviceEnrollmentWindowsHelloForBusinessConfiguration

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса добавьте представление объекта [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) в формате JSON.

В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор учетной записи, унаследованного от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|displayName|String|Отображаемое имя конфигурации регистрации устройства, унаследованного от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|description|Строка|Описание конфигурации регистрации устройства, унаследованного от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|priority|Int32|Приоритет используется, когда пользователь существует в нескольких группах, для которых назначена конфигурация регистрации. На пользователей распространяется только конфигурация с наименьшим значением приоритета. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|createdDateTime|DateTimeOffset|Дата создания в формате UTC конфигурации регистрации устройства, унаследованного от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|Дата последнего изменения в формате UTC конфигурации регистрации устройства, унаследованного от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|version|Int32|Версия конфигурации регистрации устройства, унаследованного от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|Идентификаторы roleScopeTagId|Коллекция объектов string|Необязательные теги области роли для ограничений регистрации. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|DeviceEnrollmentConfigurationType|[DeviceEnrollmentConfigurationType](../resources/intune-onboarding-deviceenrollmentconfigurationtype.md)|Поддержка типа конфигурации регистрации, унаследованного [от deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md). Возможные значения: `unknown`, `limit`, `platformRestrictions`, `windowsHelloForBusiness`, `defaultLimit`, `defaultPlatformRestrictions`, `defaultWindowsHelloForBusiness`, `defaultWindows10EnrollmentCompletionPageConfiguration`, `windows10EnrollmentCompletionPageConfiguration`, `deviceComanagementAuthorityConfiguration`, `singlePlatformRestriction`, `unknownFutureValue`, `enrollmentNotificationsConfiguration`.|
|pinMinimumLength|Int32|Управляет минимальным количеством символов, необходимых для Windows Hello для бизнеса ПИН-кода.  Это значение должно быть в диапазоне от 4 до 127 включительно и меньше или равно значению, заданного для максимального ПИН-кода.|
|pinMaximumLength|Int32|Управляет максимальным количеством символов, разрешенных для Windows Hello для бизнеса ПИН-кода. Это значение должно быть в диапазоне от 4 до 127 включительно. Это значение должно быть больше или равно значению, заданным для минимального ПИН-кода.|
|pinUppercaseCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|Управляет возможностью использовать прописные буквы в Windows Hello для бизнеса ПИН-коде.  Разрешено использовать прописные буквы, в то время как обязательное гарантирует, что они присутствуют. Если задано значение "Запрещено", прописные буквы не будут разрешены. Возможные значения: `allowed`, `required`, `disallowed`.|
|pinLowercaseCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|Управляет возможностью использовать строчные буквы в Windows Hello для бизнеса ПИН-коде.  Разрешено использовать строчные буквы, в то время как обязательное гарантирует, что они присутствуют. Если задано значение "Запрещено", строчные буквы не будут разрешены. Возможные значения: `allowed`, `required`, `disallowed`.|
|pinSpecialCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|Управляет возможностью использовать специальные символы в Windows Hello для бизнеса ПИН-коде.  Разрешено использовать специальные символы, в то время как обязательное гарантирует, что они присутствуют. Если задано значение "Запрещено", специальные символы не будут разрешены. Возможные значения: `allowed`, `required`, `disallowed`.|
|state|[Включения](../resources/intune-shared-enablement.md)|Определяет, следует ли разрешить настройку устройства для Windows Hello для бизнеса. Если задано значение "Отключено", пользователь не может подготовить Windows Hello для бизнеса, за исключением Azure Active Directory мобильных телефонов, если это необходимо. Если задано значение "Не настроено", Intune не будут переопределять значения по умолчанию для клиента. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|securityDeviceRequired|Boolean|Определяет, требуется ли доверенный платформенный модуль (TPM) для подготовки Windows Hello для бизнеса. TPM предоставляет дополнительное преимущество безопасности в том, что хранящиеся на нем данные не могут использоваться на других устройствах. Если задано значение False, все устройства могут Windows Hello для бизнеса, даже если нет доверенного платформенного модуля.|
|unlockWithBiometricsEnabled|Boolean|Управляет использованием биометрических жестов, таких как лицо и отпечаток пальца, в качестве альтернативы Windows Hello для бизнеса ПИН-коду.  Если задано значение False, биометрические жесты не допускаются. Пользователи по-прежнему должны настраивать ПИН-код в качестве резервной копии в случае сбоев.|
|remotePassportEnabled|Boolean|Управляет использованием удаленного Windows Hello для бизнеса. Удаленные Windows Hello для бизнеса позволяют использовать переносимое зарегистрированное устройство в качестве компаньона для проверки подлинности на рабочем столе. Рабочий стол должен быть Azure AD, а устройство-компаньон должно иметь Windows Hello для бизнеса ПИН-код.|
|pinPreviousBlockCount|Int32|Управляет возможностью запретить пользователям использовать прошлые ПИН-коды. Это значение должно быть задано в диапазоне от 0 до 50 включительно, и текущий ПИН-код пользователя будет включен в это число. Если задано значение 0, предыдущие ПИН-коды не сохраняются. Журнал ПИН-кодов не сохраняется при сбросе ПИН-кода.|
|pinExpirationInDays|Int32|Управляет периодом времени (в днях), в течение которого ПИН-код может использоваться до того, как система требует от пользователя изменить его. Это значение должно быть задано в диапазоне от 0 до 730 включительно. Если задано значение 0, пин-код пользователя никогда не истечет|
|enhancedBiometricsState|[Включения](../resources/intune-shared-enablement.md)|Управляет возможностью использовать функции защиты от спуфинга для распознавания лиц на устройствах, которые ее поддерживают. Если задано значение "Отключено", функции защиты от спуфинга не допускаются. Если задано значение "Не настроено", пользователь может выбрать, следует ли использовать защиту от спуфинга. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|securityKeyForSignIn|[Включения](../resources/intune-shared-enablement.md)|Ключ безопасности для входа предоставляет емкость для удаленного включения и отключения Windows Hello Sercurity Keyl Not configured будет учитывать конфигурации, выполняемые в CLINET. Возможные значения: `notConfigured`, `enabled`, `disabled`.|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) в теле отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 778

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "deviceEnrollmentConfigurationType": "limit",
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
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 950

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
  "deviceEnrollmentConfigurationType": "limit",
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




