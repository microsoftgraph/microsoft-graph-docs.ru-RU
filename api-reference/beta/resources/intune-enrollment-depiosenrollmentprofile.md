---
title: Тип ресурса depIOSEnrollmentProfile
description: Ресурс DepIOSEnrollmentProfile представляет профиль регистрации программы регистрации устройств Apple (DEP), относщийся к конфигурации iOS. Этот тип профиля необходимо назначить серийным номерам Apple DEP, прежде чем соответствующие устройства могут зарегистрироваться через DEP.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b2f8055409be315ffd1b5ba2fb3686655b334ba8
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65210754"
---
# <a name="depiosenrollmentprofile-resource-type"></a>Тип ресурса depIOSEnrollmentProfile

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс DepIOSEnrollmentProfile представляет профиль регистрации программы регистрации устройств Apple (DEP), относщийся к конфигурации iOS. Этот тип профиля необходимо назначить серийным номерам Apple DEP, прежде чем соответствующие устройства могут зарегистрироваться через DEP.


Наследуется [от depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление depIOSEnrollmentProfiles](../api/intune-enrollment-depiosenrollmentprofile-list.md)|[Коллекция depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)|Список свойств и связей объектов [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) .|
|[Получение depIOSEnrollmentProfile](../api/intune-enrollment-depiosenrollmentprofile-get.md)|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)|Чтение свойств и связей объекта [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) .|
|[Создание depIOSEnrollmentProfile](../api/intune-enrollment-depiosenrollmentprofile-create.md)|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)|Создайте объект [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) .|
|[Удаление depIOSEnrollmentProfile](../api/intune-enrollment-depiosenrollmentprofile-delete.md)|Нет|Удаляет [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md).|
|[Обновление depIOSEnrollmentProfile](../api/intune-enrollment-depiosenrollmentprofile-update.md)|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)|Обновление свойств объекта [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|GUID объекта, унаследованного от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|displayName|Строка|Имя профиля, унаследованного от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|description|Строка|Описание профиля, унаследованного от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requiresUserAuthentication|Логический|Указывает, требуется ли для профиля проверка подлинности пользователя, унаследованного от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|configurationEndpointUrl|Строка|URL-адрес конечной точки конфигурации для регистрации, унаследованного от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|enableAuthenticationViaCompanyPortal|Логический|Указывает на проверку подлинности с помощью помощника по настройке Apple вместо Корпоративный портал. Наследуется [от enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Логический|Указывает, что Корпоративный портал на зарегистрированных устройствах помощника по настройке, унаследованных от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|isDefault|Boolean|Указывает, является ли этот профиль профилем по умолчанию, унаследованным от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|supervisedModeEnabled|Логическое|Защищенный режим, значение True для включения, значение false в противном случае. Дополнительные https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune сведения см. в этой статье. Наследуется [от depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|supportDepartment|Строка|Сведения о отделе поддержки, унаследованные [от depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|isMandatory|Логический|Указывает, является ли профиль обязательным наследованием [от depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|locationDisabled|Логическое|Указывает, отключена ли область установки службы location Inherited от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|supportPhoneNumber|Строка|Номер телефона службы поддержки, унаследованный от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|profileRemovalDisabled|Логическое|Указывает, отключен ли параметр удаления профиля Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md).|
|restoreBlocked|Логическое|Указывает, заблокирована ли область установки восстановления. Наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|appleIdDisabled|Логический|Указывает, отключена ли область установки идентификатора Apple Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md).|
|termsAndConditionsDisabled|Логический|Указывает, отключена ли область установки "Условия". Наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|touchIdDisabled|Логический|Указывает, отключена ли панель установки touch id Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|applePayDisabled|Логическое|Указывает, отключена ли область настройки apple Pay Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|siriDisabled|Логическое|Указывает, отключена ли область установки siri Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|diagnosticsDisabled|Логический|Указывает, отключена ли область настройки диагностики Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|displayToneSetupDisabled|Логическое|Указывает, отключен ли экран установки displaytone inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
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
|enableSingleAppEnrollmentMode|Логический|Указывает устройству включить режим одного приложения и применить блокировку приложения во время регистрации. Значение по умолчанию: false. Для задания этого свойства необходимо задать параметры enableAuthenticationViaCompanyPortal и companyPortalVppTokenId.|
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

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.depIOSEnrollmentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.depIOSEnrollmentProfile",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "String",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true,
  "isDefault": true,
  "supervisedModeEnabled": true,
  "supportDepartment": "String",
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "String",
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
  "deviceNameTemplate": "String",
  "configurationWebUrl": true,
  "iTunesPairingMode": "String",
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "String",
      "certificate": "String"
    }
  ],
  "restoreFromAndroidDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 1024,
  "enableSharedIPad": true,
  "companyPortalVppTokenId": "String",
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
  "temporarySessionTimeoutInSeconds": 1024,
  "userSessionTimeoutInSeconds": 1024,
  "passcodeLockGracePeriodInSeconds": 1024,
  "carrierActivationUrl": "String",
  "userlessSharedAadModeEnabled": true
}
```




