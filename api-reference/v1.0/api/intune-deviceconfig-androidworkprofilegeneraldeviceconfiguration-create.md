---
title: Создание androidWorkProfileGeneralDeviceConfiguration
description: Создайте новый объект AndroidWorkProfileGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e4e2734eec245a06afa96e1199952cb214558a4c
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2021
ms.locfileid: "60457108"
---
# <a name="create-androidworkprofilegeneraldeviceconfiguration"></a>Создание androidWorkProfileGeneralDeviceConfiguration

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создайте новый [объект AndroidWorkProfileGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса предоставляем представление JSON для объекта AndroidWorkProfileGeneralDeviceConfiguration.

В следующей таблице показаны свойства, необходимые при создании androidWorkProfileGeneralDeviceConfiguration.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|passwordBlockFingerprintUnlock|Boolean|Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.|
|passwordBlockTrustAgents|Boolean|Указывает, следует ли блокировать Smart Lock и другие агенты безопасности.|
|passwordExpirationDays|Int32|Количество дней до окончания срока действия пароля. Допустимые значения: от 1 до 365.|
|passwordMinimumLength|Int32|Минимальная длина паролей. Допустимые значения: от 4 до 16.|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Время с момента последнего действия до отключения экрана (в минутах).|
|passwordPreviousPasswordBlockCount|Int32|Количество предыдущих паролей, которые следует заблокировать. Допустимые значения: от 0 до 24.|
|passwordSignInFailureCountBeforeFactoryReset|Int32|Количество неудачных попыток входа до восстановления заводских настроек. Допустимые значения от 1 до 16|
|passwordRequiredType|[androidWorkProfileRequiredPasswordType](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|Требуемый тип пароля. Возможные значения: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.|
|workProfileDataSharingType|[androidWorkProfileCrossProfileDataSharingType](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|Тип разрешенного обмена данными. Возможные значения: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.|
|workProfileBlockNotificationsWhileDeviceLocked|Логический|Указывает, следует ли блокировать уведомления во время блокировки устройства.|
|workProfileBlockAddingAccounts|Логический|Блокировать добавление и удаление учетных записей в профиле работы.|
|workProfileBluetoothEnableContactSharing|Логический|Разрешить устройствам Bluetooth доступ к корпоративным контактам.|
|workProfileBlockScreenCapture|Логический|Блокировка захвата экрана в профиле работы.|
|workProfileBlockCrossProfileCallerId|Логический|Блокировка ИД вызываемой личности вызываемой на экране работы в личном профиле.|
|workProfileBlockCamera|Логический|Блокировка камеры профиля работы.|
|workProfileBlockCrossProfileContactsSearch|Логический|Блокировка доступности контактов профилей работы в личном профиле.|
|workProfileBlockCrossProfileCopyPaste|Логический|Boolean, который указывает, включен ли параметр, который не позволяет копировать/вклеить перекрестный профиль.|
|workProfileDefaultAppPermissionPolicy|[androidWorkProfileDefaultAppPermissionPolicyType](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|Требуемый тип пароля. Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.|
|workProfilePasswordBlockFingerprintUnlock|Логический|Указывает, следует ли блокировать разблокировку отпечатков пальцев для профиля работы.|
|workProfilePasswordBlockTrustAgents|Логический|Указывает, следует ли блокировать Smart Lock и другие агенты доверия для профиля работы.|
|workProfilePasswordExpirationDays|Int32|Количество дней до истечения срока действия пароля профиля работы. Допустимые значения: от 1 до 365.|
|workProfilePasswordMinimumLength|Int32|Минимальная длина пароля профиля работы. Допустимые значения: от 4 до 16.|
|workProfilePasswordMinNumericCharacters|Int32|Минимум # числимые символы, необходимые в пароле профиля работы. Допустимые значения от 1 до 10|
|workProfilePasswordMinNonLetterCharacters|Int32|Минимальное количество символов без букв, необходимых в пароле профиля работы. Допустимые значения от 1 до 10|
|workProfilePasswordMinLetterCharacters|Int32|Минимальный # буквы символов, необходимых в пароле профиля работы. Допустимые значения от 1 до 10|
|workProfilePasswordMinLowerCaseCharacters|Int32|Минимальное количество символов нижнего уровня, необходимых для пароля профиля работы. Допустимые значения от 1 до 10|
|workProfilePasswordMinUpperCaseCharacters|Int32|Минимальный # символов верхнего уровня, необходимых в пароле профиля работы. Допустимые значения от 1 до 10|
|workProfilePasswordMinSymbolCharacters|Int32|Минимальный # символов, необходимых в пароле профиля работы. Допустимые значения от 1 до 10|
|workProfilePasswordMinutesOfInactivityBeforeScreenTimeout|Int32|Время с момента последнего действия до отключения экрана (в минутах).|
|workProfilePasswordPreviousPasswordBlockCount|Int32|Количество предыдущих паролей профилей работы для блокировки. Допустимые значения: от 0 до 24.|
|workProfilePasswordSignInFailureCountBeforeFactoryReset|Int32|Количество входов в сбои, разрешенные до удаления профиля работы и удаления всех корпоративных данных. Допустимые значения от 1 до 16|
|workProfilePasswordRequiredType|[androidWorkProfileRequiredPasswordType](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|Тип необходимого пароля профиля работы. Возможные значения: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.|
|workProfileRequirePassword|Логический|Пароль требуется или не требуется для профиля работы|
|securityRequireVerifyApps|Boolean|Указывает, что требуется включить функцию проверки приложений для Android.|



## <a name="response"></a>Ответ
В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект AndroidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) в теле отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1831

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "lowSecurityBiometric",
  "workProfileDataSharingType": "preventAny",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "prompt",
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinNumericCharacters": 7,
  "workProfilePasswordMinNonLetterCharacters": 9,
  "workProfilePasswordMinLetterCharacters": 6,
  "workProfilePasswordMinLowerCaseCharacters": 9,
  "workProfilePasswordMinUpperCaseCharacters": 9,
  "workProfilePasswordMinSymbolCharacters": 6,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
  "workProfilePasswordPreviousPasswordBlockCount": 13,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "lowSecurityBiometric",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2003

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
  "id": "6decda7e-da7e-6dec-7eda-ec6d7edaec6d",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "lowSecurityBiometric",
  "workProfileDataSharingType": "preventAny",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "prompt",
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinNumericCharacters": 7,
  "workProfilePasswordMinNonLetterCharacters": 9,
  "workProfilePasswordMinLetterCharacters": 6,
  "workProfilePasswordMinLowerCaseCharacters": 9,
  "workProfilePasswordMinUpperCaseCharacters": 9,
  "workProfilePasswordMinSymbolCharacters": 6,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
  "workProfilePasswordPreviousPasswordBlockCount": 13,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "lowSecurityBiometric",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true
}
```



