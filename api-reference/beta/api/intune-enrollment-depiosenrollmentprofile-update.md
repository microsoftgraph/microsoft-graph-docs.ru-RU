---
title: Обновление depIOSEnrollmentProfile
description: Обновление свойств объекта depIOSEnrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a19dbe9fc3e4cb669fb729804006f0d07a14e3f4
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209235"
---
# <a name="update-depiosenrollmentprofile"></a>Обновление depIOSEnrollmentProfile

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementServiceConfig.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementServiceConfig.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса добавьте представление объекта [depIOSEnrollmentProfile в формате](../resources/intune-enrollment-depiosenrollmentprofile.md) JSON.

В следующей таблице показаны свойства, необходимые при создании [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|GUID объекта, унаследованного от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|displayName|Строка|Имя профиля, унаследованного от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|description|Строка|Описание профиля, унаследованного от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requiresUserAuthentication|Логический|Указывает, требуется ли для профиля проверка подлинности пользователя, унаследованного от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|configurationEndpointUrl|Строка|URL-адрес конечной точки конфигурации для регистрации, унаследованного от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|enableAuthenticationViaCompanyPortal|Логическое|Указывает на проверку подлинности с помощью помощника по настройке Apple вместо Корпоративный портал. Наследуется [от enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Логический|Указывает, что Корпоративный портал на зарегистрированных устройствах помощника по настройке, унаследованных от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|isDefault|Boolean|Указывает, является ли этот профиль профилем по умолчанию, унаследованным от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|supervisedModeEnabled|Логическое|Защищенный режим, значение True для включения, значение false в противном случае. Дополнительные https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune сведения см. в этой статье. Наследуется [от depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|supportDepartment|Строка|Сведения о отделе поддержки, унаследованные [от depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|isMandatory|Логический|Указывает, является ли профиль обязательным наследованием [от depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|locationDisabled|Логический|Указывает, отключена ли область установки службы location Inherited от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|supportPhoneNumber|Строка|Номер телефона службы поддержки, унаследованный от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|profileRemovalDisabled|Логическое|Указывает, отключен ли параметр удаления профиля Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md).|
|restoreBlocked|Логический|Указывает, заблокирована ли область установки восстановления. Наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|appleIdDisabled|Логический|Указывает, отключена ли область установки идентификатора Apple Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md).|
|termsAndConditionsDisabled|Логический|Указывает, отключена ли область установки "Условия". Наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|touchIdDisabled|Логический|Указывает, отключена ли панель установки touch id Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|applePayDisabled|Логический|Указывает, отключена ли область настройки apple Pay Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|siriDisabled|Логический|Указывает, отключена ли область установки siri Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|diagnosticsDisabled|Логический|Указывает, отключена ли область настройки диагностики Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|displayToneSetupDisabled|Логический|Указывает, отключен ли экран установки displaytone inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|privacyPaneDisabled|Логическое|Указывает, отключен ли экран конфиденциальности Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|screenTimeScreenDisabled|Логический|Указывает, отключена ли настройка времени ожидания экрана . Наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|deviceNameTemplate|Строка|Задает литерал или шаблон имени. Наследуется [от depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|configurationWebUrl|Логический|URL-адрес для входа помощника по настройке, унаследованный от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|iTunesPairingMode|[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md)|Указывает режим связывания iTunes. Возможные значения: `disallow`, `allow`, `requiresCertificate`.|
|managementCertificates|[Коллекция managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)|Сертификаты управления для Apple Configurator|
|restoreFromAndroidDisabled|Логическое|Указывает, отключено ли восстановление из Android|
|awaitDeviceConfiguredConfirmation|Логическое|Указывает, нужно ли устройству ждать настроенного подтверждения.|
|sharedIPadMaximumUserCount|Int32|Указывает максимальное число пользователей, которые могут использовать общий iPad. Применимо только в режиме общего iPad.|
|enableSharedIPad|Логическое|Это указывает, должно ли устройство быть зарегистрировано в режиме, который включает сценарии с несколькими пользователями. Применимо только на общих устройствах iPad.|
|companyPortalVppTokenId|Строка|Если задано, указывает, какой токен Vpp следует использовать для развертывания Корпоративный портал w/device licensing. Чтобы задать это свойство, необходимо задать параметр enableAuthenticationViaCompanyPortal.|
|enableSingleAppEnrollmentMode|Логическое|Указывает устройству включить режим одного приложения и применить блокировку приложения во время регистрации. Значение по умолчанию: false. Для задания этого свойства необходимо задать параметры enableAuthenticationViaCompanyPortal и companyPortalVppTokenId.|
|homeButtonScreenDisabled|Логический|Указывает, отключен ли экран конфиденциальности кнопки "Главная"|
|iMessageAndFaceTimeScreenDisabled|Логическое|Указывает, отключен ли экран iMessage и FaceTime|
|onBoardingScreenDisabled|Логическое|Указывает, отключен ли экран настройки подключения.|
|simSetupScreenDisabled|Логическое|Указывает, отключен ли экран SIMSetup|
|softwareUpdateScreenDisabled|Логическое|Указывает, отключен ли обязательный экран обновления sofware|
|watchMigrationScreenDisabled|Логическое|Указывает, отключен ли экран переноса контрольных значений|
|appearanceScreenDisabled|Логическое|Указывает, отключен ли экран Apperance|
|ExpressLanguageScreenDisabled|Логическое|Указывает, отключен ли экран express Language|
|preferredLanguageScreenDisabled|Логическое|Указывает, отключен ли экран предпочитаемого языка|
|deviceToDeviceMigrationDisabled|Логическое|Указывает, отключена ли миграция с устройства на устройство|
|welcomeScreenDisabled|Логическое|Указывает, отключен ли экран Weclome|
|passCodeDisabled|Логическое|Указывает, отключена ли область установки секретного кода|
|zoomDisabled|Логическое|Указывает, отключена ли область настройки масштабирования|
|restoreCompletedScreenDisabled|Логическое|Указывает, отключен ли экран Weclome|
|updateCompleteScreenDisabled|Логическое|Указывает, отключен ли экран Weclome|
|forceTemporarySession|Логическое|Указывает, включены ли временные сеансы|
|temporarySessionTimeoutInSeconds|Int32|Указывает время ожидания временного сеанса|
|userSessionTimeoutInSeconds|Int32|Указывает время ожидания временного сеанса|
|секретный кодLockGracePeriodInSeconds|Int32|Указывает время ожидания перед блокировкой экрана, когда пользователь должен ввести парольную передачу устройства, чтобы разблокировать его.|
|carrierActivationUrl|Строка|URL-адрес оператора для активации устройства eSIM.|
|userlessSharedAadModeEnabled|Логическое|Указывает, что это устройство Apple предназначено для поддержки сценариев режима общего устройства. Это отличается от сценария "общий iPad". См. https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-shared-ios|



## <a name="response"></a>Ответ
В случае успешного выполнения этот `200 OK` метод возвращает код отклика и обновленный объект [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) в теле отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
Content-type: application/json
Content-length: 2377

{
  "@odata.type": "#microsoft.graph.depIOSEnrollmentProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true,
  "isDefault": true,
  "supervisedModeEnabled": true,
  "supportDepartment": "Support Department value",
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "Support Phone Number value",
  "profileRemovalDisabled": true,
  "restoreBlocked": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "displayToneSetupDisabled": true,
  "privacyPaneDisabled": true,
  "screenTimeScreenDisabled": true,
  "deviceNameTemplate": "Device Name Template value",
  "configurationWebUrl": true,
  "iTunesPairingMode": "allow",
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "Thumbprint value",
      "certificate": "Certificate value"
    }
  ],
  "restoreFromAndroidDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 10,
  "enableSharedIPad": true,
  "companyPortalVppTokenId": "Company Portal Vpp Token Id value",
  "enableSingleAppEnrollmentMode": true,
  "homeButtonScreenDisabled": true,
  "iMessageAndFaceTimeScreenDisabled": true,
  "onBoardingScreenDisabled": true,
  "simSetupScreenDisabled": true,
  "softwareUpdateScreenDisabled": true,
  "watchMigrationScreenDisabled": true,
  "appearanceScreenDisabled": true,
  "expressLanguageScreenDisabled": true,
  "preferredLanguageScreenDisabled": true,
  "deviceToDeviceMigrationDisabled": true,
  "welcomeScreenDisabled": true,
  "passCodeDisabled": true,
  "zoomDisabled": true,
  "restoreCompletedScreenDisabled": true,
  "updateCompleteScreenDisabled": true,
  "forceTemporarySession": true,
  "temporarySessionTimeoutInSeconds": 0,
  "userSessionTimeoutInSeconds": 11,
  "passcodeLockGracePeriodInSeconds": 0,
  "carrierActivationUrl": "https://example.com/carrierActivationUrl/",
  "userlessSharedAadModeEnabled": true
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2426

{
  "@odata.type": "#microsoft.graph.depIOSEnrollmentProfile",
  "id": "1ec10a60-0a60-1ec1-600a-c11e600ac11e",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true,
  "isDefault": true,
  "supervisedModeEnabled": true,
  "supportDepartment": "Support Department value",
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "Support Phone Number value",
  "profileRemovalDisabled": true,
  "restoreBlocked": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "displayToneSetupDisabled": true,
  "privacyPaneDisabled": true,
  "screenTimeScreenDisabled": true,
  "deviceNameTemplate": "Device Name Template value",
  "configurationWebUrl": true,
  "iTunesPairingMode": "allow",
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "Thumbprint value",
      "certificate": "Certificate value"
    }
  ],
  "restoreFromAndroidDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 10,
  "enableSharedIPad": true,
  "companyPortalVppTokenId": "Company Portal Vpp Token Id value",
  "enableSingleAppEnrollmentMode": true,
  "homeButtonScreenDisabled": true,
  "iMessageAndFaceTimeScreenDisabled": true,
  "onBoardingScreenDisabled": true,
  "simSetupScreenDisabled": true,
  "softwareUpdateScreenDisabled": true,
  "watchMigrationScreenDisabled": true,
  "appearanceScreenDisabled": true,
  "expressLanguageScreenDisabled": true,
  "preferredLanguageScreenDisabled": true,
  "deviceToDeviceMigrationDisabled": true,
  "welcomeScreenDisabled": true,
  "passCodeDisabled": true,
  "zoomDisabled": true,
  "restoreCompletedScreenDisabled": true,
  "updateCompleteScreenDisabled": true,
  "forceTemporarySession": true,
  "temporarySessionTimeoutInSeconds": 0,
  "userSessionTimeoutInSeconds": 11,
  "passcodeLockGracePeriodInSeconds": 0,
  "carrierActivationUrl": "https://example.com/carrierActivationUrl/",
  "userlessSharedAadModeEnabled": true
}
```




