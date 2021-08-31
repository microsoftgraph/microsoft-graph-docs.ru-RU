---
title: тип ресурса depEnrollmentProfile
description: Ресурс depEnrollmentProfile представляет профиль программы регистрации устройств Apple (DEP). Этот тип профиля должен быть назначен серийным номерам DeP Apple, прежде чем соответствующие устройства смогут зарегистрироваться с помощью DEP.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5c3ee226769e9e24e5673992e36d9e765e320c88
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58800382"
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
|displayName|Строка|Имя профиля, унаследованной от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|description|Строка|Описание профиля, унаследованной от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requiresUserAuthentication|Boolean|Указывает, требует ли профиль проверки подлинности пользователя, унаследованной от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|configurationEndpointUrl|String|URL-адрес конечной точки конфигурации для использования для регистрации, унаследованной [от enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|enableAuthenticationViaCompanyPortal|Boolean|Указывает на проверку подлинности с помощью помощника установки Apple вместо Корпоративный портал. Унаследованный от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Логический|Указывает, Корпоративный портал требуется на устройствах, зарегистрированных помощником установки, унаследованных от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|isDefault|Boolean|Указывает, является ли это профилем по умолчанию|
|supervisedModeEnabled|Boolean|Режим Под контролем, True, чтобы включить, ложные в противном случае. Дополнительные https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune сведения см. в дополнительных сведениях.|
|supportDepartment|Строка|Сведения отдела поддержки|
|passCodeDisabled|Логический|Указывает отключение области установки passcode|
|isMandatory|Boolean|Указывает, является ли профиль обязательным|
|locationDisabled|Логический|Указывает, отключена ли панорама установки службы расположения|
|supportPhoneNumber|Строка|Номер телефона поддержки|
|iTunesPairingMode|[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md).|Указывает режим сопряжения iTunes. Возможные значения: `disallow`, `allow`, `requiresCertificate`.|
|profileRemovalDisabled|Логический|Указывает, отключен ли параметр удаления профиля|
|managementCertificates|[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection|Сертификаты управления для Apple Configurator|
|restoreBlocked|Boolean|Указывает, заблокирована ли настройка области восстановления|
|restoreFromAndroidDisabled|Логический|Указывает, отключено ли восстановление с Android|
|appleIdDisabled|Boolean|Указывает, отключена ли области установки apple id|
|termsAndConditionsDisabled|Логический|Указывает, отключено ли области установки "Условия и условия"|
|touchIdDisabled|Логический|Указывает, отключена ли настройка сенсорного id|
|applePayDisabled|Логический|Указывает, отключена ли система установки apple pay|
|zoomDisabled|Логический|Указывает, отключена ли панорама настройки масштабирования|
|siriDisabled|Логический|Указывает, отключено ли области настройки siri|
|diagnosticsDisabled|Логический|Указывает отключение области настройки диагностики|
|macOSRegistrationDisabled|Логический|Указывает, отключена ли регистрация ОС Mac|
|macOSFileVaultDisabled|Логический|Указывает, отключено ли хранилище файлов ОС Mac|
|awaitDeviceConfiguredConfirmation|Логический|Указывает, нужно ли устройству ждать настроенного подтверждения|
|sharedIPadMaximumUserCount|Int32|Это указывает максимальное число пользователей, которые могут использовать общие iPad. Применимо только в iPad режиме.|
|enableSharedIPad|Логический|Это указывает, должно ли устройство быть зарегистрированным в режиме, который включает несколько сценариев пользователей. Применимо только в общих iPads.|

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



