---
title: тип ресурса depEnrollmentProfile
description: Ресурс depEnrollmentProfile представляет профиль программы регистрации устройств Apple (DEP). Этот тип профиля должен быть назначен серийным номерам DeP Apple, прежде чем соответствующие устройства смогут зарегистрироваться с помощью DEP.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b2e6050e0807780bfc7423571fcaf51b574a0de8
ms.sourcegitcommit: 0076eb6abb89be3dca3575631924a74a5202be30
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2022
ms.locfileid: "64629199"
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
|[Список depEnrollmentProfiles](../api/intune-enrollment-depenrollmentprofile-list.md)|[коллекция depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)|Список свойств и связей объектов [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) .|
|[Получить depEnrollmentProfile](../api/intune-enrollment-depenrollmentprofile-get.md)|[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md);|Чтение свойств и связей объекта [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) .|
|[Создание depEnrollmentProfile](../api/intune-enrollment-depenrollmentprofile-create.md)|[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md);|Создайте новый [объект depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) .|
|[Удаление depEnrollmentProfile](../api/intune-enrollment-depenrollmentprofile-delete.md)|Нет|Удаляет [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md).|
|[Обновление depEnrollmentProfile](../api/intune-enrollment-depenrollmentprofile-update.md)|[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md);|Обновление свойств объекта [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|GUID для объекта Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|displayName|Строка|Имя профиля, унаследованной от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|description|Строка|Описание профиля, унаследованной от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requiresUserAuthentication|Boolean|Указывает, требует ли профиль проверки подлинности пользователя, унаследованной от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|configurationEndpointUrl|Строка|URL-адрес конечной точки конфигурации для использования для регистрации, унаследованной [от enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|enableAuthenticationViaCompanyPortal|Логический|Указывает на проверку подлинности с помощью помощника установки Apple вместо Корпоративный портал. Унаследованный от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Boolean|Указывает, Корпоративный портал требуется на устройствах, зарегистрированных помощником установки, унаследованных от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|isDefault|Boolean|Указывает, является ли это профилем по умолчанию|
|supervisedModeEnabled|Boolean|Режим Под контролем, True, чтобы включить, ложные в противном случае. Дополнительные сведения см. [в Microsoft Intune](/mem/intune/enrollment) устройствах регистрации.|
|supportDepartment|Строка|Сведения отдела поддержки|
|passCodeDisabled|Boolean|Указывает отключение области установки passcode|
|isMandatory|Логический|Указывает, является ли профиль обязательным|
|locationDisabled|Логическое|Указывает, отключена ли панорама установки службы расположения|
|supportPhoneNumber|Строка|Номер телефона поддержки|
|iTunesPairingMode|[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md)|Указывает режим сопряжения iTunes. Возможные значения: `disallow`, `allow`, `requiresCertificate`.|
|profileRemovalDisabled|Boolean|Указывает, отключен ли параметр удаления профиля|
|managementCertificates|[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection|Сертификаты управления для Apple Configurator|
|restoreBlocked|Логический|Указывает, заблокирована ли настройка области восстановления|
|restoreFromAndroidDisabled|Boolean|Указывает, отключено ли восстановление с Android|
|appleIdDisabled|Логическое|Указывает, отключена ли области установки apple id|
|termsAndConditionsDisabled|Логическое|Указывает, отключено ли области установки "Условия и условия"|
|touchIdDisabled|Boolean|Указывает, отключена ли настройка сенсорного id|
|applePayDisabled|Логическое|Указывает, отключена ли система установки apple pay|
|zoomDisabled|Boolean|Указывает, отключена ли панорама настройки масштабирования|
|siriDisabled|Boolean|Указывает, отключено ли области настройки siri|
|diagnosticsDisabled|Boolean|Указывает отключение области настройки диагностики|
|macOSRegistrationDisabled|Логическое|Указывает, отключена ли регистрация ОС Mac|
|macOSFileVaultDisabled|Boolean|Указывает, отключено ли хранилище файлов ОС Mac|
|awaitDeviceConfiguredConfirmation|Boolean|Указывает, нужно ли устройству ждать настроенного подтверждения|
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




