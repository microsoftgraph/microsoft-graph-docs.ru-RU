---
title: Тип ресурса depEnrollmentProfile
description: Ресурс depEnrollmentProfile представляет профиль регистрации программы регистрации устройств Apple (DEP). Этот тип профиля должен быть назначен серийным номерам Apple DEP, прежде чем соответствующие устройства смогут регистрироваться с помощью функции DEP.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 025b104ea43745c3885806ec977e277e8dc3a68e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724405"
---
# <a name="depenrollmentprofile-resource-type"></a>Тип ресурса depEnrollmentProfile

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс depEnrollmentProfile представляет профиль регистрации программы регистрации устройств Apple (DEP). Этот тип профиля должен быть назначен серийным номерам Apple DEP, прежде чем соответствующие устройства смогут регистрироваться с помощью функции DEP.


Наследуется от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)

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
|id|Строка|GUID объекта, наследуемого от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)|
|displayName|Строка|Имя профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)|
|description|Строка|Описание профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)|
|рекуиресусераусентикатион|Логический|Указывает, требуется ли для профиля проверка подлинности пользователей, унаследованных от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)|
|конфигуратионендпоинтурл|Строка|URL-адрес конечной точки конфигурации, используемый для регистрации, унаследованный от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)|
|enableAuthenticationViaCompanyPortal|Логический|Указывает на проверку подлинности с помощью помощника по настройке Apple, а не корпоративного портала. Наследуется от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)|
|рекуирекомпанипорталонсетупассистантенролледдевицес|Логический|Указывает, что корпоративный портал необходим на зарегистрированных устройствах помощника по настройке, наследуемых от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)|
|isDefault|Boolean|Указывает, является ли этот профиль профилем по умолчанию|
|супервиседмодинаблед|Логический|Защищенный режим, true для включения, false в противном случае. https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intuneДополнительную информацию можно узнать в статье.|
|суппортдепартмент|Строка|Сведения о отделе поддержки|
|пасскодедисаблед|Логический|Указывает, отключена ли область настройки секретного кода|
|Обязательный|Логический|Указывает, является ли профиль обязательной|
|локатиондисаблед|Логический|Указывает, отключена ли область настройки службы расположения|
|суппортфоненумбер|Строка|Номер телефона службы поддержки|
|iTunesPairingMode|[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md).|Указывает режим связывания iTunes. Возможные значения: `disallow`, `allow`, `requiresCertificate`.|
|профилеремовалдисаблед|Логический|Указывает, отключен ли параметр удаления профиля|
|манажементцертификатес|Коллекция [манажементцертификатевиссумбпринт](../resources/intune-enrollment-managementcertificatewiththumbprint.md)|Сертификаты управления для конфигуратора Apple|
|рестореблоккед|Логический|Указывает, заблокирована ли область настроек восстановления|
|ресторефромандроиддисаблед|Логический|Указывает, отключено ли восстановление из Android|
|апплеиддисаблед|Логический|Указывает, отключена ли область настройки Apple ID|
|термсандкондитионсдисаблед|Логический|Указывает, отключена ли область установки "условия и условия"|
|таучиддисаблед|Логический|Указывает, отключена ли панель настройки сенсорного экрана|
|апплепайдисаблед|Логический|Указывает, отключена ли область настройки оплаты Apple|
|зумдисаблед|Логический|Указывает, отключена ли область настройки масштабирования|
|сиридисаблед|Логический|Указывает, отключена ли область настройки Siri|
|диагностиксдисаблед|Логический|Указывает, отключена ли область настройки диагностики|
|макосрегистратиондисаблед|Логический|Указывает, отключена ли регистрация Mac OS|
|макосфилеваултдисаблед|Логический|Указывает, отключено ли хранилище файлов Mac OS|
|аваитдевицеконфигуредконфирматион|Логический|Указывает, должно ли устройство ждать настройки подтверждения.|
|Свойства sharedipadmaximumusercount|Int32|Указывает максимальное количество пользователей, которые могут использовать общий iPad. Относится только к общему режиму iPad.|
|Enablesharedipad к|Логический|Указывает, следует ли зарегистрировать устройство в режиме, позволяющем использовать сценарии с несколькими пользователями. Применяется только в общих iPad.|

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





