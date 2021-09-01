---
title: Создание depIOSEnrollmentProfile
description: Создание нового объекта depIOSEnrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3d5ea9ce1b919e00257734fb66ba048ac02e2c12
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58765185"
---
# <a name="create-depiosenrollmentprofile"></a>Создание depIOSEnrollmentProfile

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового [объекта depIOSEnrollmentProfile.](../resources/intune-enrollment-depiosenrollmentprofile.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementServiceConfig.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Application|DeviceManagementServiceConfig.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для объекта depIOSEnrollmentProfile.

В следующей таблице показаны свойства, необходимые при создании depIOSEnrollmentProfile.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|GUID для объекта Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|displayName|Строка|Имя профиля, унаследованной от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|description|String|Описание профиля, унаследованной от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requiresUserAuthentication|Логический|Указывает, требует ли профиль проверки подлинности пользователя, унаследованной от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|configurationEndpointUrl|String|URL-адрес конечной точки конфигурации для использования для регистрации, унаследованной [от enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|enableAuthenticationViaCompanyPortal|Boolean|Указывает на проверку подлинности с помощью помощника установки Apple вместо Корпоративный портал. Унаследованный от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Логический|Указывает, Корпоративный портал требуется на устройствах, зарегистрированных помощником установки, унаследованных от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|isDefault|Boolean|Указывает, является ли это профилем по умолчанию, унаследованной от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|supervisedModeEnabled|Логический|Режим Под контролем, True, чтобы включить, ложные в противном случае. Дополнительные https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune сведения см. в дополнительных сведениях. Унаследованный от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|supportDepartment|String|Сведения отдела поддержки, унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|isMandatory|Логический|Указывает, является ли профиль обязательным, унаследованный от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|locationDisabled|Boolean|Указывает, отключено ли области установки службы расположения из [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|supportPhoneNumber|String|Номер телефона поддержки, унаследованный от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|profileRemovalDisabled|Boolean|Указывает, отключен ли параметр удаления профиля, унаследованный от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|restoreBlocked|Логический|Указывает, заблокирована ли настройка области восстановления, наследуемая [от depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|appleIdDisabled|Boolean|Указывает, отключена ли система установки apple id Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|termsAndConditionsDisabled|Логический|Указывает, отключено ли области установки "Условия и условия", унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|touchIdDisabled|Boolean|Указывает, отключена ли для настройки сенсорного id наследуемая из [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|applePayDisabled|Логический|Указывает, отключена ли система установки apple pay inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|siriDisabled|Логический|Указывает, отключена ли настройка siri из [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|diagnosticsDisabled|Логический|Указывает, отключено ли области настройки диагностики, унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|displayToneSetupDisabled|Логический|Указывает, отключен ли экран настройки displaytone, унаследованный от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|privacyPaneDisabled|Логический|Указывает, отключен ли экран конфиденциальности, унаследованный от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|screenTimeScreenDisabled|Логический|Указывает, отключена ли установка расстановки времени на экране, наследуемая [из depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|deviceNameTemplate|Строка|Задает буквальный или имя шаблон. Унаследованный от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|configurationWebUrl|Логический|URL-адрес для входа помощника установки, унаследованный от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|iTunesPairingMode|[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md).|Указывает режим сопряжения iTunes. Возможные значения: `disallow`, `allow`, `requiresCertificate`.|
|managementCertificates|[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection|Сертификаты управления для Apple Configurator|
|restoreFromAndroidDisabled|Логический|Указывает, отключено ли восстановление с Android|
|awaitDeviceConfiguredConfirmation|Логический|Указывает, нужно ли устройству ждать настроенного подтверждения|
|sharedIPadMaximumUserCount|Int32|Это указывает максимальное число пользователей, которые могут использовать общие iPad. Применимо только в iPad режиме.|
|enableSharedIPad|Логический|Это указывает, должно ли устройство быть зарегистрированным в режиме, который включает несколько сценариев пользователей. Применимо только в общих iPads.|
|companyPortalVppTokenId|Строка|Если установлено, указывается, какой маркер Vpp следует использовать для развертывания Корпоративный портал w/device licensing. Для этого свойства необходимо установить "enableAuthenticationViaCompanyPortal".|
|enableSingleAppEnrollmentMode|Boolean|Сообщает устройству включить режим одного приложения и применить блокировку приложения во время регистрации. Значение по умолчанию: false. Для этого свойства необходимо установить "enableAuthenticationViaCompanyPortal" и "companyPortalVppTokenId".|
|homeButtonScreenDisabled|Логический|Указывает, отключен ли экран чувствительности домашней кнопки|
|iMessageAndFaceTimeScreenDisabled|Boolean|Указывает, отключен ли экран iMessage и FaceTime|
|onBoardingScreenDisabled|Логический|Указывает, отключен ли экран установки бортовой установки|
|simSetupScreenDisabled|Boolean|Указывает, отключен ли экран SIMSetup|
|softwareUpdateScreenDisabled|Логический|Указывает, отключен ли экран обязательного обновления sofware|
|watchMigrationScreenDisabled|Boolean|Указывает, отключен ли экран переноса часов|
|appearanceScreenDisabled|Логический|Указывает, отключен ли экран Apperance|
|expressLanguageScreenDisabled|Логический|Указывает, отключен ли экран express Language|
|preferredLanguageScreenDisabled|Логический|Указывает, отключен ли предпочтительный языковой экран|
|deviceToDeviceMigrationDisabled|Логический|Указывает, отключена ли миграция устройства на устройство|
|welcomeScreenDisabled|Логический|Указывает, отключен ли экран Weclome|
|passCodeDisabled|Логический|Указывает отключение области установки passcode|
|zoomDisabled|Логический|Указывает, отключена ли панорама настройки масштабирования|
|restoreCompletedScreenDisabled|Boolean|Указывает, отключен ли экран Weclome|
|updateCompleteScreenDisabled|Логический|Указывает, отключен ли экран Weclome|
|forceTemporarySession|Логический|Указывает, включены ли временные сеансы|
|temporarySessionTimeoutInSeconds|Int32|Указывает время времени временного сеанса|
|userSessionTimeoutInSeconds|Int32|Указывает время времени временного сеанса|
|passcodeLockGracePeriodInSeconds|Int32|Указывает время перед блокировкой экрана, чтобы пользователь вошел в пасокд устройства, чтобы разблокировать его|
|carrierActivationUrl|Строка|URL-адрес carrier для активации eSIM устройства.|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код ответа и `201 Created` [объект depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
Content-type: application/json
Content-length: 2336

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
  "carrierActivationUrl": "https://example.com/carrierActivationUrl/"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2385

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
  "carrierActivationUrl": "https://example.com/carrierActivationUrl/"
}
```



