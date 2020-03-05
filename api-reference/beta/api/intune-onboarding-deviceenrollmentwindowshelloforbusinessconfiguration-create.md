---
title: Создание deviceEnrollmentWindowsHelloForBusinessConfiguration
description: Создание объекта deviceEnrollmentWindowsHelloForBusinessConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f0ab9872746b356285de0ebf965d1367080492b4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42462385"
---
# <a name="create-deviceenrollmentwindowshelloforbusinessconfiguration"></a>Создание deviceEnrollmentWindowsHelloForBusinessConfiguration

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание объекта [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementServiceConfig.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementServiceConfig.ReadWrite.All|

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
|id|String|Уникальный идентификатор для учетной записи, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|displayName|Строка|Отображаемое имя конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|description|String|Описание конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|priority|Int32|Priority используется, когда пользователь существует в нескольких группах, которым назначена Настройка регистрации. Пользователи подчиняются только конфигурации с наименьшим значением приоритета. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|createdDateTime|DateTimeOffset|Созданная Дата и время в формате UTC для настройки регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|version|Int32|Версия конфигурации регистрации устройств, унаследованная от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|pinMinimumLength|Int32|Определяет минимальное количество символов, необходимое для ПИН-кода Windows Hello для бизнеса.  Это значение должно находиться в диапазоне от 4 до 127 включительно, и меньше или равно значению, заданному для максимального ПИН-кода.|
|pinMaximumLength|Int32|Управляет максимальным количеством символов для ПИН-кода Windows Hello для бизнеса. Это значение должно находиться в диапазоне от 4 до 127 включительно. Это значение должно быть больше или равно значению, заданному для минимального ПИН-кода.|
|pinUppercaseCharactersUsage|[виндовшеллофорбусинесспинусаже](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|Управляет возможностью использования прописных букв в ПИН-коде Windows Hello для бизнеса.  Allows разрешает использование прописных букв (s), в то время как это необходимо. Если задано значение "не разрешено", прописные буквы не будут разрешены. Возможные значения: `allowed`, `required`, `disallowed`.|
|pinLowercaseCharactersUsage|[виндовшеллофорбусинесспинусаже](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|Управляет возможностью использования строчных букв в ПИН-коде Windows Hello для бизнеса.  Allows разрешает использование строчных букв (s), в то время как это необходимо. Если задано значение "не разрешено", буквы нижнего регистра не будут разрешены. Возможные значения: `allowed`, `required`, `disallowed`.|
|pinSpecialCharactersUsage|[виндовшеллофорбусинесспинусаже](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|Управляет возможностью использования специальных символов в ПИН-коде Windows Hello для бизнеса.  Allows разрешает использование специальных символов, в то время как они необходимы для их отображения. Если задано значение "не разрешено", Специальные символы не будут разрешены. Возможные значения: `allowed`, `required`, `disallowed`.|
|state|[Включение](../resources/intune-shared-enablement.md)|Определяет, разрешено ли настраивать устройство для Windows Hello для бизнеса. Если задано значение Disabled, пользователь не сможет подготовить Windows Hello для бизнеса, за исключением того, что в Azure Active Directory присоединяются мобильные телефоны, если это необходимо. Если задано значение не задано, Intune не будет переопределять значения по умолчанию для клиента. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|securityDeviceRequired|Логический|Определяет, требуется ли доверенный ПЛАТФОРМЕНный модуль для подготовки Windows Hello для бизнеса. TPM предоставляет дополнительные преимущества безопасности, которые хранятся на нем, не могут использоваться на других устройствах. Если задано значение false, все устройства могут подготавливать Windows Hello для бизнеса, даже если нет пригодного к использованию доверенного платформенного модуля.|
|unlockWithBiometricsEnabled|Логический|Управляет использованием биометрических жестов, таких как лицо и отпечаток, в качестве альтернативы ПИН-коду Windows Hello для бизнеса.  Если задано значение false, биометрические жесты не разрешены. Пользователи по-прежнему должны настроить ПИН-код в качестве резервной копии в случае сбоев.|
|remotePassportEnabled|Boolean|Управляет использованием удаленного Windows Hello для бизнеса. Удаленная функция Windows Hello для бизнеса обеспечивает возможность использования портативного, зарегистрированного устройства в качестве вспомогательного для проверки подлинности на настольных компьютерах. Рабочий стол должен быть присоединен к Azure AD, а на вспомогательном устройстве должен быть ПИН-код Windows Hello для бизнеса.|
|pinPreviousBlockCount|Int32|Управляет возможностью запретить пользователям использовать прошлые контакты. Он должен иметь значение от 0 до 50 включительно, а текущий ПИН-код пользователя включен в этот счетчик. Если задано значение 0, предыдущие ПИН-коды не сохраняются. История ПИН-кодов не сохраняется при сбросе ПИН-кода.|
|pinExpirationInDays|Int32|Определяет период времени (в днях), в течение которого можно использовать ПИН-код, прежде чем система потребует от пользователя изменить его. Должно быть задано значение от 0 до 730 включительно. Если задано значение 0, срок действия ПИН-кода пользователя никогда не истекает|
|enhancedBiometricsState|[Включение](../resources/intune-shared-enablement.md)|Управляет возможностью использования функций защиты от спуфинга для распознавания лиц на поддерживающих его устройствах. Если задано значение Disabled, функции защиты от спуфинга не допускаются. Если задано значение не задано, пользователь может выбрать, следует ли использовать функцию защиты от спуфинга. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|секуритикэйфорсигнин|[Включение](../resources/intune-shared-enablement.md)|Ключ безопасности для входа предоставляет возможность удаленного включения и ВЫКЛЮЧЕНия функции Windows Hello Серкурити Кэйл, которые не настроены, будут поддерживать конфигурации, выполненные в Клинет. Возможные значения: `notConfigured`, `enabled`, `disabled`.|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) в теле отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 667

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
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
Content-Length: 839

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
  "id": "3068e0cd-e0cd-3068-cde0-6830cde06830",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
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





