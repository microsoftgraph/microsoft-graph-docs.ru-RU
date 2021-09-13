---
title: тип ресурса depEnrollmentProfile
description: Ресурс depEnrollmentProfile представляет профиль программы регистрации устройств Apple (DEP). Этот тип профиля должен быть назначен серийным номерам DeP Apple, прежде чем соответствующие устройства смогут зарегистрироваться с помощью DEP.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2ed2fa9eb93eaf03d31d54390ab77569e9b976b0
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59091218"
---
# <a name="depenrollmentprofile-resource-type"></a>тип ресурса depEnrollmentProfile

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс depEnrollmentProfile представляет профиль программы регистрации устройств Apple (DEP). Этот тип профиля должен быть назначен серийным номерам DeP Apple, прежде чем соответствующие устройства смогут зарегистрироваться с помощью DEP.


Наследует [от enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список depEnrollmentProfiles](../api/intune-enrollment-depenrollmentprofile-list.md)|[коллекция depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)|Список свойств и связей объектов [depEnrollmentProfile.](../resources/intune-enrollment-depenrollmentprofile.md)|
|[Получить depEnrollmentProfile](../api/intune-enrollment-depenrollmentprofile-get.md)|[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md);|Чтение свойств и связей объекта [depEnrollmentProfile.](../resources/intune-enrollment-depenrollmentprofile.md)|
|[Создание depEnrollmentProfile](../api/intune-enrollment-depenrollmentprofile-create.md)|[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md);|Создайте новый [объект depEnrollmentProfile.](../resources/intune-enrollment-depenrollmentprofile.md)|
|[Удаление depEnrollmentProfile](../api/intune-enrollment-depenrollmentprofile-delete.md)|Нет|Удаляет [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md).|
|[Обновление depEnrollmentProfile](../api/intune-enrollment-depenrollmentprofile-update.md)|[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md);|Обновление свойств объекта [depEnrollmentProfile.](../resources/intune-enrollment-depenrollmentprofile.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|GUID для объекта Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|displayName|String|Имя профиля, унаследованной от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|description|String|Описание профиля, унаследованной от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requiresUserAuthentication|Логическое|Указывает, требует ли профиль проверки подлинности пользователя, унаследованной от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|configurationEndpointUrl|String|URL-адрес конечной точки конфигурации для использования для регистрации, унаследованной [от enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|enableAuthenticationViaCompanyPortal|Логическое|Указывает на проверку подлинности с помощью помощника установки Apple вместо Корпоративный портал. Унаследованный от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Логическое|Указывает, Корпоративный портал требуется на устройствах, зарегистрированных помощником установки, унаследованных от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|isDefault|Boolean|Указывает, является ли это профилем по умолчанию|
|supervisedModeEnabled|Логический|Режим Под контролем, True, чтобы включить, ложные в противном случае. Дополнительные https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune сведения см. в дополнительных сведениях.|
|supportDepartment|String|Сведения отдела поддержки|
|passCodeDisabled|Логический|Указывает отключение области установки passcode|
|isMandatory|Логическое|Указывает, является ли профиль обязательным|
|locationDisabled|Логическое|Указывает, отключена ли панорама установки службы расположения|
|supportPhoneNumber|String|Номер телефона поддержки|
|iTunesPairingMode|[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md).|Указывает режим сопряжения iTunes. Возможные значения: `disallow`, `allow`, `requiresCertificate`.|
|profileRemovalDisabled|Логическое|Указывает, отключен ли параметр удаления профиля|
|managementCertificates|[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection|Сертификаты управления для Apple Configurator|
|restoreBlocked|Логическое|Указывает, заблокирована ли настройка области восстановления|
|restoreFromAndroidDisabled|Логический|Указывает, отключено ли восстановление с Android|
|appleIdDisabled|Логический|Указывает, отключена ли области установки apple id|
|termsAndConditionsDisabled|Логическое|Указывает, отключено ли области установки "Условия и условия"|
|touchIdDisabled|Логический|Указывает, отключена ли настройка сенсорного id|
|applePayDisabled|Логическое|Указывает, отключена ли система установки apple pay|
|zoomDisabled|Логическое|Указывает, отключена ли панорама настройки масштабирования|
|siriDisabled|Логический|Указывает, отключено ли области настройки siri|
|diagnosticsDisabled|Логический|Указывает отключение области настройки диагностики|
|macOSRegistrationDisabled|Логическое|Указывает, отключена ли регистрация ОС Mac|
|macOSFileVaultDisabled|Логическое|Указывает, отключено ли хранилище файлов ОС Mac|
|awaitDeviceConfiguredConfirmation|Логический|Указывает, нужно ли устройству ждать настроенного подтверждения|
|sharedIPadMaximumUserCount|Int32|Это указывает максимальное число пользователей, которые могут использовать общие iPad. Применимо только в iPad режиме.|
|enableSharedIPad|Логическое|Это указывает, должно ли устройство быть зарегистрированным в режиме, который включает несколько сценариев пользователей. Применимо только в общих iPads.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.depEnrollmentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.depEnrollmentProfile",
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
  "passCodeDisabled": true,
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "String",
  "iTunesPairingMode": "String",
  "profileRemovalDisabled": true,
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "String",
      "certificate": "String"
    }
  ],
  "restoreBlocked": true,
  "restoreFromAndroidDisabled": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "macOSRegistrationDisabled": true,
  "macOSFileVaultDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 1024,
  "enableSharedIPad": true
}
```



