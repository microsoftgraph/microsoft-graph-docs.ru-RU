---
title: Тип ресурса depEnrollmentProfile
description: Ресурс depEnrollmentProfile представляет профиль регистрации программы регистрации устройств Apple (DEP). Этот тип профиля должен быть назначен серийным номерам Apple DEP, прежде чем соответствующие устройства смогут регистрироваться с помощью функции DEP.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0ecc14dcd7cf2d171259c76592352ff13bb6ed1d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166425"
---
# <a name="depenrollmentprofile-resource-type"></a>Тип ресурса depEnrollmentProfile

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс depEnrollmentProfile представляет профиль регистрации программы регистрации устройств Apple (DEP). Этот тип профиля должен быть назначен серийным номерам Apple DEP, прежде чем соответствующие устройства смогут регистрироваться с помощью функции DEP.


НаСледуется от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Депенроллментпрофилес](../api/intune-enrollment-depenrollmentprofile-list.md)|Коллекция [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)|Список свойств и связей объектов [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) .|
|[Получение depEnrollmentProfile](../api/intune-enrollment-depenrollmentprofile-get.md)|[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md);|Чтение свойств и связей объекта [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) .|
|[Создание depEnrollmentProfile](../api/intune-enrollment-depenrollmentprofile-create.md)|[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md);|Создание нового объекта [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) .|
|[Удаление depEnrollmentProfile](../api/intune-enrollment-depenrollmentprofile-delete.md)|Нет|Удаляет объект [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md).|
|[Обновление depEnrollmentProfile](../api/intune-enrollment-depenrollmentprofile-update.md)|[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md);|Обновление свойств объекта [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|GUID объекта, наСледуемого от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)|
|displayName|String|Имя профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)|
|description|String|Описание профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)|
|Рекуиресусераусентикатион|Логический|Указывает, требуется ли для профиля проверка подлинности пользователей, унаследованных от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)|
|Конфигуратионендпоинтурл|String|URL-адрес конечной точки конфигурации, используемый для регистрации, унаследованный от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)|
|enableAuthenticationViaCompanyPortal|Логический|Указывает на проверку подлинности с помощью помощника по настройке Apple, а не корпоративного портала. НаСледуется от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)|
|Рекуирекомпанипорталонсетупассистантенролледдевицес|Логический|Указывает, что корпоративный портал необходим на зарегистрированных устройствах помощника по настройке, наСледуемых от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)|
|isDefault|Логический|Указывает, является ли этот профиль профилем по умолчанию|
|Супервиседмодинаблед|Логический|Защищенный режим, true для включения, false в противном случае. Дополнительную https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune информацию можно узнать в статье.|
|Суппортдепартмент|String|Сведения о отделе поддержки|
|Пасскодедисаблед|Логический|Указывает, отключена ли область настройки секретного кода|
|Обязательный|Логический|Указывает, является ли профиль обязательной|
|Локатиондисаблед|Логический|Указывает, отключена ли область настройки службы расположения|
|Суппортфоненумбер|String|Номер телефона службы поддержки|
|iTunesPairingMode.|[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md).|Указывает режим связывания iTunes. Возможные значения: `disallow`, `allow`, `requiresCertificate`.|
|Профилеремовалдисаблед|Логический|Указывает, отключен ли параметр удаления профиля|
|Манажементцертификатес|Коллекция [манажементцертификатевиссумбпринт](../resources/intune-enrollment-managementcertificatewiththumbprint.md)|Сертификаты управления для конфигуратора Apple|
|Рестореблоккед|Логический|Указывает, заблокирована ли область настроек восстановления|
|Ресторефромандроиддисаблед|Логический|Указывает, отключено ли восстановление из Android|
|Апплеиддисаблед|Логический|Указывает, отключена ли область настройки Apple ID|
|Термсандкондитионсдисаблед|Логический|Указывает, отключена ли область установки "условия и условия"|
|Таучиддисаблед|Логический|Указывает, отключена ли панель настройки сенсорного экрана|
|Апплепайдисаблед|Логический|Указывает, отключена ли область настройки оплаты Apple|
|Зумдисаблед|Логический|Указывает, отключена ли область настройки масштабирования|
|Сиридисаблед|Логический|Указывает, отключена ли область настройки Siri|
|Диагностиксдисаблед|Логический|Указывает, отключена ли область настройки диагностики|
|Макосрегистратиондисаблед|Логический|Указывает, отключена ли регистрация Mac OS|
|Макосфилеваултдисаблед|Логический|Указывает, отключено ли хранилище файлов Mac OS|
|Аваитдевицеконфигуредконфирматион|Логический|Указывает, должно ли устройство ждать настройки подтверждения.|
|Свойства sharedipadmaximumusercount|Int32|Указывает максимальное количество пользователей, которые могут использовать общий iPad. Относится только к общему режиму iPad.|
|Enablesharedipad к|Логический|Указывает, следует ли зарегистрировать устройство в режиме, позволяющем использовать сценарии с несколькими пользователями. Применяется только в общих iPad.|

## <a name="relationships"></a>Отношения
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




