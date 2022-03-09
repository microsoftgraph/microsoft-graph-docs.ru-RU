---
title: тип ресурса depIOSEnrollmentProfile
description: Ресурс DepIOSEnrollmentProfile представляет профиль регистрации программы регистрации устройств Apple (DEP), специфический для конфигурации iOS. Этот тип профиля должен быть назначен серийным номерам DeP Apple, прежде чем соответствующие устройства смогут зарегистрироваться с помощью DEP.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 38c61aa1f27a13a613e2a2dd062b56ebe03f7ae3
ms.sourcegitcommit: efa06c63cd3154bcc7ecc993011f314c2dea9a92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63367624"
---
# <a name="depiosenrollmentprofile-resource-type"></a>тип ресурса depIOSEnrollmentProfile

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс DepIOSEnrollmentProfile представляет профиль регистрации программы регистрации устройств Apple (DEP), специфический для конфигурации iOS. Этот тип профиля должен быть назначен серийным номерам DeP Apple, прежде чем соответствующие устройства смогут зарегистрироваться с помощью DEP.


Наследует [от depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список depIOSEnrollmentProfiles](../api/intune-enrollment-depiosenrollmentprofile-list.md)|[коллекция depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)|Список свойств и связей объектов [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) .|
|[Получить depIOSEnrollmentProfile](../api/intune-enrollment-depiosenrollmentprofile-get.md)|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)|Чтение свойств и связей объекта [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) .|
|[Создание depIOSEnrollmentProfile](../api/intune-enrollment-depiosenrollmentprofile-create.md)|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)|Создание нового [объекта depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) .|
|[Удаление depIOSEnrollmentProfile](../api/intune-enrollment-depiosenrollmentprofile-delete.md)|Нет|Удаляет [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md).|
|[Обновление depIOSEnrollmentProfile](../api/intune-enrollment-depiosenrollmentprofile-update.md)|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)|Обновление свойств объекта [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|GUID для объекта Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|displayName|Строка|Имя профиля, унаследованной от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|description|String|Описание профиля, унаследованной от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requiresUserAuthentication|Boolean|Указывает, требует ли профиль проверки подлинности пользователя, унаследованной от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|configurationEndpointUrl|Строка|URL-адрес конечной точки конфигурации для использования для регистрации, унаследованной [от enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|enableAuthenticationViaCompanyPortal|Boolean|Указывает на проверку подлинности с помощью помощника установки Apple вместо Корпоративный портал. Унаследованный от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Boolean|Указывает, Корпоративный портал требуется на устройствах, зарегистрированных помощником установки, унаследованных от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|isDefault|Boolean|Указывает, является ли это профилем по умолчанию, унаследованной от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|supervisedModeEnabled|Boolean|Режим Под контролем, True, чтобы включить, ложные в противном случае. Дополнительные сведения см [. в записи устройства Intune](/mem/intune/enrollment/device-enrollment) . Унаследованный от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|supportDepartment|String|Сведения отдела поддержки, унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|isMandatory|Boolean|Указывает, является ли профиль обязательным, унаследованный от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|locationDisabled|Boolean|Указывает, отключено ли области установки службы расположения из [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|supportPhoneNumber|Строка|Номер телефона поддержки, унаследованный от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|profileRemovalDisabled|Boolean|Указывает, отключен ли параметр удаления профиля, унаследованный от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|restoreBlocked|Boolean|Указывает, заблокирована ли настройка области восстановления, наследуемая [от depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|appleIdDisabled|Boolean|Указывает, отключена ли система установки apple id Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|termsAndConditionsDisabled|Boolean|Указывает, отключено ли области установки "Условия и условия", унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|touchIdDisabled|Boolean|Указывает, отключена ли для настройки сенсорного id наследуемая из [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|applePayDisabled|Boolean|Указывает, отключена ли система установки apple pay inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|siriDisabled|Boolean|Указывает, отключена ли настройка siri из [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|diagnosticsDisabled|Boolean|Указывает, отключено ли области настройки диагностики, унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|displayToneSetupDisabled|Boolean|Указывает, отключен ли экран настройки displaytone, унаследованный от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|privacyPaneDisabled|Boolean|Указывает, отключен ли экран конфиденциальности, унаследованный от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|screenTimeScreenDisabled|Boolean|Указывает, отключена ли установка расстановки времени на экране, наследуемая [из depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|deviceNameTemplate|Строка|Задает буквальный или имя шаблон. Унаследованный от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|configurationWebUrl|Boolean|URL-адрес для входа помощника установки, унаследованный от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|iTunesPairingMode|[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md).|Указывает режим сопряжения iTunes. Возможные значения: `disallow`, `allow`, `requiresCertificate`.|
|managementCertificates|[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection|Сертификаты управления для Apple Configurator|
|restoreFromAndroidDisabled|Boolean|Указывает, отключено ли восстановление с Android|
|awaitDeviceConfiguredConfirmation|Boolean|Указывает, нужно ли устройству ждать настроенного подтверждения|
|sharedIPadMaximumUserCount|Int32|Это указывает максимальное число пользователей, которые могут использовать общие iPad. Применимо только в iPad режиме.|
|enableSharedIPad|Boolean|Это указывает, должно ли устройство быть зарегистрированным в режиме, который включает несколько сценариев пользователей. Применимо только в общих iPads.|
|companyPortalVppTokenId|Строка|Если установлено, указывается, какой маркер Vpp следует использовать для развертывания Корпоративный портал w/device licensing. Для этого свойства необходимо установить "enableAuthenticationViaCompanyPortal".|
|enableSingleAppEnrollmentMode|Boolean|Сообщает устройству включить режим одного приложения и применить блокировку приложения во время регистрации. Значение по умолчанию: false. Для этого свойства необходимо установить "enableAuthenticationViaCompanyPortal" и "companyPortalVppTokenId".|
|homeButtonScreenDisabled|Boolean|Указывает, отключен ли экран чувствительности домашней кнопки|
|iMessageAndFaceTimeScreenDisabled|Boolean|Указывает, отключен ли экран iMessage и FaceTime|
|onBoardingScreenDisabled|Boolean|Указывает, отключен ли экран установки бортовой установки|
|simSetupScreenDisabled|Boolean|Указывает, отключен ли экран SIMSetup|
|softwareUpdateScreenDisabled|Boolean|Указывает, отключен ли экран обязательного обновления sofware|
|watchMigrationScreenDisabled|Boolean|Указывает, отключен ли экран переноса часов|
|appearanceScreenDisabled|Boolean|Указывает, отключен ли экран Apperance|
|expressLanguageScreenDisabled|Boolean|Указывает, отключен ли экран express Language|
|preferredLanguageScreenDisabled|Boolean|Указывает, отключен ли предпочтительный языковой экран|
|deviceToDeviceMigrationDisabled|Boolean|Указывает, отключена ли миграция устройства на устройство|
|welcomeScreenDisabled|Boolean|Указывает, отключен ли экран Weclome|
|passCodeDisabled|Boolean|Указывает отключение области установки passcode|
|zoomDisabled|Boolean|Указывает, отключена ли панорама настройки масштабирования|
|restoreCompletedScreenDisabled|Boolean|Указывает, отключен ли экран Weclome|
|updateCompleteScreenDisabled|Boolean|Указывает, отключен ли экран Weclome|
|forceTemporarySession|Boolean|Указывает, включены ли временные сеансы|
|temporarySessionTimeoutInSeconds|Int32|Указывает время времени временного сеанса|
|userSessionTimeoutInSeconds|Int32|Указывает время времени временного сеанса|
|passcodeLockGracePeriodInSeconds|Int32|Указывает время перед блокировкой экрана, чтобы пользователь вошел в пасокд устройства, чтобы разблокировать его|
|carrierActivationUrl|Строка|URL-адрес carrier для активации eSIM устройства.|
|userlessSharedAadModeEnabled|Boolean|Указывает, что это устройство apple предназначено для поддержки сценариев "общего режима устройства". Это отличается от сценария "общие iPad". См [. общие устройства iOS и iPadOS](/mem/intune/enrollment/device-enrollment-shared-ios)|

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




